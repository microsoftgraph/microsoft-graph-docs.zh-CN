---
title: Microsoft Graph 工具包中的模板
description: 使用自定义模板修改组件的内容。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: f0648d0ac1348fbadad6cebe8a022f9445fcf1e3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242957"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="44d7b-103">Microsoft Graph 工具包中的模板</span><span class="sxs-lookup"><span data-stu-id="44d7b-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="44d7b-104">使用自定义模板修改组件的内容。</span><span class="sxs-lookup"><span data-stu-id="44d7b-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="44d7b-105">所有 web 组件都支持基于元素的`<template>`模板。</span><span class="sxs-lookup"><span data-stu-id="44d7b-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="44d7b-106">例如, 若要覆盖组件的模板, 请在组件中`<template>`添加元素。</span><span class="sxs-lookup"><span data-stu-id="44d7b-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

<span data-ttu-id="44d7b-107">以下模板功能受支持:</span><span class="sxs-lookup"><span data-stu-id="44d7b-107">The following template features are supported:</span></span>

- <span data-ttu-id="44d7b-108">使用双花括号 (`{{expression}}`) 展开表达式。</span><span class="sxs-lookup"><span data-stu-id="44d7b-108">Use the double curly brackets (`{{expression}}`) to expand an expression.</span></span> <span data-ttu-id="44d7b-109">在上面的示例中, `<mgt-person>`传递一个`person`可在模板中使用的对象。</span><span class="sxs-lookup"><span data-stu-id="44d7b-109">In the previous example, the `<mgt-person>` passes a `person` object that you can use in the template.</span></span>
- <span data-ttu-id="44d7b-110">使用`data-if`和`data-else`属性进行条件呈现。</span><span class="sxs-lookup"><span data-stu-id="44d7b-110">Use the `data-if` and `data-else` attributes for conditional rendering.</span></span> <span data-ttu-id="44d7b-111">支持`event.attendees.length > 2`的条件表达式 (如支持)。</span><span class="sxs-lookup"><span data-stu-id="44d7b-111">Conditional expressions such as `event.attendees.length > 2` are supported.</span></span>
- <span data-ttu-id="44d7b-112">`data-for`使用重复元素。</span><span class="sxs-lookup"><span data-stu-id="44d7b-112">Use the `data-for` to repeat an element.</span></span>
- <span data-ttu-id="44d7b-113">`data-type`使用指定要模板的组件部分。</span><span class="sxs-lookup"><span data-stu-id="44d7b-113">Use the `data-type` to specify what part of the component to template.</span></span> <span data-ttu-id="44d7b-114">如果不指定类型, 则会将该模板应用于整个组件。</span><span class="sxs-lookup"><span data-stu-id="44d7b-114">Not specifying the type will apply the template to the entire component.</span></span>

<span data-ttu-id="44d7b-115">每个组件都记录`data-type`受支持的值和向下传递给每个模板的数据上下文。</span><span class="sxs-lookup"><span data-stu-id="44d7b-115">Each component documents the supported `data-type` values and what data context is passed down to each template.</span></span>

<span data-ttu-id="44d7b-116">模板的样式可以像在阴影 dom 外部呈现的那样正常显示。</span><span class="sxs-lookup"><span data-stu-id="44d7b-116">The templates can be styled normally as they are rendered outside of the shadow dom.</span></span>
