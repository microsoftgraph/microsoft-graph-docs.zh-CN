---
title: Microsoft Graph 工具包中的 "人员" 组件
description: 您可以使用`mgt-people` web 组件显示一组用户或联系人，方法是使用其照片或缩写。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 34b7877b16d7f97d201e7bd96e1378c1e542bbcf
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144294"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="f9e04-103">Microsoft Graph 工具包中的 "人员" 组件</span><span class="sxs-lookup"><span data-stu-id="f9e04-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="f9e04-104">您可以使用`mgt-people` web 组件显示一组用户或联系人，方法是使用其照片或缩写。</span><span class="sxs-lookup"><span data-stu-id="f9e04-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="f9e04-105">默认情况下，它将显示登录用户最常使用的联系人。</span><span class="sxs-lookup"><span data-stu-id="f9e04-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="f9e04-106">此组件使用多个 "控制[人员](./person.md)" 控件，但它可以绑定到一组人员描述符。</span><span class="sxs-lookup"><span data-stu-id="f9e04-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="f9e04-107">如果要显示的人员多于`show-max`该值，则将添加一个数字以指示其他联系人的数量。</span><span class="sxs-lookup"><span data-stu-id="f9e04-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="f9e04-108">示例</span><span class="sxs-lookup"><span data-stu-id="f9e04-108">Example</span></span>

<span data-ttu-id="f9e04-109">下面的示例展示了使用`mgt-people`组件显示的一组人员。</span><span class="sxs-lookup"><span data-stu-id="f9e04-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="f9e04-110">您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="f9e04-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="f9e04-111">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="f9e04-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="f9e04-112">属性</span><span class="sxs-lookup"><span data-stu-id="f9e04-112">Properties</span></span>

<span data-ttu-id="f9e04-113">默认情况下， `mgt-people`组件使用`personType/class eq 'Person'`筛选器从`/me/people`终结点提取事件，以显示经常联系的用户。</span><span class="sxs-lookup"><span data-stu-id="f9e04-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="f9e04-114">您可以使用多个属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="f9e04-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="f9e04-115">属性</span><span class="sxs-lookup"><span data-stu-id="f9e04-115">Attribute</span></span> | <span data-ttu-id="f9e04-116">属性</span><span class="sxs-lookup"><span data-stu-id="f9e04-116">Property</span></span> | <span data-ttu-id="f9e04-117">说明</span><span class="sxs-lookup"><span data-stu-id="f9e04-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="f9e04-118">show-max</span><span class="sxs-lookup"><span data-stu-id="f9e04-118">show-max</span></span> | <span data-ttu-id="f9e04-119">showMax</span><span class="sxs-lookup"><span data-stu-id="f9e04-119">showMax</span></span> | <span data-ttu-id="f9e04-120">指示要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="f9e04-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="f9e04-121">默认值为3。</span><span class="sxs-lookup"><span data-stu-id="f9e04-121">Default value is 3.</span></span> |
| <span data-ttu-id="f9e04-122">people</span><span class="sxs-lookup"><span data-stu-id="f9e04-122">people</span></span> | <span data-ttu-id="f9e04-123">people</span><span class="sxs-lookup"><span data-stu-id="f9e04-123">people</span></span> | <span data-ttu-id="f9e04-124">获取或设置组件呈现的人员列表的人员数组。</span><span class="sxs-lookup"><span data-stu-id="f9e04-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="f9e04-125">使用此属性可访问组件加载的人员。</span><span class="sxs-lookup"><span data-stu-id="f9e04-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="f9e04-126">设置此值可加载自己的人员。</span><span class="sxs-lookup"><span data-stu-id="f9e04-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="f9e04-127">组 id</span><span class="sxs-lookup"><span data-stu-id="f9e04-127">group-id</span></span> | <span data-ttu-id="f9e04-128">groupId</span><span class="sxs-lookup"><span data-stu-id="f9e04-128">groupId</span></span> | <span data-ttu-id="f9e04-129">从各自的 ID 检索特定 Microsoft Graph 中的人员。</span><span class="sxs-lookup"><span data-stu-id="f9e04-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="f9e04-130">用户 id</span><span class="sxs-lookup"><span data-stu-id="f9e04-130">user-ids</span></span> | <span data-ttu-id="f9e04-131">userIds</span><span class="sxs-lookup"><span data-stu-id="f9e04-131">userIds</span></span> | <span data-ttu-id="f9e04-132">给定一个 Microsoft Graph 用户`ids`的数组，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="f9e04-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="f9e04-133">人员-卡片</span><span class="sxs-lookup"><span data-stu-id="f9e04-133">person-card</span></span> | <span data-ttu-id="f9e04-134">personCard</span><span class="sxs-lookup"><span data-stu-id="f9e04-134">personCard</span></span> | <span data-ttu-id="f9e04-135">一个枚举，用于确定激活浮出式面板- `hover`或`click`的必需用户操作。</span><span class="sxs-lookup"><span data-stu-id="f9e04-135">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="f9e04-136">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="f9e04-136">Default value is `none`.</span></span> |


<span data-ttu-id="f9e04-137">下面的示例设置要显示的最大用户数。</span><span class="sxs-lookup"><span data-stu-id="f9e04-137">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="f9e04-138">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="f9e04-138">CSS custom properties</span></span>

<span data-ttu-id="f9e04-139">`mgt-people`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="f9e04-139">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
}
```

## <a name="templates"></a><span data-ttu-id="f9e04-140">模板</span><span class="sxs-lookup"><span data-stu-id="f9e04-140">Templates</span></span>

<span data-ttu-id="f9e04-141">支持多个[模板](../templates.md)，这些模板可用于替换组件的某些部分。 `mgt-people`</span><span class="sxs-lookup"><span data-stu-id="f9e04-141">The `mgt-people` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="f9e04-142">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="f9e04-142">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="f9e04-143">数据类型</span><span class="sxs-lookup"><span data-stu-id="f9e04-143">Data type</span></span> | <span data-ttu-id="f9e04-144">数据上下文</span><span class="sxs-lookup"><span data-stu-id="f9e04-144">Data context</span></span> | <span data-ttu-id="f9e04-145">说明</span><span class="sxs-lookup"><span data-stu-id="f9e04-145">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="f9e04-146">`people`： person 对象列表</span><span class="sxs-lookup"><span data-stu-id="f9e04-146">`people`: list of person objects</span></span> | <span data-ttu-id="f9e04-147">默认模板会将整个组件替换为您自己的组件。</span><span class="sxs-lookup"><span data-stu-id="f9e04-147">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="f9e04-148">`person`： person 对象</span><span class="sxs-lookup"><span data-stu-id="f9e04-148">`person`: person object</span></span> | <span data-ttu-id="f9e04-149">用于呈现每个人的模板。</span><span class="sxs-lookup"><span data-stu-id="f9e04-149">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="f9e04-150">`people`： person 对象列表</span><span class="sxs-lookup"><span data-stu-id="f9e04-150">`people`: list of person objects</span></span> <br> <span data-ttu-id="f9e04-151">`max`：显示的人员的数量</span><span class="sxs-lookup"><span data-stu-id="f9e04-151">`max`: number of shown people</span></span> <br> <span data-ttu-id="f9e04-152">`extra`：额外人员数</span><span class="sxs-lookup"><span data-stu-id="f9e04-152">`extra`: number of extra people</span></span> | <span data-ttu-id="f9e04-153">用于将数字呈现在人员列表右侧的最大值之后的模板。</span><span class="sxs-lookup"><span data-stu-id="f9e04-153">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="f9e04-154">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="f9e04-154">No data context is passed</span></span> | <span data-ttu-id="f9e04-155">没有可用数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="f9e04-155">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="f9e04-156">不传递数据上下文</span><span class="sxs-lookup"><span data-stu-id="f9e04-156">No data context is passed</span></span> | <span data-ttu-id="f9e04-157">组件加载状态时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="f9e04-157">The template used while the component loads state.</span></span>

<span data-ttu-id="f9e04-158">下面的示例演示如何使用`person`模板。</span><span class="sxs-lookup"><span data-stu-id="f9e04-158">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="f9e04-159">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="f9e04-159">Microsoft Graph permissions</span></span>

<span data-ttu-id="f9e04-160">此组件使用以下 Microsoft Graph Api 和权限：</span><span class="sxs-lookup"><span data-stu-id="f9e04-160">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="f9e04-161">资源</span><span class="sxs-lookup"><span data-stu-id="f9e04-161">Resource</span></span> | <span data-ttu-id="f9e04-162">权限</span><span class="sxs-lookup"><span data-stu-id="f9e04-162">Permission</span></span> |
| - | - |
| [<span data-ttu-id="f9e04-163">/me/people</span><span class="sxs-lookup"><span data-stu-id="f9e04-163">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |

## <a name="authentication"></a><span data-ttu-id="f9e04-164">身份验证</span><span class="sxs-lookup"><span data-stu-id="f9e04-164">Authentication</span></span>

<span data-ttu-id="f9e04-165">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="f9e04-165">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="f9e04-166">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="f9e04-166">Extend for more control</span></span>

<span data-ttu-id="f9e04-167">对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法。</span><span class="sxs-lookup"><span data-stu-id="f9e04-167">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="f9e04-168">方法</span><span class="sxs-lookup"><span data-stu-id="f9e04-168">Method</span></span> | <span data-ttu-id="f9e04-169">说明</span><span class="sxs-lookup"><span data-stu-id="f9e04-169">Description</span></span> |
| - | - |
| <span data-ttu-id="f9e04-170">renderLoading</span><span class="sxs-lookup"><span data-stu-id="f9e04-170">renderLoading</span></span> | <span data-ttu-id="f9e04-171">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="f9e04-171">Renders the loading state.</span></span> |
| <span data-ttu-id="f9e04-172">renderNoData</span><span class="sxs-lookup"><span data-stu-id="f9e04-172">renderNoData</span></span> | <span data-ttu-id="f9e04-173">呈现空数据状态。</span><span class="sxs-lookup"><span data-stu-id="f9e04-173">Renders the empty data state.</span></span> |
| <span data-ttu-id="f9e04-174">renderPeople</span><span class="sxs-lookup"><span data-stu-id="f9e04-174">renderPeople</span></span> | <span data-ttu-id="f9e04-175">呈现最大`show-max`值的人员列表。</span><span class="sxs-lookup"><span data-stu-id="f9e04-175">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="f9e04-176">renderPerson</span><span class="sxs-lookup"><span data-stu-id="f9e04-176">renderPerson</span></span> | <span data-ttu-id="f9e04-177">呈现单个人员。</span><span class="sxs-lookup"><span data-stu-id="f9e04-177">Renders an individual person.</span></span> |
| <span data-ttu-id="f9e04-178">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="f9e04-178">renderOverflow</span></span> | <span data-ttu-id="f9e04-179">呈现除`show-max`值之外的剩余人员的表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9e04-179">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
