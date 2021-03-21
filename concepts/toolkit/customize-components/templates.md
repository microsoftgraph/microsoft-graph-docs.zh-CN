---
title: Microsoft Graph 模板Toolkit
description: 使用自定义模板修改组件的内容。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 1db3f315cd89932481a0a2325eecae19592d9276
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963279"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="07950-103">Microsoft Graph 模板Toolkit</span><span class="sxs-lookup"><span data-stu-id="07950-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="07950-104">大多数 Microsoft Graph Toolkit组件都支持使用自定义模板来修改组件的内容。</span><span class="sxs-lookup"><span data-stu-id="07950-104">Most Microsoft Graph Toolkit components support the use of custom templates to modify the content of a component.</span></span>

<span data-ttu-id="07950-105">所有 Web 组件都支持基于 元素的 `<template>` 模板。</span><span class="sxs-lookup"><span data-stu-id="07950-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="07950-106">例如，若要替代组件的模板，在组件 `<template>` 内添加元素。</span><span class="sxs-lookup"><span data-stu-id="07950-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

<span data-ttu-id="07950-107">如果你使用的是 Microsoft Graph 和 React Toolkit，可以使用 React 创作模板。</span><span class="sxs-lookup"><span data-stu-id="07950-107">If you're using the Microsoft Graph Toolkit React components, you can use React for authoring templates.</span></span> <span data-ttu-id="07950-108">有关详细信息，请参阅 [将工具包与 React 一同使用](../get-started/mgt-react.md)。</span><span class="sxs-lookup"><span data-stu-id="07950-108">For details, see [Use the toolkit with React](../get-started/mgt-react.md).</span></span>

## <a name="data-type"></a><span data-ttu-id="07950-109">数据类型</span><span class="sxs-lookup"><span data-stu-id="07950-109">Data-type</span></span>

<span data-ttu-id="07950-110">每个组件可以有多个可模板创建的部件。</span><span class="sxs-lookup"><span data-stu-id="07950-110">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="07950-111">例如，在组件中，可以模板单个事件、单个节标题、 `mgt-agenda` 加载视图、无数据视图等。</span><span class="sxs-lookup"><span data-stu-id="07950-111">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="07950-112">若要指示模板，请使用 `data-type` 模板上的 属性。</span><span class="sxs-lookup"><span data-stu-id="07950-112">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="07950-113">例如，若要为 中的每个事件创建模板 `mgt-agenda` ，请使用 `event` 数据类型，如下所示。</span><span class="sxs-lookup"><span data-stu-id="07950-113">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="07950-114">如果 `data-type` 未指定，则整个组件将替换为模板。</span><span class="sxs-lookup"><span data-stu-id="07950-114">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="07950-115">您还可以用于 `data-type="default"` 同一目的。</span><span class="sxs-lookup"><span data-stu-id="07950-115">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="07950-116">绑定数据</span><span class="sxs-lookup"><span data-stu-id="07950-116">Binding data</span></span>

<span data-ttu-id="07950-117">许多模板允许绑定作为数据上下文传递给模板的数据。</span><span class="sxs-lookup"><span data-stu-id="07950-117">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="07950-118">例如， `event` 组件中的模板 `mgt-agenda` 传递 `{event}` 可以直接在模板中使用的对象。</span><span class="sxs-lookup"><span data-stu-id="07950-118">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="07950-119">若要展开表达式（如 `event.subject` ），请使用双花括号。</span><span class="sxs-lookup"><span data-stu-id="07950-119">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="07950-120">此格式还可在属性内使用：</span><span class="sxs-lookup"><span data-stu-id="07950-120">This format can also be used inside attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="07950-121">**注意：** 还可以展开 或 等对象 `{{event}}` `{{this}}` ，它们将呈现为 JSON 字符串。</span><span class="sxs-lookup"><span data-stu-id="07950-121">**Note:** You can also expand objects such as `{{event}}` or `{{this}}` and they will render as JSON strings.</span></span> <span data-ttu-id="07950-122">在开发模板时，这非常有用。</span><span class="sxs-lookup"><span data-stu-id="07950-122">This can be useful when you're developing the templates.</span></span>

### <a name="change-binding-syntax"></a><span data-ttu-id="07950-123">更改绑定语法</span><span class="sxs-lookup"><span data-stu-id="07950-123">Change binding syntax</span></span>

<span data-ttu-id="07950-124">默认情况下，若要展开表达式，请使用双花括号 `{{expression}}` () 。</span><span class="sxs-lookup"><span data-stu-id="07950-124">By default, to expand an expression, you use double curly brackets ( `{{expression}}` ).</span></span> <span data-ttu-id="07950-125">但是，您可以更改已使用双括号语法的环境的此语法。</span><span class="sxs-lookup"><span data-stu-id="07950-125">However, you can change this syntax for environments where the double curly bracket syntax is already used.</span></span> <span data-ttu-id="07950-126">例如，以下示例使用双方括号 `[[expression]]` () 。</span><span class="sxs-lookup"><span data-stu-id="07950-126">For example, the following example uses double square brackets ( `[[expression]]` ).</span></span>

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a><span data-ttu-id="07950-127">数据上下文帮助程序属性</span><span class="sxs-lookup"><span data-stu-id="07950-127">Data context helper properties</span></span>

<span data-ttu-id="07950-128">以下属性还可与模板中的数据上下文对象一同使用。</span><span class="sxs-lookup"><span data-stu-id="07950-128">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="07950-129">属性</span><span class="sxs-lookup"><span data-stu-id="07950-129">Property</span></span> | <span data-ttu-id="07950-130">说明</span><span class="sxs-lookup"><span data-stu-id="07950-130">Description</span></span>                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="07950-131">$index</span><span class="sxs-lookup"><span data-stu-id="07950-131">$index</span></span>   | <span data-ttu-id="07950-132">使用 循环时呈现的项目的数字索引 `data-for` 。</span><span class="sxs-lookup"><span data-stu-id="07950-132">Numerical index of item being rendered while being looped with `data-for`.</span></span>                                     |
| <span data-ttu-id="07950-133">$parent</span><span class="sxs-lookup"><span data-stu-id="07950-133">$parent</span></span>  | <span data-ttu-id="07950-134">如果模板呈现在另一个模板内，则此属性允许您访问父数据上下文。</span><span class="sxs-lookup"><span data-stu-id="07950-134">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="07950-135">以下示例演示如何在 `$index` data-for 循环中使用 属性。</span><span class="sxs-lookup"><span data-stu-id="07950-135">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

### <a name="this"></a><span data-ttu-id="07950-136">{{this}}</span><span class="sxs-lookup"><span data-stu-id="07950-136">{{this}}</span></span>

<span data-ttu-id="07950-137">为了帮助调试数据上下文，可以在 `this` 绑定表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="07950-137">To help debug the data context, you can use `this` in your binding expressions.</span></span> <span data-ttu-id="07950-138">最简单的表单是在模板 `{{this}}` 中的任何位置添加。</span><span class="sxs-lookup"><span data-stu-id="07950-138">The simplest form is to add `{{this}}` anywhere in your template.</span></span>

```html
<template data-type="event">
  <div>
    {{this}}
  </div>
</template>
```

<span data-ttu-id="07950-139">由于可以在绑定表达式中使用 JavaScript，因此还可以访问对象，该对象允许你在模板中使用 [`console`](https://developer.mozilla.org/docs/Web/API/Console) `console.log(this)` (或其他任何 API `console`) 。</span><span class="sxs-lookup"><span data-stu-id="07950-139">Because you can use JavaScript in your binding expressions, you also have access to the [`console`](https://developer.mozilla.org/docs/Web/API/Console) object which allows you to use `console.log(this)` (or any other `console` API) in your templates.</span></span>

```html
<template data-type="event">
  <div>
    {{console.log(this)}}
  </div>
</template>
```

## <a name="conditional-rendering"></a><span data-ttu-id="07950-140">条件呈现</span><span class="sxs-lookup"><span data-stu-id="07950-140">Conditional rendering</span></span>

<span data-ttu-id="07950-141">您可能只希望根据数据上下文在条件为 true 或 false 时呈现元素。</span><span class="sxs-lookup"><span data-stu-id="07950-141">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="07950-142">和 `data-if` `data-else` 属性可以计算表达式，并且仅在 true 或 false 时呈现。</span><span class="sxs-lookup"><span data-stu-id="07950-142">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="07950-143">循环</span><span class="sxs-lookup"><span data-stu-id="07950-143">Looping</span></span>

<span data-ttu-id="07950-144">在某些情况下，数据上下文对象包含循环，并且你需要循环访问数据。</span><span class="sxs-lookup"><span data-stu-id="07950-144">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="07950-145">对于此方案，请使用 `data-for` 属性。</span><span class="sxs-lookup"><span data-stu-id="07950-145">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a><span data-ttu-id="07950-146">模板上下文</span><span class="sxs-lookup"><span data-stu-id="07950-146">Template context</span></span>

<span data-ttu-id="07950-147">在需要转换绑定中数据、绑定到事件或仅使用模板绑定中的外部数据的方案中，模板支持绑定到外部数据上下文。</span><span class="sxs-lookup"><span data-stu-id="07950-147">In scenarios where you need to convert data in your bindings, bind to events, or just use external data in your templates bindings, the templates support binding to external data context.</span></span> <span data-ttu-id="07950-148">可以通过两种方式添加其他模板上下文：</span><span class="sxs-lookup"><span data-stu-id="07950-148">You can add additional template context in two ways:</span></span>

1. <span data-ttu-id="07950-149">直接在组件上。</span><span class="sxs-lookup"><span data-stu-id="07950-149">Directly on the component.</span></span>

    <span data-ttu-id="07950-150">每个组件都定义 属性，可用于向组件中的任意 `templateContext` 模板传递其他数据。</span><span class="sxs-lookup"><span data-stu-id="07950-150">Each component defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span>

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    <span data-ttu-id="07950-151">对象中的 `templateContext` 属性现在可用于模板中的绑定表达式。</span><span class="sxs-lookup"><span data-stu-id="07950-151">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

2. <span data-ttu-id="07950-152">针对所有组件的全局性。</span><span class="sxs-lookup"><span data-stu-id="07950-152">Globally for all components.</span></span>

    <span data-ttu-id="07950-153">`TemplateHelper`类公开 `globalContext` 对象以添加应在全局上可用于所有组件的数据或函数。</span><span class="sxs-lookup"><span data-stu-id="07950-153">The `TemplateHelper` class exposes the `globalContext` object to add data or functions that should be globally available for all components.</span></span>

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a><span data-ttu-id="07950-154">转换器</span><span class="sxs-lookup"><span data-stu-id="07950-154">Converters</span></span>

<span data-ttu-id="07950-155">在许多情况下，您可能希望先转换数据，然后再将数据呈现在模板中。</span><span class="sxs-lookup"><span data-stu-id="07950-155">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="07950-156">例如，您可能希望在呈现日期之前正确设置日期的格式。</span><span class="sxs-lookup"><span data-stu-id="07950-156">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="07950-157">在这些情况下，您可能需要使用模板转换器。</span><span class="sxs-lookup"><span data-stu-id="07950-157">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="07950-158">若要使用模板转换器，首先需要定义一个将执行转换的函数。</span><span class="sxs-lookup"><span data-stu-id="07950-158">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="07950-159">例如，您可以定义一个函数以将事件对象转换为格式化的时区。</span><span class="sxs-lookup"><span data-stu-id="07950-159">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="07950-160">若要在模板中使用此转换器，请使用它，就像在代码隐藏部分使用函数一样。</span><span class="sxs-lookup"><span data-stu-id="07950-160">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="07950-161">事件或属性绑定</span><span class="sxs-lookup"><span data-stu-id="07950-161">Event or property binding</span></span>

<span data-ttu-id="07950-162">`data-props`通过 属性，您可以直接在模板中添加事件侦听器或设置属性值。</span><span class="sxs-lookup"><span data-stu-id="07950-162">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span>

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="07950-163">data-props 接受您可能要设置的每个属性或事件处理程序的逗号分隔字符串。</span><span class="sxs-lookup"><span data-stu-id="07950-163">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span>

<span data-ttu-id="07950-164">若要添加事件处理程序，请以 作为事件名称的前缀 `@` 。</span><span class="sxs-lookup"><span data-stu-id="07950-164">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="07950-165">事件处理程序将需要在 元素中 `templateContext` 可用。</span><span class="sxs-lookup"><span data-stu-id="07950-165">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="07950-166">事件参数、数据上下文和模板的根元素作为参数传递给事件处理程序。</span><span class="sxs-lookup"><span data-stu-id="07950-166">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="07950-167">模板呈现事件</span><span class="sxs-lookup"><span data-stu-id="07950-167">Template rendered event</span></span>

<span data-ttu-id="07950-168">在某些情况下，您可能希望获取对已呈现元素的引用。</span><span class="sxs-lookup"><span data-stu-id="07950-168">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="07950-169">如果希望自己处理内容的呈现，或者要修改呈现的元素，这将非常有用。</span><span class="sxs-lookup"><span data-stu-id="07950-169">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="07950-170">在此方案中，可以使用 `templateRendered` 事件，该事件在模板呈现后触发。</span><span class="sxs-lookup"><span data-stu-id="07950-170">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="07950-171">事件详细信息将包含对要呈现的元素的引用、数据上下文对象和模板的类型。</span><span class="sxs-lookup"><span data-stu-id="07950-171">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="07950-172">样式设置</span><span class="sxs-lookup"><span data-stu-id="07950-172">Styling</span></span>

<span data-ttu-id="07950-173">模板可以通过 CSS 正常设置样式，因为它们呈现在阴影 dom 之外。</span><span class="sxs-lookup"><span data-stu-id="07950-173">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
