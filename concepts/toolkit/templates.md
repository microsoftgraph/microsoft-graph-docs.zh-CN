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
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="6ba93-103">Microsoft Graph 工具包中的模板</span><span class="sxs-lookup"><span data-stu-id="6ba93-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="6ba93-104">使用自定义模板修改组件的内容。</span><span class="sxs-lookup"><span data-stu-id="6ba93-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="6ba93-105">所有 web 组件都支持基于元素的`<template>`模板。</span><span class="sxs-lookup"><span data-stu-id="6ba93-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="6ba93-106">例如，若要覆盖组件的模板，请在组件中`<template>`添加元素。</span><span class="sxs-lookup"><span data-stu-id="6ba93-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

## <a name="data-type"></a><span data-ttu-id="6ba93-107">数据类型</span><span class="sxs-lookup"><span data-stu-id="6ba93-107">Data-type</span></span>

<span data-ttu-id="6ba93-108">每个组件都可以具有多个可模板化的部件。</span><span class="sxs-lookup"><span data-stu-id="6ba93-108">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="6ba93-109">例如，在`mgt-agenda`组件中，可以对单个事件、各个节标题、加载视图、无数据视图等进行模板。</span><span class="sxs-lookup"><span data-stu-id="6ba93-109">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="6ba93-110">若要指示模板，请使用`data-type`模板上的属性。</span><span class="sxs-lookup"><span data-stu-id="6ba93-110">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="6ba93-111">例如，若要在中为每个`mgt-agenda`事件提供模板`event` ，请使用数据类型，如下所示。</span><span class="sxs-lookup"><span data-stu-id="6ba93-111">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="6ba93-112">如果指定`data-type`为 "否"，则整个组件将替换为模板。</span><span class="sxs-lookup"><span data-stu-id="6ba93-112">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="6ba93-113">您也可以使用`data-type="default"`相同的目的。</span><span class="sxs-lookup"><span data-stu-id="6ba93-113">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="6ba93-114">绑定数据</span><span class="sxs-lookup"><span data-stu-id="6ba93-114">Binding data</span></span>

<span data-ttu-id="6ba93-115">许多模板允许将作为数据上下文传递给模板的数据绑定。</span><span class="sxs-lookup"><span data-stu-id="6ba93-115">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="6ba93-116">例如， `event` `mgt-agenda`组件中的模板传递可直接在`{event}`模板中使用的对象。</span><span class="sxs-lookup"><span data-stu-id="6ba93-116">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="6ba93-117">若要展开表达式（例如`event.subject`），请使用双花括号。</span><span class="sxs-lookup"><span data-stu-id="6ba93-117">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="6ba93-118">此外，还可以在属性内使用此格式：</span><span class="sxs-lookup"><span data-stu-id="6ba93-118">This format can also be used inside of attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="6ba93-119">**注意：** 您还可以展开诸如等对象`{{event}}` ，它们将呈现为 JSON 字符串。</span><span class="sxs-lookup"><span data-stu-id="6ba93-119">**Note:** You can also expand objects such as `{{event}}` and they will render as JSON strings.</span></span> <span data-ttu-id="6ba93-120">这在开发模板时可能很有用。</span><span class="sxs-lookup"><span data-stu-id="6ba93-120">This can be useful when you're developing the templates.</span></span>

## <a name="data-context-helper-properties"></a><span data-ttu-id="6ba93-121">数据上下文帮助程序属性</span><span class="sxs-lookup"><span data-stu-id="6ba93-121">Data context helper properties</span></span>

<span data-ttu-id="6ba93-122">下列属性也可以与模板中的数据上下文对象一起使用。</span><span class="sxs-lookup"><span data-stu-id="6ba93-122">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="6ba93-123">属性</span><span class="sxs-lookup"><span data-stu-id="6ba93-123">Property</span></span> |  <span data-ttu-id="6ba93-124">说明</span><span class="sxs-lookup"><span data-stu-id="6ba93-124">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="6ba93-125">$index</span><span class="sxs-lookup"><span data-stu-id="6ba93-125">$index</span></span> | <span data-ttu-id="6ba93-126">循环使用`data-for`时呈现的项的数字索引。</span><span class="sxs-lookup"><span data-stu-id="6ba93-126">Numerical index of item being rendered while being looped with `data-for`.</span></span> |
| <span data-ttu-id="6ba93-127">$parent</span><span class="sxs-lookup"><span data-stu-id="6ba93-127">$parent</span></span> | <span data-ttu-id="6ba93-128">如果模板呈现在另一个模板中，则此属性允许您访问父数据上下文。</span><span class="sxs-lookup"><span data-stu-id="6ba93-128">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="6ba93-129">下面的示例演示如何在数据 for `$index`循环中使用该属性。</span><span class="sxs-lookup"><span data-stu-id="6ba93-129">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

## <a name="conditional-rendering"></a><span data-ttu-id="6ba93-130">条件呈现</span><span class="sxs-lookup"><span data-stu-id="6ba93-130">Conditional rendering</span></span>

<span data-ttu-id="6ba93-131">您可能只希望在条件为 true 或 false 时呈现基于数据上下文的元素。</span><span class="sxs-lookup"><span data-stu-id="6ba93-131">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="6ba93-132">`data-if`和`data-else`属性可以计算表达式，并且只有在 true 或 false 时才会呈现。</span><span class="sxs-lookup"><span data-stu-id="6ba93-132">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="6ba93-133">循环</span><span class="sxs-lookup"><span data-stu-id="6ba93-133">Looping</span></span>

<span data-ttu-id="6ba93-134">在某些情况下，数据上下文对象包含循环，您需要对数据循环。</span><span class="sxs-lookup"><span data-stu-id="6ba93-134">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="6ba93-135">对于此方案，请使用`data-for`属性。</span><span class="sxs-lookup"><span data-stu-id="6ba93-135">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="templatecontext"></a><span data-ttu-id="6ba93-136">TemplateContext</span><span class="sxs-lookup"><span data-stu-id="6ba93-136">TemplateContext</span></span>

<span data-ttu-id="6ba93-137">Microsoft Graph 工具包中的每个组件都`templateContext`定义了属性，可使用该属性将其他数据传递到组件中的任何模板。</span><span class="sxs-lookup"><span data-stu-id="6ba93-137">Each component in the Microsoft Graph Toolkit defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span> 

```ts
document.querySelector('mgt-agenda').templateContext = {

  someObject: {},
  formatDate: (date: Date) => { /* format date and return */ },
  someEventHandler: (e) => { /* handleEvent */  }

}
```

<span data-ttu-id="6ba93-138">此时，该`templateContext`对象中的属性将可用于模板中的绑定表达式。</span><span class="sxs-lookup"><span data-stu-id="6ba93-138">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

<span data-ttu-id="6ba93-139">这在很多情况下都很有用，例如在绑定中转换数据或绑定到事件。</span><span class="sxs-lookup"><span data-stu-id="6ba93-139">This can be useful in many scenarios, such as converting data in your bindings, or binding to events.</span></span> 

### <a name="converters"></a><span data-ttu-id="6ba93-140">转换器</span><span class="sxs-lookup"><span data-stu-id="6ba93-140">Converters</span></span>

<span data-ttu-id="6ba93-141">在很多情况下，您可能需要在将数据呈现在模板中之前对数据进行转换。</span><span class="sxs-lookup"><span data-stu-id="6ba93-141">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="6ba93-142">例如，您可能希望在呈现日期之前正确设置日期格式。</span><span class="sxs-lookup"><span data-stu-id="6ba93-142">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="6ba93-143">在这些情况下，您可能需要使用模板转换器。</span><span class="sxs-lookup"><span data-stu-id="6ba93-143">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="6ba93-144">若要使用模板转换器，首先需要定义将执行转换的函数。</span><span class="sxs-lookup"><span data-stu-id="6ba93-144">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="6ba93-145">例如，您可以定义一个函数来将事件对象转换为格式化的时间范围。</span><span class="sxs-lookup"><span data-stu-id="6ba93-145">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="6ba93-146">若要在模板中使用转换器，请使用它，就像在代码隐藏中使用函数一样。</span><span class="sxs-lookup"><span data-stu-id="6ba93-146">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="6ba93-147">事件或属性绑定</span><span class="sxs-lookup"><span data-stu-id="6ba93-147">Event or property binding</span></span>

<span data-ttu-id="6ba93-148">`data-props`属性允许您添加事件侦听器或直接在模板中设置属性值。</span><span class="sxs-lookup"><span data-stu-id="6ba93-148">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span> 

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="6ba93-149">对于您可能想要设置的每个属性或事件处理程序，数据属性接受以逗号分隔的字符串。</span><span class="sxs-lookup"><span data-stu-id="6ba93-149">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span> 

<span data-ttu-id="6ba93-150">若要添加事件处理程序，请为事件的名称加`@`上前缀。</span><span class="sxs-lookup"><span data-stu-id="6ba93-150">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="6ba93-151">事件处理程序将需要在元素`templateContext`的中可用。</span><span class="sxs-lookup"><span data-stu-id="6ba93-151">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="6ba93-152">将模板的事件参数、数据上下文和根元素作为参数传递给事件处理程序。</span><span class="sxs-lookup"><span data-stu-id="6ba93-152">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="6ba93-153">模板呈现事件</span><span class="sxs-lookup"><span data-stu-id="6ba93-153">Template rendered event</span></span>

<span data-ttu-id="6ba93-154">在某些情况下，您可能需要获取对呈现的元素的引用。</span><span class="sxs-lookup"><span data-stu-id="6ba93-154">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="6ba93-155">如果您希望自己处理内容的呈现，或者想要修改呈现的元素，这会非常有用。</span><span class="sxs-lookup"><span data-stu-id="6ba93-155">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="6ba93-156">在这种情况下，您可以`templateRendered`使用事件，该事件将在呈现模板后触发。</span><span class="sxs-lookup"><span data-stu-id="6ba93-156">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="6ba93-157">事件详细信息将包含对要呈现的元素、数据上下文对象和模板类型的引用。</span><span class="sxs-lookup"><span data-stu-id="6ba93-157">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="6ba93-158">样式</span><span class="sxs-lookup"><span data-stu-id="6ba93-158">Styling</span></span>

<span data-ttu-id="6ba93-159">可以通过 CSS 对模板进行样式化，因为它们呈现在阴影 dom 外部。</span><span class="sxs-lookup"><span data-stu-id="6ba93-159">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
