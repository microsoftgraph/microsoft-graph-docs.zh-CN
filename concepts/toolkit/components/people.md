---
title: Microsoft Graph 工具包中的 "人员" 组件
description: 您可以使用`mgt-people` web 组件显示一组用户或联系人, 方法是使用其照片或缩写。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: fcc44262f807d3f10f42e8af8e476975ad262cda
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242978"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8f0a6-103">Microsoft Graph 工具包中的 "人员" 组件</span><span class="sxs-lookup"><span data-stu-id="8f0a6-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8f0a6-104">您可以使用`mgt-people` web 组件显示一组用户或联系人, 方法是使用其照片或缩写。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="8f0a6-105">默认情况下, 它将显示登录用户最常使用的联系人。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="8f0a6-106">此组件使用多个 "控制[人员](./person.md)" 控件, 但它可以绑定到一组人员描述符。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="8f0a6-107">如果要显示的人员多于`show-max`该值, 则将添加一个数字以指示其他联系人的数量。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="8f0a6-108">示例</span><span class="sxs-lookup"><span data-stu-id="8f0a6-108">Example</span></span>

[<span data-ttu-id="8f0a6-109">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="8f0a6-109">jsfiddle example</span></span>](https://jsfiddle.net/metulev/az6pqy2r/)

```html
<mgt-people></mgt-people>
```

![组织-人员](./images/mgt-people.png)

## <a name="properties"></a><span data-ttu-id="8f0a6-111">属性</span><span class="sxs-lookup"><span data-stu-id="8f0a6-111">Properties</span></span>

<span data-ttu-id="8f0a6-112">默认情况下, `mgt-people`组件使用`personType/class eq 'Person'`筛选器从`/me/people`终结点提取事件, 以显示经常联系的用户。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-112">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="8f0a6-113">您可以使用多个属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-113">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="8f0a6-114">属性</span><span class="sxs-lookup"><span data-stu-id="8f0a6-114">Property</span></span> | <span data-ttu-id="8f0a6-115">属性</span><span class="sxs-lookup"><span data-stu-id="8f0a6-115">Attribute</span></span> | <span data-ttu-id="8f0a6-116">说明</span><span class="sxs-lookup"><span data-stu-id="8f0a6-116">Description</span></span> |
| --- | --- | --- |
| `showMax` | `show-max` | <span data-ttu-id="8f0a6-117">指示要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-117">Indicate the maximum number of people to show.</span></span> <span data-ttu-id="8f0a6-118">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-118">Default value is 3.</span></span> |
| `people` | `people` | <span data-ttu-id="8f0a6-119">获取或设置组件呈现的人员列表的人员数组。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-119">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="8f0a6-120">使用此属性可访问组件加载的人员。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-120">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="8f0a6-121">设置此值可加载自己的人员。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-121">Set this value to load your own people.</span></span> |

<span data-ttu-id="8f0a6-122">下面的示例设置要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-122">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="8f0a6-123">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="8f0a6-123">CSS custom properties</span></span>

<span data-ttu-id="8f0a6-124">`mgt-people`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-124">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="8f0a6-125">模板</span><span class="sxs-lookup"><span data-stu-id="8f0a6-125">Templates</span></span>

<span data-ttu-id="8f0a6-126">支持多个[模板](../templates.md), 这些模板可用于替换组件的某些部分。 `mgt-people`</span><span class="sxs-lookup"><span data-stu-id="8f0a6-126">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="8f0a6-127">若要指定模板, 请在`<template>`组件内添加一个元素, 并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-127">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="8f0a6-128">数据类型</span><span class="sxs-lookup"><span data-stu-id="8f0a6-128">Data type</span></span> | <span data-ttu-id="8f0a6-129">数据上下文</span><span class="sxs-lookup"><span data-stu-id="8f0a6-129">Data context</span></span> | <span data-ttu-id="8f0a6-130">说明</span><span class="sxs-lookup"><span data-stu-id="8f0a6-130">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="8f0a6-131">`people`: person 对象列表</span><span class="sxs-lookup"><span data-stu-id="8f0a6-131">`people`: list of person objects</span></span> | <span data-ttu-id="8f0a6-132">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-132">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="8f0a6-133">`person`: person 对象</span><span class="sxs-lookup"><span data-stu-id="8f0a6-133">`person`: person object</span></span> | <span data-ttu-id="8f0a6-134">用于呈现每个人的模板。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-134">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="8f0a6-135">`people`: person 对象列表</span><span class="sxs-lookup"><span data-stu-id="8f0a6-135">`people`: list of person objects</span></span> <br> <span data-ttu-id="8f0a6-136">`max`: 显示的人员的数量</span><span class="sxs-lookup"><span data-stu-id="8f0a6-136">`max`: number of shown people</span></span> <br> <span data-ttu-id="8f0a6-137">`extra`: 额外人员数</span><span class="sxs-lookup"><span data-stu-id="8f0a6-137">`extra`: number of extra people</span></span> | <span data-ttu-id="8f0a6-138">用于将数字呈现在人员列表右侧的最大值之后的模板。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-138">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="8f0a6-139">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="8f0a6-139">No data context is passed</span></span> | <span data-ttu-id="8f0a6-140">没有人可用时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-140">The template used when no people are available.</span></span> |

<span data-ttu-id="8f0a6-141">下面的示例演示如何使用`person`模板。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-141">The following examples shows how to use the `person` template.</span></span>

```html
<mgt-people>
  <template>
    <ul><li data-for="person in people">
      <mgt-person person-query="{{ person.userPrincipalName }}"></mgt-person>
      <h3>{{ person.displayName }}</h3>
      <p>{{ person.jobTitle }}</p>
      <p>{{ person.department }}</p>
    </li></ul>
  </template>
</mgt-people>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8f0a6-142">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="8f0a6-142">Microsoft Graph permissions</span></span>

<span data-ttu-id="8f0a6-143">此组件使用以下 Microsoft Graph Api 和权限:</span><span class="sxs-lookup"><span data-stu-id="8f0a6-143">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="8f0a6-144">资源</span><span class="sxs-lookup"><span data-stu-id="8f0a6-144">Resource</span></span> | <span data-ttu-id="8f0a6-145">权限/范围</span><span class="sxs-lookup"><span data-stu-id="8f0a6-145">Permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="8f0a6-146">/me/people</span><span class="sxs-lookup"><span data-stu-id="8f0a6-146">/me/people</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="8f0a6-147">身份验证</span><span class="sxs-lookup"><span data-stu-id="8f0a6-147">Authentication</span></span>

<span data-ttu-id="8f0a6-148">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="8f0a6-148">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
