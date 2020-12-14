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
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="fd0cf-103">Templates in the Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="fd0cf-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="fd0cf-104">大多数 Microsoft Graph Toolkit组件都支持使用自定义模板来修改组件的内容。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-104">Most Microsoft Graph Toolkit components support the use of custom templates to modify the content of a component.</span></span>

<span data-ttu-id="fd0cf-105">所有 Web 组件都支持基于该元素的 `<template>` 模板。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="fd0cf-106">例如，若要替代组件的模板，在组件 `<template>` 内添加元素。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

<span data-ttu-id="fd0cf-107">如果你使用的是 Microsoft Graph Toolkit React 组件，可以使用 React 创作模板。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-107">If you're using the Microsoft Graph Toolkit React components, you can use React for authoring templates.</span></span> <span data-ttu-id="fd0cf-108">有关详细信息，请参阅 [使用 React 工具包](../get-started/mgt-react.md)。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-108">For details, see [Use the toolkit with React](../get-started/mgt-react.md).</span></span>

## <a name="data-type"></a><span data-ttu-id="fd0cf-109">数据类型</span><span class="sxs-lookup"><span data-stu-id="fd0cf-109">Data-type</span></span>

<span data-ttu-id="fd0cf-110">每个组件可以包含多个可模板的部件。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-110">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="fd0cf-111">例如，在组件中，可以模板单个事件、单个节标题、 `mgt-agenda` 加载视图、无数据视图等。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-111">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="fd0cf-112">若要指示模板，请使用 `data-type` 模板上的属性。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-112">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="fd0cf-113">例如，若要为中的每个事件创建模板 `mgt-agenda` ，请使用 `event` 数据类型，如下所示。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-113">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="fd0cf-114">如果 `data-type` 未指定，则整个组件将替换为模板。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-114">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="fd0cf-115">您还可以用于 `data-type="default"` 同一目的。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-115">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="fd0cf-116">绑定数据</span><span class="sxs-lookup"><span data-stu-id="fd0cf-116">Binding data</span></span>

<span data-ttu-id="fd0cf-117">许多模板允许绑定作为数据上下文传递给模板的数据。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-117">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="fd0cf-118">例如， `event` 组件中的模板传递可以直接在模板 `mgt-agenda` `{event}` 中使用的对象。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-118">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="fd0cf-119">若要展开表达式（如 `event.subject` ，请使用双大括号）。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-119">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="fd0cf-120">此格式还可在属性内使用：</span><span class="sxs-lookup"><span data-stu-id="fd0cf-120">This format can also be used inside attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="fd0cf-121">**注意：** 还可以展开对象，例如 `{{event}}` 或 `{{this}}` 对象将呈现为 JSON 字符串。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-121">**Note:** You can also expand objects such as `{{event}}` or `{{this}}` and they will render as JSON strings.</span></span> <span data-ttu-id="fd0cf-122">在开发模板时，这非常有用。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-122">This can be useful when you're developing the templates.</span></span>

### <a name="change-binding-syntax"></a><span data-ttu-id="fd0cf-123">更改绑定语法</span><span class="sxs-lookup"><span data-stu-id="fd0cf-123">Change binding syntax</span></span>

<span data-ttu-id="fd0cf-124">默认情况下，若要展开表达式，请使用双花括号 `{{expression}}` () 。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-124">By default, to expand an expression, you use double curly brackets ( `{{expression}}` ).</span></span> <span data-ttu-id="fd0cf-125">但是，您可以更改已使用双大括号语法的环境的此语法。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-125">However, you can change this syntax for environments where the double curly bracket syntax is already used.</span></span> <span data-ttu-id="fd0cf-126">例如，以下示例使用双方括号 `[[expression]]` () 。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-126">For example, the following example uses double square brackets ( `[[expression]]` ).</span></span>

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a><span data-ttu-id="fd0cf-127">数据上下文帮助程序属性</span><span class="sxs-lookup"><span data-stu-id="fd0cf-127">Data context helper properties</span></span>

<span data-ttu-id="fd0cf-128">以下属性还可以与模板中的数据上下文对象一同使用。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-128">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="fd0cf-129">属性</span><span class="sxs-lookup"><span data-stu-id="fd0cf-129">Property</span></span> | <span data-ttu-id="fd0cf-130">说明</span><span class="sxs-lookup"><span data-stu-id="fd0cf-130">Description</span></span>                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fd0cf-131">$index</span><span class="sxs-lookup"><span data-stu-id="fd0cf-131">$index</span></span>   | <span data-ttu-id="fd0cf-132">与 循环时呈现的项目的数字索引 `data-for` 。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-132">Numerical index of item being rendered while being looped with `data-for`.</span></span>                                     |
| <span data-ttu-id="fd0cf-133">$parent</span><span class="sxs-lookup"><span data-stu-id="fd0cf-133">$parent</span></span>  | <span data-ttu-id="fd0cf-134">如果模板在另一个模板内呈现，则此属性允许您访问父数据上下文。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-134">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="fd0cf-135">以下示例演示如何在数据 for `$index` 循环中使用该属性。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-135">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

## <a name="conditional-rendering"></a><span data-ttu-id="fd0cf-136">条件呈现</span><span class="sxs-lookup"><span data-stu-id="fd0cf-136">Conditional rendering</span></span>

<span data-ttu-id="fd0cf-137">您可能只希望根据数据上下文在条件为 true 或 false 时呈现元素。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-137">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="fd0cf-138">and `data-if` `data-else` 属性可以计算表达式，并且仅在 true 或 false 时呈现。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-138">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="fd0cf-139">循环</span><span class="sxs-lookup"><span data-stu-id="fd0cf-139">Looping</span></span>

<span data-ttu-id="fd0cf-140">在某些情况下，数据上下文对象包含循环，并且你需要循环访问数据。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-140">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="fd0cf-141">对于此方案，请使用 `data-for` 属性。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-141">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a><span data-ttu-id="fd0cf-142">模板上下文</span><span class="sxs-lookup"><span data-stu-id="fd0cf-142">Template context</span></span>

<span data-ttu-id="fd0cf-143">在需要转换绑定中数据、绑定到事件或仅使用模板绑定中的外部数据的方案中，模板支持绑定到外部数据上下文。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-143">In scenarios where you need to convert data in your bindings, bind to events, or just use external data in your templates bindings, the templates support binding to external data context.</span></span> <span data-ttu-id="fd0cf-144">可以通过两种方式添加其他模板上下文：</span><span class="sxs-lookup"><span data-stu-id="fd0cf-144">You can add additional template context in two ways:</span></span>

1. <span data-ttu-id="fd0cf-145">直接在组件上。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-145">Directly on the component.</span></span>

    <span data-ttu-id="fd0cf-146">每个组件都定义属性，可用于向组件中的 `templateContext` 任意模板传递其他数据。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-146">Each component defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span>

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    <span data-ttu-id="fd0cf-147">对象中的 `templateContext` 属性现在可用于模板中的绑定表达式。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-147">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

2. <span data-ttu-id="fd0cf-148">全局所有组件。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-148">Globally for all components.</span></span>

    <span data-ttu-id="fd0cf-149">该类 `TemplateHelper` 公开对象以添加应全局可用于所有组件 `globalContext` 的数据或函数。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-149">The `TemplateHelper` class exposes the `globalContext` object to add data or functions that should be globally available for all components.</span></span>

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a><span data-ttu-id="fd0cf-150">转换器</span><span class="sxs-lookup"><span data-stu-id="fd0cf-150">Converters</span></span>

<span data-ttu-id="fd0cf-151">在许多情况下，您可能希望先转换数据，然后再将数据呈现在模板中。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-151">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="fd0cf-152">例如，您可能希望在呈现日期之前正确设置日期的格式。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-152">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="fd0cf-153">在这些情况下，您可能需要使用模板转换器。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-153">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="fd0cf-154">若要使用模板转换器，首先需要定义将执行转换的函数。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-154">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="fd0cf-155">例如，您可以定义一个函数以将事件对象转换为格式化的时区。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-155">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="fd0cf-156">若要在模板中使用该转换器，请使用它，就像在代码隐藏部分使用函数一样。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-156">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="fd0cf-157">事件或属性绑定</span><span class="sxs-lookup"><span data-stu-id="fd0cf-157">Event or property binding</span></span>

<span data-ttu-id="fd0cf-158">`data-props`该属性允许你直接在模板中添加事件侦听器或设置属性值。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-158">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span>

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="fd0cf-159">对于您可能需要设置的每个属性或事件处理程序，数据属性接受逗号分隔的字符串。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-159">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span>

<span data-ttu-id="fd0cf-160">若要添加事件处理程序，请为事件的名称加上前缀 `@` 。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-160">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="fd0cf-161">事件处理程序将需要在元素 `templateContext` 中可用。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-161">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="fd0cf-162">事件参数、数据上下文和模板的根元素作为参数传递给事件处理程序。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-162">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="fd0cf-163">模板呈现的事件</span><span class="sxs-lookup"><span data-stu-id="fd0cf-163">Template rendered event</span></span>

<span data-ttu-id="fd0cf-164">在某些情况下，您可能希望获取对呈现的元素的引用。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-164">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="fd0cf-165">如果你希望自己处理内容的呈现，或者要修改呈现的元素，这将非常有用。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-165">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="fd0cf-166">在此方案中，可以使用呈现模板后 `templateRendered` 触发的事件。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-166">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="fd0cf-167">事件详细信息将包含对正在呈现的元素、数据上下文对象和模板类型的引用。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-167">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="fd0cf-168">样式设置</span><span class="sxs-lookup"><span data-stu-id="fd0cf-168">Styling</span></span>

<span data-ttu-id="fd0cf-169">模板可以通过 CSS 正常设置样式，因为它们呈现在阴影 dom 之外。</span><span class="sxs-lookup"><span data-stu-id="fd0cf-169">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
