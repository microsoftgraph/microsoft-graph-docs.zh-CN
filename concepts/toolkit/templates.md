---
title: Microsoft Graph 工具包中的模板
description: 使用自定义模板修改组件的内容。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 46a1f9b771f358de6099bf1266c10c4c1ebe0cb0
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144259"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的模板

使用自定义模板修改组件的内容。

所有 web 组件都支持基于元素的`<template>`模板。 例如，若要覆盖组件的模板，请在组件中`<template>`添加元素。

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

每个组件都可以具有多个可模板化的部件。 例如，在`mgt-agenda`组件中，可以对单个事件、各个节标题、加载视图、无数据视图等进行模板。 若要指示模板，请使用`data-type`模板上的属性。 例如，若要在中为每个`mgt-agenda`事件提供模板`event` ，请使用数据类型，如下所示。

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

如果指定`data-type`为 "否"，则整个组件将替换为模板。 您也可以使用`data-type="default"`相同的目的。

## <a name="binding-data"></a>绑定数据

许多模板允许将作为数据上下文传递给模板的数据绑定。 例如， `event` `mgt-agenda`组件中的模板传递可直接在`{event}`模板中使用的对象。 若要展开表达式（例如`event.subject`），请使用双花括号。

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

> **注意：** 您还可以展开诸如等对象`{{event}}` ，它们将呈现为 JSON 字符串。 这在开发模板时可能很有用。

## <a name="data-context-helper-properties"></a>数据上下文帮助程序属性

下列属性也可以与模板中的数据上下文对象一起使用。

| 属性 |  说明 |
| --- | --- | --- |
| $index | 循环使用`data-for`时呈现的项的数字索引。 |
| $parent | 如果模板呈现在另一个模板中，则此属性允许您访问父数据上下文。 |

下面的示例演示如何在数据 for `$index`循环中使用该属性。

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

您可能只希望在条件为 true 或 false 时呈现基于数据上下文的元素。 `data-if`和`data-else`属性可以计算表达式，并且只有在 true 或 false 时才会呈现。

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

在某些情况下，数据上下文对象包含循环，您需要对数据循环。 对于此方案，请使用`data-for`属性。

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="templatecontext"></a>TemplateContext

Microsoft Graph 工具包中的每个组件都`templateContext`定义了属性，可使用该属性将其他数据传递到组件中的任何模板。 

```ts
document.querySelector('mgt-agenda').templateContext = {

  someObject: {},
  formatDate: (date: Date) => { /* format date and return */ },
  someEventHandler: (e) => { /* handleEvent */  }

}
```

此时，该`templateContext`对象中的属性将可用于模板中的绑定表达式。

这在很多情况下都很有用，例如在绑定中转换数据或绑定到事件。 

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

若要添加事件处理程序，请为事件的名称加`@`上前缀。 事件处理程序将需要在元素`templateContext`的中可用。

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

在这种情况下，您可以`templateRendered`使用事件，该事件将在呈现模板后触发。

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
