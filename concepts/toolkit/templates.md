---
title: Microsoft Graph 工具包中的模板
description: 使用自定义模板修改组件的内容。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 00be58b006fd4442154f547603cf1f2c5dbeb5a5
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682241"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的模板

使用自定义模板修改组件的内容。

所有 web 组件都支持基于元素的模板 `<template>` 。 例如，若要覆盖组件的模板，请 `<template>` 在组件中添加元素。

```html
<mgt-agenda>
  <template data-type="event">
      <div>{{event.subject}}</div>
      <div data-for='attendee in event.attendees'>
          <mgt-person person-query="{{attendee.emailAddress.name}}">
            <template>
              <div data-if="person.image">
                <img src="{{person.image}}" />
              </div>
              <div data-else>
                {{person.displayName}}
              </div>
            </template>
          </mgt-person>
      </div>
  </template>
</mgt-agenda>
```

## <a name="data-type"></a>数据类型

每个组件都可以具有多个可模板化的部件。 例如，在组件中 `mgt-agenda` ，可以对单个事件、各个节标题、加载视图、无数据视图等进行模板。 若要指示模板，请使用 `data-type` 模板上的属性。 例如，若要在中为每个事件提供模板 `mgt-agenda` ，请使用 `event` 数据类型，如下所示。

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

如果 `data-type` 指定为 "否"，则整个组件将替换为模板。 您也可以使用 `data-type="default"` 相同的目的。

## <a name="binding-data"></a>绑定数据

许多模板允许将作为数据上下文传递给模板的数据绑定。 例如， `event` 组件中的模板 `mgt-agenda` 传递 `{event}` 可直接在模板中使用的对象。 若要展开表达式（例如 `event.subject` ），请使用双花括号。

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

此外，还可以在属性内使用此格式：

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> **注意：** 您还可以展开诸如等对象 `{{event}}` ，它们将呈现为 JSON 字符串。 这在开发模板时可能很有用。

### <a name="change-binding-syntax"></a>更改绑定语法

默认情况下，若要展开表达式，请使用双花括号（ `{{expression}}` ）。 但是，您可以为已使用双花括号语法的环境更改此语法。 例如，下面的示例使用双方括号（ `[[expression]]` ）。

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a>数据上下文帮助程序属性

下列属性也可以与模板中的数据上下文对象一起使用。

| 属性 |  说明 |
| --- | --- | --- |
| $index | 循环使用时呈现的项的数字索引 `data-for` 。 |
| $parent | 如果模板呈现在另一个模板中，则此属性允许您访问父数据上下文。 |

下面的示例演示如何 `$index` 在数据 for 循环中使用该属性。

```html
<mgt-person>
  <mgt-person-card>
    <template data-type="additional-details">
      <span data-for="language in languages">
        {{ language.displayName }}<span data-if="$index < languages.length - 1">, </span>
      </span>
    </template>
  </mgt-person-card>
</mgt-person>
```

## <a name="conditional-rendering"></a>条件呈现

您可能只希望在条件为 true 或 false 时呈现基于数据上下文的元素。 `data-if`和 `data-else` 属性可以计算表达式，并且只有在 true 或 false 时才会呈现。

```html
<mgt-person person-query="john doe">
  <template>
    <div data-if="person.image">
      <img src="{{ person.image }}" />
    </div>
    <div data-else>
      {{ person.displayName }}
    </div>
  </template>
</mgt-person>
```

## <a name="looping"></a>循环

在某些情况下，数据上下文对象包含循环，您需要对数据循环。 对于此方案，请使用 `data-for` 属性。

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a>模板上下文

在需要转换绑定中的数据、绑定到事件或仅在模板绑定中使用外部数据的情况下，这些模板支持绑定到外部数据上下文。 您可以通过两种方式添加其他模板上下文：

1. 直接在组件上。

    每个组件定义 `templateContext` 属性，您可以使用该属性将其他数据传递到组件中的任何模板。 

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    此时，该对象中的属性 `templateContext` 将可用于模板中的绑定表达式。

2. 对所有组件全局。

    `TemplateHelper`类公开 `globalContext` 对象，以添加全局可用于所有组件的数据或函数。

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a>转换器

在很多情况下，您可能需要在将数据呈现在模板中之前对数据进行转换。 例如，您可能希望在呈现日期之前正确设置日期格式。 在这些情况下，您可能需要使用模板转换器。

若要使用模板转换器，首先需要定义将执行转换的函数。 例如，您可以定义一个函数来将事件对象转换为格式化的时间范围。

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

若要在模板中使用转换器，请使用它，就像在代码隐藏中使用函数一样。

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a>事件或属性绑定

`data-props`属性允许您添加事件侦听器或直接在模板中设置属性值。 

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

对于您可能想要设置的每个属性或事件处理程序，数据属性接受以逗号分隔的字符串。 

若要添加事件处理程序，请为事件的名称加上前缀 `@` 。 事件处理程序将需要在元素的中可用 `templateContext` 。

```ts
document.querySelector('mgt-agenda').templateContext = {

  someEventHandler: (e, context, root) => { /* handleEvent */  }

}
```

```html
<template>
    <button data-props="{{@click: someEventHandler}}"></button>
</template>
```

将模板的事件参数、数据上下文和根元素作为参数传递给事件处理程序。


## <a name="template-rendered-event"></a>模板呈现事件

在某些情况下，您可能需要获取对呈现的元素的引用。 如果您希望自己处理内容的呈现，或者想要修改呈现的元素，这会非常有用。

在这种情况下，您可以使用 `templateRendered` 事件，该事件将在呈现模板后触发。

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

事件详细信息将包含对要呈现的元素、数据上下文对象和模板类型的引用。

```ts
agenda.addEventListener('templateRendered', (e) => { 
  let templateType = e.detail.templateType;
  let dataContext = e.detail.context;
  let element = e.detail.element;

  if (templateType === 'event') {
    element.querySelector('.some-button').addEventListener('click', () => {});
  }
});
```

## <a name="styling"></a>样式

可以通过 CSS 对模板进行样式化，因为它们呈现在阴影 dom 外部。
