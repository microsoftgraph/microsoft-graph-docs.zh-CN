---
title: Microsoft Graph 工具包中的模板
description: 使用自定义模板修改组件的内容。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9ef4b9422d84886fa4df76618b6cdf14def2378
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275708"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="92693-103">Microsoft Graph 工具包中的模板</span><span class="sxs-lookup"><span data-stu-id="92693-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="92693-104">使用自定义模板修改组件的内容。</span><span class="sxs-lookup"><span data-stu-id="92693-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="92693-105">所有 web 组件都支持基于元素的`<template>`模板。</span><span class="sxs-lookup"><span data-stu-id="92693-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="92693-106">例如，若要覆盖组件的模板，请在组件中`<template>`添加元素。</span><span class="sxs-lookup"><span data-stu-id="92693-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

## <a name="data-type"></a><span data-ttu-id="92693-107">数据类型</span><span class="sxs-lookup"><span data-stu-id="92693-107">Data-type</span></span>

<span data-ttu-id="92693-108">每个组件都可以具有多个可模板化的部件。</span><span class="sxs-lookup"><span data-stu-id="92693-108">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="92693-109">例如，在`mgt-agenda`组件中，可以对单个事件、各个节标题、加载视图、无数据视图等进行模板。</span><span class="sxs-lookup"><span data-stu-id="92693-109">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="92693-110">若要指示模板，请使用`data-type`模板上的属性。</span><span class="sxs-lookup"><span data-stu-id="92693-110">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="92693-111">例如，若要在中为每个`mgt-agenda`事件提供模板`event` ，请使用数据类型，如下所示。</span><span class="sxs-lookup"><span data-stu-id="92693-111">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="92693-112">如果指定`data-type`为 "否"，则整个组件将替换为模板。</span><span class="sxs-lookup"><span data-stu-id="92693-112">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="92693-113">您也可以使用`data-type="default"`相同的目的。</span><span class="sxs-lookup"><span data-stu-id="92693-113">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="92693-114">绑定数据</span><span class="sxs-lookup"><span data-stu-id="92693-114">Binding data</span></span>

<span data-ttu-id="92693-115">许多模板允许将作为数据上下文传递给模板的数据绑定。</span><span class="sxs-lookup"><span data-stu-id="92693-115">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="92693-116">例如， `event` `mgt-agenda`组件中的模板传递可直接在`{event}`模板中使用的对象。</span><span class="sxs-lookup"><span data-stu-id="92693-116">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="92693-117">若要展开表达式（例如`event.subject`），请使用双花括号。</span><span class="sxs-lookup"><span data-stu-id="92693-117">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="92693-118">此外，还可以在属性内使用此格式：</span><span class="sxs-lookup"><span data-stu-id="92693-118">This format can also be used inside of attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="92693-119">**注意：** 您还可以展开诸如等对象`{{event}}` ，它们将呈现为 JSON 字符串。</span><span class="sxs-lookup"><span data-stu-id="92693-119">**Note:** You can also expand objects such as `{{event}}` and they will render as JSON strings.</span></span> <span data-ttu-id="92693-120">这在开发模板时可能很有用。</span><span class="sxs-lookup"><span data-stu-id="92693-120">This can be useful when you're developing the templates.</span></span>

## <a name="conditional-rendering"></a><span data-ttu-id="92693-121">条件呈现</span><span class="sxs-lookup"><span data-stu-id="92693-121">Conditional rendering</span></span>

<span data-ttu-id="92693-122">您可能只希望在条件为 true 或 false 时呈现基于数据上下文的元素。</span><span class="sxs-lookup"><span data-stu-id="92693-122">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="92693-123">`data-if`和`data-else`属性可以计算表达式，并且只有在 true 或 false 时才会呈现。</span><span class="sxs-lookup"><span data-stu-id="92693-123">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="92693-124">循环</span><span class="sxs-lookup"><span data-stu-id="92693-124">Looping</span></span>

<span data-ttu-id="92693-125">在某些情况下，数据上下文对象包含循环，您需要对数据循环。</span><span class="sxs-lookup"><span data-stu-id="92693-125">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="92693-126">对于此方案，请使用`data-for`属性。</span><span class="sxs-lookup"><span data-stu-id="92693-126">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="converters"></a><span data-ttu-id="92693-127">转换器</span><span class="sxs-lookup"><span data-stu-id="92693-127">Converters</span></span>

<span data-ttu-id="92693-128">在很多情况下，您可能需要在将数据呈现在模板中之前对数据进行转换。</span><span class="sxs-lookup"><span data-stu-id="92693-128">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="92693-129">例如，您可能希望在呈现日期之前正确设置日期格式。</span><span class="sxs-lookup"><span data-stu-id="92693-129">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="92693-130">在这些情况下，您可能需要使用模板转换器。</span><span class="sxs-lookup"><span data-stu-id="92693-130">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="92693-131">若要使用模板转换器，首先需要定义将执行转换的函数。</span><span class="sxs-lookup"><span data-stu-id="92693-131">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="92693-132">例如，您可以定义一个函数来设置日期格式。</span><span class="sxs-lookup"><span data-stu-id="92693-132">For example, you might define a function to format a date.</span></span>

```ts
getTimeRange(event) {
  // TODO: format a string from the event object as you wish
  // timeRange = ...

  return timeRange;
}
```

<span data-ttu-id="92693-133">然后，在元素上定义新的转换器并将其命名为 "匹配"。</span><span class="sxs-lookup"><span data-stu-id="92693-133">Then define a new converter on the element and name it as you see fit.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.templateConverters["myConverter"] = getTimeRange;
```

<span data-ttu-id="92693-134">若要在模板中使用转换器，请使用三向花括号。</span><span class="sxs-lookup"><span data-stu-id="92693-134">To use the converter in your template, use the triple curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{{ myConverter(event) }}}</div>
</template>
```

<span data-ttu-id="92693-135">您还可以使用内置函数，而无需定义模板转换器。</span><span class="sxs-lookup"><span data-stu-id="92693-135">You can also use built-in functions without defining template converter.</span></span>

```html
<template data-type="event">
  <div>{{{ event.subject.toUpperCase() }}}</div>
</template>
```

## <a name="template-rendered-event"></a><span data-ttu-id="92693-136">模板呈现事件</span><span class="sxs-lookup"><span data-stu-id="92693-136">Template Rendered Event</span></span>

<span data-ttu-id="92693-137">在某些情况下，您可能需要获取对呈现的元素的引用。</span><span class="sxs-lookup"><span data-stu-id="92693-137">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="92693-138">这在向模板中的元素添加事件侦听器时非常有用。</span><span class="sxs-lookup"><span data-stu-id="92693-138">This can be useful for adding event listeners to elements in the template.</span></span> <span data-ttu-id="92693-139">在这种情况下，可以使用`templateRendered`事件。</span><span class="sxs-lookup"><span data-stu-id="92693-139">In this scenario, you might use the `templateRendered` event.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="92693-140">事件详细信息将包含对要呈现的元素、数据上下文对象和模板类型的引用。</span><span class="sxs-lookup"><span data-stu-id="92693-140">The event details will contain reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

```ts
agenda.addEventListener('templateRendered', (e) => { 
  let templateType = e.detail.templateType;
  let dataContext = e.detail.context;
  let element = e.detail.element;

  if (type === 'event') {
    element.querySelector('.some-button').addEventListener('click', () => {});
  }
});
```

## <a name="styling"></a><span data-ttu-id="92693-141">样式</span><span class="sxs-lookup"><span data-stu-id="92693-141">Styling</span></span>

<span data-ttu-id="92693-142">可以通过 CSS 对模板进行样式化，因为它们呈现在阴影 dom 外部。</span><span class="sxs-lookup"><span data-stu-id="92693-142">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
