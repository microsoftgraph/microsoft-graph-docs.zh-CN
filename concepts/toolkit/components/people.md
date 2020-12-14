---
title: Microsoft Graph 功能中的人员Toolkit
description: 您可以使用 Web 组件通过用户的照片或缩写显示一 `mgt-people` 组人员或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 9e19636c6f69784984d7438d53f57bac78fc6675
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660056"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c4e05-103">Microsoft Graph 功能中的人员Toolkit</span><span class="sxs-lookup"><span data-stu-id="c4e05-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c4e05-104">您可以使用 Web 组件通过用户的照片或缩写显示一 `mgt-people` 组人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="c4e05-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="c4e05-105">默认情况下，它将显示已登录用户的最常见的联系人。</span><span class="sxs-lookup"><span data-stu-id="c4e05-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="c4e05-106">此组件使用多个 [人员](./person.md) 控制，但可以绑定到一组人员描述符。</span><span class="sxs-lookup"><span data-stu-id="c4e05-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="c4e05-107">如果显示人数多于该值，将添加一个数字以 `show-max` 指示其他联系人的数量。</span><span class="sxs-lookup"><span data-stu-id="c4e05-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="c4e05-108">示例</span><span class="sxs-lookup"><span data-stu-id="c4e05-108">Example</span></span>

<span data-ttu-id="c4e05-109">以下示例显示了使用组件显示的一组 `mgt-people` 人员。</span><span class="sxs-lookup"><span data-stu-id="c4e05-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="c4e05-110">可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="c4e05-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="c4e05-111">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="c4e05-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="c4e05-112">属性</span><span class="sxs-lookup"><span data-stu-id="c4e05-112">Properties</span></span>

<span data-ttu-id="c4e05-113">默认情况下，组件通过筛选器从终结点提取事件 `mgt-people` `/me/people` `personType/class eq 'Person'` 以显示经常联系的用户。</span><span class="sxs-lookup"><span data-stu-id="c4e05-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="c4e05-114">可以使用多个属性更改此行为。</span><span class="sxs-lookup"><span data-stu-id="c4e05-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="c4e05-115">属性</span><span class="sxs-lookup"><span data-stu-id="c4e05-115">Attribute</span></span> | <span data-ttu-id="c4e05-116">属性</span><span class="sxs-lookup"><span data-stu-id="c4e05-116">Property</span></span> | <span data-ttu-id="c4e05-117">说明</span><span class="sxs-lookup"><span data-stu-id="c4e05-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="c4e05-118">show-max</span><span class="sxs-lookup"><span data-stu-id="c4e05-118">show-max</span></span> | <span data-ttu-id="c4e05-119">showMax</span><span class="sxs-lookup"><span data-stu-id="c4e05-119">showMax</span></span> | <span data-ttu-id="c4e05-120">指示要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="c4e05-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="c4e05-121">默认值为 3。</span><span class="sxs-lookup"><span data-stu-id="c4e05-121">Default value is 3.</span></span> |
| <span data-ttu-id="c4e05-122">people</span><span class="sxs-lookup"><span data-stu-id="c4e05-122">people</span></span> | <span data-ttu-id="c4e05-123">people</span><span class="sxs-lookup"><span data-stu-id="c4e05-123">people</span></span> | <span data-ttu-id="c4e05-124">用于获取或设置组件呈现人员列表的一组人员。</span><span class="sxs-lookup"><span data-stu-id="c4e05-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="c4e05-125">使用此属性访问组件加载的人。</span><span class="sxs-lookup"><span data-stu-id="c4e05-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="c4e05-126">设置此值可加载您自己的人员。</span><span class="sxs-lookup"><span data-stu-id="c4e05-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="c4e05-127">group-id</span><span class="sxs-lookup"><span data-stu-id="c4e05-127">group-id</span></span> | <span data-ttu-id="c4e05-128">groupId</span><span class="sxs-lookup"><span data-stu-id="c4e05-128">groupId</span></span> | <span data-ttu-id="c4e05-129">从特定 Microsoft Graph 中检索相应 ID 中的人员。</span><span class="sxs-lookup"><span data-stu-id="c4e05-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="c4e05-130">user-ids</span><span class="sxs-lookup"><span data-stu-id="c4e05-130">user-ids</span></span> | <span data-ttu-id="c4e05-131">userIds</span><span class="sxs-lookup"><span data-stu-id="c4e05-131">userIds</span></span> | <span data-ttu-id="c4e05-132">给定 Microsoft Graph 用户数组 `ids` 后，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="c4e05-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="c4e05-133">people-queries</span><span class="sxs-lookup"><span data-stu-id="c4e05-133">people-queries</span></span> | <span data-ttu-id="c4e05-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="c4e05-134">peopleQueries</span></span> | <span data-ttu-id="c4e05-135">给定一组人员查询 (、upns、电子邮件) ，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="c4e05-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="c4e05-136">person-card</span><span class="sxs-lookup"><span data-stu-id="c4e05-136">person-card</span></span> | <span data-ttu-id="c4e05-137">personCard</span><span class="sxs-lookup"><span data-stu-id="c4e05-137">personCard</span></span> | <span data-ttu-id="c4e05-138">一个枚举，用于确定激活飞出面板所需的用户操作 - `hover` 或 `click` 。</span><span class="sxs-lookup"><span data-stu-id="c4e05-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="c4e05-139">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="c4e05-139">Default value is `none`.</span></span> |
| <span data-ttu-id="c4e05-140">show-presence</span><span class="sxs-lookup"><span data-stu-id="c4e05-140">show-presence</span></span> | <span data-ttu-id="c4e05-141">showPresence</span><span class="sxs-lookup"><span data-stu-id="c4e05-141">showPresence</span></span> | <span data-ttu-id="c4e05-142">一个布尔值，用于确定是否在人像上显示人员状态锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="c4e05-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="c4e05-143">以下示例设置要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="c4e05-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="c4e05-144">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="c4e05-144">CSS custom properties</span></span>

<span data-ttu-id="c4e05-145">该 `mgt-people` 组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="c4e05-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="c4e05-146">模板</span><span class="sxs-lookup"><span data-stu-id="c4e05-146">Templates</span></span>

<span data-ttu-id="c4e05-147">支持 `mgt-people` [多个模板](../customize-components/templates.md) ，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="c4e05-147">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="c4e05-148">若要指定模板，请包含 `<template>` 组件中的元素，将值设置为下列 `data-type` 值之一。</span><span class="sxs-lookup"><span data-stu-id="c4e05-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="c4e05-149">数据类型</span><span class="sxs-lookup"><span data-stu-id="c4e05-149">Data type</span></span> | <span data-ttu-id="c4e05-150">数据上下文</span><span class="sxs-lookup"><span data-stu-id="c4e05-150">Data context</span></span> | <span data-ttu-id="c4e05-151">说明</span><span class="sxs-lookup"><span data-stu-id="c4e05-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="c4e05-152">`people`：人员对象列表</span><span class="sxs-lookup"><span data-stu-id="c4e05-152">`people`: list of person objects</span></span> | <span data-ttu-id="c4e05-153">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="c4e05-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="c4e05-154">`person`： person 对象</span><span class="sxs-lookup"><span data-stu-id="c4e05-154">`person`: person object</span></span> | <span data-ttu-id="c4e05-155">用于呈现每个人模板。</span><span class="sxs-lookup"><span data-stu-id="c4e05-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="c4e05-156">`people`：人员对象列表</span><span class="sxs-lookup"><span data-stu-id="c4e05-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="c4e05-157">`max`： 显示人员的数量</span><span class="sxs-lookup"><span data-stu-id="c4e05-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="c4e05-158">`extra`：额外人员的数量</span><span class="sxs-lookup"><span data-stu-id="c4e05-158">`extra`: number of extra people</span></span> | <span data-ttu-id="c4e05-159">用于呈现超过人员列表右侧最大值的号码的模板。</span><span class="sxs-lookup"><span data-stu-id="c4e05-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="c4e05-160">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="c4e05-160">No data context is passed</span></span> | <span data-ttu-id="c4e05-161">没有可用数据时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="c4e05-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="c4e05-162">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="c4e05-162">No data context is passed</span></span> | <span data-ttu-id="c4e05-163">组件加载状态时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="c4e05-163">The template used while the component loads state.</span></span>

<span data-ttu-id="c4e05-164">以下示例显示如何使用 `person` 模板。</span><span class="sxs-lookup"><span data-stu-id="c4e05-164">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="c4e05-165">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="c4e05-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="c4e05-166">此组件使用以下 Microsoft Graph API 和权限：</span><span class="sxs-lookup"><span data-stu-id="c4e05-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="c4e05-167">资源</span><span class="sxs-lookup"><span data-stu-id="c4e05-167">Resource</span></span> | <span data-ttu-id="c4e05-168">权限</span><span class="sxs-lookup"><span data-stu-id="c4e05-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="c4e05-169">/me/people</span><span class="sxs-lookup"><span data-stu-id="c4e05-169">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="c4e05-170">使用默认模板时，需要其他 API 和权限。</span><span class="sxs-lookup"><span data-stu-id="c4e05-170">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="c4e05-171">此组件的默认模板使用 [mgt-person](person.md) 组件，这需要以下内容。</span><span class="sxs-lookup"><span data-stu-id="c4e05-171">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="c4e05-172">资源</span><span class="sxs-lookup"><span data-stu-id="c4e05-172">Resource</span></span> | <span data-ttu-id="c4e05-173">权限</span><span class="sxs-lookup"><span data-stu-id="c4e05-173">Permission</span></span> |
| - | - |
| [<span data-ttu-id="c4e05-174">/users</span><span class="sxs-lookup"><span data-stu-id="c4e05-174">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="c4e05-175">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="c4e05-175">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="c4e05-176">身份验证</span><span class="sxs-lookup"><span data-stu-id="c4e05-176">Authentication</span></span>

<span data-ttu-id="c4e05-177">该控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="c4e05-177">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="c4e05-178">扩展以更多控制</span><span class="sxs-lookup"><span data-stu-id="c4e05-178">Extend for more control</span></span>

<span data-ttu-id="c4e05-179">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法。</span><span class="sxs-lookup"><span data-stu-id="c4e05-179">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="c4e05-180">方法</span><span class="sxs-lookup"><span data-stu-id="c4e05-180">Method</span></span> | <span data-ttu-id="c4e05-181">说明</span><span class="sxs-lookup"><span data-stu-id="c4e05-181">Description</span></span> |
| - | - |
| <span data-ttu-id="c4e05-182">renderLoading</span><span class="sxs-lookup"><span data-stu-id="c4e05-182">renderLoading</span></span> | <span data-ttu-id="c4e05-183">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="c4e05-183">Renders the loading state.</span></span> |
| <span data-ttu-id="c4e05-184">renderNoData</span><span class="sxs-lookup"><span data-stu-id="c4e05-184">renderNoData</span></span> | <span data-ttu-id="c4e05-185">呈现空数据状态。</span><span class="sxs-lookup"><span data-stu-id="c4e05-185">Renders the empty data state.</span></span> |
| <span data-ttu-id="c4e05-186">renderPeople</span><span class="sxs-lookup"><span data-stu-id="c4e05-186">renderPeople</span></span> | <span data-ttu-id="c4e05-187">呈现人员列表，最多呈现 `show-max` 值。</span><span class="sxs-lookup"><span data-stu-id="c4e05-187">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="c4e05-188">renderPerson</span><span class="sxs-lookup"><span data-stu-id="c4e05-188">renderPerson</span></span> | <span data-ttu-id="c4e05-189">呈现单个人员。</span><span class="sxs-lookup"><span data-stu-id="c4e05-189">Renders an individual person.</span></span> |
| <span data-ttu-id="c4e05-190">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="c4e05-190">renderOverflow</span></span> | <span data-ttu-id="c4e05-191">呈现剩余人员超出该值 `show-max` 的表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4e05-191">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
