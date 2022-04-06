---
title: Microsoft Graph Toolkit
description: 使用自定义模板修改组件的内容。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 2632b726c1f2260afe31dacb8c487d5976224be7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587775"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Microsoft Graph Toolkit

大多数 Microsoft Graph Toolkit组件都支持使用自定义模板来修改组件的内容。

所有 Web 组件都支持基于 元素的 `<template>` 模板。 例如，若要替代组件的模板，在组件 `<template>` 中添加元素。

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

如果你使用的是 Microsoft Graph Toolkit React组件，可以使用React模板。 有关详细信息，请参阅[将工具包与 React](../get-started/mgt-react.md)。

## <a name="data-type"></a>数据类型

每个组件可以有多个可模板创建的部件。 例如，在 `mgt-agenda` 组件中，可以模板单个事件、单个节标题、加载视图、无数据视图等。 若要指示模板，请使用 `data-type` 模板上的 属性。 例如，若要为 中的每个事件 `mgt-agenda`创建模板，请使用 `event` 数据类型，如下所示。

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

如果未指定 `data-type` ，则整个组件将替换为模板。 您还可以用于 `data-type="default"` 同一目的。

## <a name="binding-data"></a>绑定数据

许多模板允许绑定作为数据上下文传递给模板的数据。 例如，组件 `event` 中的模板 `mgt-agenda` 传递可以直接 `{event}` 在模板中使用的对象。 若要展开表达式（如 ） `event.subject`，请使用双花括号。

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

此格式还可在属性内使用：

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> **注意：** 还可以展开 或 等对象`{{event}}``{{this}}`，它们将呈现为 JSON 字符串。 在开发模板时，这非常有用。

### <a name="change-binding-syntax"></a>更改绑定语法

默认情况下，若要展开表达式，请使用双花括号 () `{{expression}}` 。 但是，您可以更改已使用双括号语法的环境的此语法。 例如，以下示例使用双方括号 () `[[expression]]` 。

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a>数据上下文帮助程序属性

以下属性还可与模板中的数据上下文对象一同使用。

| 属性 | 说明                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| $index   | 使用 循环时呈现的项目的数字索引 `data-for`。                                     |
| $parent  | 如果模板呈现在另一个模板内，则此属性允许您访问父数据上下文。 |

以下示例演示如何在 data-for `$index` 循环中使用 属性。

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

### <a name="this"></a>{{this}}

为了帮助调试数据上下文，可以在绑定 `this` 表达式中使用。 最简单的表单是在模板中的任何 `{{this}}` 位置添加。

```html
<template data-type="event">
  <div>
    {{this}}
  </div>
</template>
```

由于可以在绑定表达式中使用 JavaScript [`console`](https://developer.mozilla.org/docs/Web/API/Console) `console.log(this)` `console` ，因此还可以访问对象，该对象允许你在模板 (任何其他 API) 。

```html
<template data-type="event">
  <div>
    {{console.log(this)}}
  </div>
</template>
```

## <a name="conditional-rendering"></a>条件呈现

您可能只希望根据数据上下文在条件为 true 或 false 时呈现元素。 `data-else`和 `data-if` 属性可以计算表达式，并且仅在 true 或 false 时呈现。

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

在某些情况下，数据上下文对象包含循环，并且你需要循环访问数据。 对于此方案，请使用 `data-for` 属性。

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

在需要转换绑定中数据、绑定到事件或仅使用模板绑定中的外部数据的方案中，模板支持绑定到外部数据上下文。 可以通过两种方式添加其他模板上下文：

1. 直接在组件上。

    每个组件都定义 `templateContext` 属性，可用于向组件中的任意模板传递其他数据。

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    对象中的 `templateContext` 属性现在可用于模板中的绑定表达式。

2. 针对所有组件的全局性。

    类 `TemplateHelper` 公开对象以 `globalContext` 添加应在全局上可供所有组件使用的数据或函数。

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a>转换器

在许多情况下，您可能希望先转换数据，然后再将数据呈现在模板中。 例如，您可能希望在呈现日期之前正确设置日期的格式。 在这些情况下，您可能需要使用模板转换器。

若要使用模板转换器，首先需要定义一个将执行转换的函数。 例如，您可以定义一个函数以将事件对象转换为格式化的时区。

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

若要在模板中使用此转换器，请使用它，就像在代码隐藏部分使用函数一样。

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a>事件或属性绑定

通过 `data-props` 属性，您可以直接在模板中添加事件侦听器或设置属性值。

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

data-props 接受您可能要设置的每个属性或事件处理程序的逗号分隔字符串。

若要添加事件处理程序，请以 作为事件名称的前缀 `@`。 事件处理程序将需要在 元素中 `templateContext` 可用。

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

事件参数、数据上下文和模板的根元素作为参数传递给事件处理程序。


## <a name="template-rendered-event"></a>模板呈现事件

在某些情况下，您可能希望获取对已呈现元素的引用。 如果希望自己处理内容的呈现，或者要修改呈现的元素，这将非常有用。

在此方案中，可以使用事件 `templateRendered` ，该事件在模板呈现后触发。

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

事件详细信息将包含对要呈现的元素的引用、数据上下文对象和模板的类型。

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

## <a name="styling"></a>样式设置

模板可以通过 CSS 正常设置样式，因为它们呈现在阴影 dom 之外。
