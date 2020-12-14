---
title: Templates in the Microsoft Graph Toolkit
description: 使用自定义模板修改组件的内容。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 94529f45c95dcfdd56ade2dffc7b4ac7bf48babb
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658588"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Templates in the Microsoft Graph Toolkit

大多数 Microsoft Graph Toolkit组件都支持使用自定义模板来修改组件的内容。

所有 Web 组件都支持基于该元素的 `<template>` 模板。 例如，若要替代组件的模板，在组件 `<template>` 内添加元素。

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

如果你使用的是 Microsoft Graph Toolkit React 组件，可以使用 React 创作模板。 有关详细信息，请参阅 [使用 React 工具包](../get-started/mgt-react.md)。

## <a name="data-type"></a>数据类型

每个组件可以包含多个可模板的部件。 例如，在组件中，可以模板单个事件、单个节标题、 `mgt-agenda` 加载视图、无数据视图等。 若要指示模板，请使用 `data-type` 模板上的属性。 例如，若要为中的每个事件创建模板 `mgt-agenda` ，请使用 `event` 数据类型，如下所示。

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

如果 `data-type` 未指定，则整个组件将替换为模板。 您还可以用于 `data-type="default"` 同一目的。

## <a name="binding-data"></a>绑定数据

许多模板允许绑定作为数据上下文传递给模板的数据。 例如， `event` 组件中的模板传递可以直接在模板 `mgt-agenda` `{event}` 中使用的对象。 若要展开表达式（如 `event.subject` ，请使用双大括号）。

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

> **注意：** 还可以展开对象，例如 `{{event}}` 或 `{{this}}` 对象将呈现为 JSON 字符串。 在开发模板时，这非常有用。

### <a name="change-binding-syntax"></a>更改绑定语法

默认情况下，若要展开表达式，请使用双花括号 `{{expression}}` () 。 但是，您可以更改已使用双大括号语法的环境的此语法。 例如，以下示例使用双方括号 `[[expression]]` () 。

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a>数据上下文帮助程序属性

以下属性还可以与模板中的数据上下文对象一同使用。

| 属性 | 说明                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| $index   | 与 循环时呈现的项目的数字索引 `data-for` 。                                     |
| $parent  | 如果模板在另一个模板内呈现，则此属性允许您访问父数据上下文。 |

以下示例演示如何在数据 for `$index` 循环中使用该属性。

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

您可能只希望根据数据上下文在条件为 true 或 false 时呈现元素。 and `data-if` `data-else` 属性可以计算表达式，并且仅在 true 或 false 时呈现。

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

    每个组件都定义属性，可用于向组件中的 `templateContext` 任意模板传递其他数据。

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    对象中的 `templateContext` 属性现在可用于模板中的绑定表达式。

2. 全局所有组件。

    该类 `TemplateHelper` 公开对象以添加应全局可用于所有组件 `globalContext` 的数据或函数。

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a>转换器

在许多情况下，您可能希望先转换数据，然后再将数据呈现在模板中。 例如，您可能希望在呈现日期之前正确设置日期的格式。 在这些情况下，您可能需要使用模板转换器。

若要使用模板转换器，首先需要定义将执行转换的函数。 例如，您可以定义一个函数以将事件对象转换为格式化的时区。

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

若要在模板中使用该转换器，请使用它，就像在代码隐藏部分使用函数一样。

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a>事件或属性绑定

`data-props`该属性允许你直接在模板中添加事件侦听器或设置属性值。

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

对于您可能需要设置的每个属性或事件处理程序，数据属性接受逗号分隔的字符串。

若要添加事件处理程序，请为事件的名称加上前缀 `@` 。 事件处理程序将需要在元素 `templateContext` 中可用。

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


## <a name="template-rendered-event"></a>模板呈现的事件

在某些情况下，您可能希望获取对呈现的元素的引用。 如果你希望自己处理内容的呈现，或者要修改呈现的元素，这将非常有用。

在此方案中，可以使用呈现模板后 `templateRendered` 触发的事件。

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

事件详细信息将包含对正在呈现的元素、数据上下文对象和模板类型的引用。

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
