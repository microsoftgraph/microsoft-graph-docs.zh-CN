---
title: Microsoft Graph 功能中的人员Toolkit
description: 可以使用 Web 组件通过用户的照片或缩写显示一组 `mgt-people` 人员或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0cdade8720112dc623e617514f31ab63151b80ff
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266848"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="cd6b5-103">Microsoft Graph 功能中的人员Toolkit</span><span class="sxs-lookup"><span data-stu-id="cd6b5-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="cd6b5-104">可以使用 Web 组件通过用户的照片或缩写显示一组 `mgt-people` 人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="cd6b5-105">默认情况下，它将显示已登录用户的最常见的联系人。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="cd6b5-106">此组件使用多个 [mgt-person](./person.md) 控件，但可以绑定到一组人员描述符。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="cd6b5-107">如果要显示的人数多于该值，将添加一个号码以 `show-max` 指示其他联系人的数量。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="cd6b5-108">示例</span><span class="sxs-lookup"><span data-stu-id="cd6b5-108">Example</span></span>

<span data-ttu-id="cd6b5-109">以下示例显示使用组件显示的一组 `mgt-people` 人员。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="cd6b5-110">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="cd6b5-111">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="cd6b5-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="cd6b5-112">属性</span><span class="sxs-lookup"><span data-stu-id="cd6b5-112">Properties</span></span>

<span data-ttu-id="cd6b5-113">默认情况下，组件 `mgt-people` 通过筛选器从终结点 `/me/people` 提取事件 `personType/class eq 'Person'` 以显示经常联系的用户。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="cd6b5-114">可以使用多个属性更改此行为。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="cd6b5-115">属性</span><span class="sxs-lookup"><span data-stu-id="cd6b5-115">Attribute</span></span> | <span data-ttu-id="cd6b5-116">属性</span><span class="sxs-lookup"><span data-stu-id="cd6b5-116">Property</span></span> | <span data-ttu-id="cd6b5-117">说明</span><span class="sxs-lookup"><span data-stu-id="cd6b5-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="cd6b5-118">show-max</span><span class="sxs-lookup"><span data-stu-id="cd6b5-118">show-max</span></span> | <span data-ttu-id="cd6b5-119">showMax</span><span class="sxs-lookup"><span data-stu-id="cd6b5-119">showMax</span></span> | <span data-ttu-id="cd6b5-120">指示要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="cd6b5-121">默认值为 3。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-121">Default value is 3.</span></span> |
| <span data-ttu-id="cd6b5-122">people</span><span class="sxs-lookup"><span data-stu-id="cd6b5-122">people</span></span> | <span data-ttu-id="cd6b5-123">people</span><span class="sxs-lookup"><span data-stu-id="cd6b5-123">people</span></span> | <span data-ttu-id="cd6b5-124">用于获取或设置组件呈现的联系人列表的一组人员。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="cd6b5-125">使用此属性访问组件加载的人。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="cd6b5-126">设置此值以加载您自己的人员。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="cd6b5-127">group-id</span><span class="sxs-lookup"><span data-stu-id="cd6b5-127">group-id</span></span> | <span data-ttu-id="cd6b5-128">groupId</span><span class="sxs-lookup"><span data-stu-id="cd6b5-128">groupId</span></span> | <span data-ttu-id="cd6b5-129">从特定 Microsoft Graph 中从各自的 ID 检索用户。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="cd6b5-130">user-ids</span><span class="sxs-lookup"><span data-stu-id="cd6b5-130">user-ids</span></span> | <span data-ttu-id="cd6b5-131">userIds</span><span class="sxs-lookup"><span data-stu-id="cd6b5-131">userIds</span></span> | <span data-ttu-id="cd6b5-132">给定一组 Microsoft Graph 用户 `ids` ，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="cd6b5-133">人员查询</span><span class="sxs-lookup"><span data-stu-id="cd6b5-133">people-queries</span></span> | <span data-ttu-id="cd6b5-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="cd6b5-134">peopleQueries</span></span> | <span data-ttu-id="cd6b5-135">给定一组人员查询 (、更新、电子邮件) ，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="cd6b5-136">person-card</span><span class="sxs-lookup"><span data-stu-id="cd6b5-136">person-card</span></span> | <span data-ttu-id="cd6b5-137">personCard</span><span class="sxs-lookup"><span data-stu-id="cd6b5-137">personCard</span></span> | <span data-ttu-id="cd6b5-138">一个枚举，用于确定激活飞出面板或 所需的用户 `hover` 操作 `click` 。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="cd6b5-139">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-139">Default value is `none`.</span></span> |
| <span data-ttu-id="cd6b5-140">show-presence</span><span class="sxs-lookup"><span data-stu-id="cd6b5-140">show-presence</span></span> | <span data-ttu-id="cd6b5-141">showPresence</span><span class="sxs-lookup"><span data-stu-id="cd6b5-141">showPresence</span></span> | <span data-ttu-id="cd6b5-142">一个布尔值，用于确定是否在人像上显示个人状态锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-142">A boolean to determine whether to show person presence badge on person image.</span></span> |


<span data-ttu-id="cd6b5-143">以下示例设置要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-143">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="cd6b5-144">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="cd6b5-144">CSS custom properties</span></span>

<span data-ttu-id="cd6b5-145">组件 `mgt-people` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-145">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="cd6b5-146">模板</span><span class="sxs-lookup"><span data-stu-id="cd6b5-146">Templates</span></span>

<span data-ttu-id="cd6b5-147">`mgt-people`支持[多个模板](../customize-components/templates.md)，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-147">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="cd6b5-148">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-148">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="cd6b5-149">数据类型</span><span class="sxs-lookup"><span data-stu-id="cd6b5-149">Data type</span></span> | <span data-ttu-id="cd6b5-150">数据上下文</span><span class="sxs-lookup"><span data-stu-id="cd6b5-150">Data context</span></span> | <span data-ttu-id="cd6b5-151">说明</span><span class="sxs-lookup"><span data-stu-id="cd6b5-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="cd6b5-152">`people`：人员对象列表</span><span class="sxs-lookup"><span data-stu-id="cd6b5-152">`people`: list of person objects</span></span> | <span data-ttu-id="cd6b5-153">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-153">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="cd6b5-154">`person`：person 对象</span><span class="sxs-lookup"><span data-stu-id="cd6b5-154">`person`: person object</span></span> | <span data-ttu-id="cd6b5-155">用于呈现每个人模板。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-155">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="cd6b5-156">`people`：人员对象列表</span><span class="sxs-lookup"><span data-stu-id="cd6b5-156">`people`: list of person objects</span></span> <br> <span data-ttu-id="cd6b5-157">`max`：显示人数</span><span class="sxs-lookup"><span data-stu-id="cd6b5-157">`max`: number of shown people</span></span> <br> <span data-ttu-id="cd6b5-158">`extra`：额外人员的数量</span><span class="sxs-lookup"><span data-stu-id="cd6b5-158">`extra`: number of extra people</span></span> | <span data-ttu-id="cd6b5-159">用于呈现超过人员列表右侧最大值的号码的模板。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-159">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="cd6b5-160">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="cd6b5-160">No data context is passed</span></span> | <span data-ttu-id="cd6b5-161">没有可用数据时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-161">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="cd6b5-162">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="cd6b5-162">No data context is passed</span></span> | <span data-ttu-id="cd6b5-163">组件加载状态时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-163">The template used while the component loads state.</span></span>

<span data-ttu-id="cd6b5-164">以下示例演示如何使用 `person` 模板。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-164">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="cd6b5-165">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="cd6b5-165">Microsoft Graph permissions</span></span>

<span data-ttu-id="cd6b5-166">此组件使用下列 Microsoft Graph API 和权限：</span><span class="sxs-lookup"><span data-stu-id="cd6b5-166">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="cd6b5-167">Resource</span><span class="sxs-lookup"><span data-stu-id="cd6b5-167">Resource</span></span> | <span data-ttu-id="cd6b5-168">权限</span><span class="sxs-lookup"><span data-stu-id="cd6b5-168">Permission</span></span> |
| - | - |
| [<span data-ttu-id="cd6b5-169">/me/people</span><span class="sxs-lookup"><span data-stu-id="cd6b5-169">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="cd6b5-170">使用默认模板时，需要其他 API 和权限。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-170">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="cd6b5-171">此组件的默认模板使用 [mgt-person](person.md) 组件，这需要以下内容。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-171">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="cd6b5-172">Resource</span><span class="sxs-lookup"><span data-stu-id="cd6b5-172">Resource</span></span> | <span data-ttu-id="cd6b5-173">权限</span><span class="sxs-lookup"><span data-stu-id="cd6b5-173">Permission</span></span> |
| - | - |
| [<span data-ttu-id="cd6b5-174">/users</span><span class="sxs-lookup"><span data-stu-id="cd6b5-174">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="cd6b5-175">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="cd6b5-175">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="cd6b5-176">身份验证</span><span class="sxs-lookup"><span data-stu-id="cd6b5-176">Authentication</span></span>

<span data-ttu-id="cd6b5-177">该控件使用身份验证文档中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-177">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="cd6b5-178">缓存</span><span class="sxs-lookup"><span data-stu-id="cd6b5-178">Cache</span></span>

|<span data-ttu-id="cd6b5-179">对象存储</span><span class="sxs-lookup"><span data-stu-id="cd6b5-179">Object store</span></span>|<span data-ttu-id="cd6b5-180">缓存数据</span><span class="sxs-lookup"><span data-stu-id="cd6b5-180">Cached data</span></span>|<span data-ttu-id="cd6b5-181">备注</span><span class="sxs-lookup"><span data-stu-id="cd6b5-181">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="cd6b5-182">有关与查询匹配的人的信息</span><span class="sxs-lookup"><span data-stu-id="cd6b5-182">Information about people matching the query</span></span>|<span data-ttu-id="cd6b5-183">指定时 `resource` 使用</span><span class="sxs-lookup"><span data-stu-id="cd6b5-183">Used when `resource` specified</span></span>|
|`users`|<span data-ttu-id="cd6b5-184">有关与查询匹配的用户的信息</span><span class="sxs-lookup"><span data-stu-id="cd6b5-184">Information about users matching the query</span></span>|<span data-ttu-id="cd6b5-185">在 `groupId` 、 `userIds` 或 `peopleQueries` 未指定任何属性时使用</span><span class="sxs-lookup"><span data-stu-id="cd6b5-185">Used when `groupId`, `userIds`, `peopleQueries` or no properties specified</span></span>|
|`presence`|<span data-ttu-id="cd6b5-186">指定人员集状态</span><span class="sxs-lookup"><span data-stu-id="cd6b5-186">Presence for the specified set of people</span></span>|<span data-ttu-id="cd6b5-187">设置为 `showPresence` 时使用 `true`</span><span class="sxs-lookup"><span data-stu-id="cd6b5-187">Used when `showPresence` set to `true`</span></span>|

> [!NOTE]
> <span data-ttu-id="cd6b5-188">默认情况下， `mgt-people` 组件使用该 [`mgt-person`](./person.md) 组件来显示有关人员的信息。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-188">By default, the `mgt-people` component uses the [`mgt-person`](./person.md) component to display information about people.</span></span> <span data-ttu-id="cd6b5-189">`mgt-person`组件自动下载并缓存每个人的照片。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-189">The `mgt-person` component automatically downloads and caches the photo for each person.</span></span>

<span data-ttu-id="cd6b5-190">若要 [详细了解](../customize-components/cache.md) 如何配置缓存，请参阅缓存。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-190">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="cd6b5-191">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="cd6b5-191">Extend for more control</span></span>

<span data-ttu-id="cd6b5-192">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-192">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="cd6b5-193">方法</span><span class="sxs-lookup"><span data-stu-id="cd6b5-193">Method</span></span> | <span data-ttu-id="cd6b5-194">说明</span><span class="sxs-lookup"><span data-stu-id="cd6b5-194">Description</span></span> |
| - | - |
| <span data-ttu-id="cd6b5-195">renderLoading</span><span class="sxs-lookup"><span data-stu-id="cd6b5-195">renderLoading</span></span> | <span data-ttu-id="cd6b5-196">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-196">Renders the loading state.</span></span> |
| <span data-ttu-id="cd6b5-197">renderNoData</span><span class="sxs-lookup"><span data-stu-id="cd6b5-197">renderNoData</span></span> | <span data-ttu-id="cd6b5-198">呈现空数据状态。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-198">Renders the empty data state.</span></span> |
| <span data-ttu-id="cd6b5-199">renderPeople</span><span class="sxs-lookup"><span data-stu-id="cd6b5-199">renderPeople</span></span> | <span data-ttu-id="cd6b5-200">呈现人员列表，最多呈现 `show-max` 值。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-200">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="cd6b5-201">renderPerson</span><span class="sxs-lookup"><span data-stu-id="cd6b5-201">renderPerson</span></span> | <span data-ttu-id="cd6b5-202">呈现单个人员。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-202">Renders an individual person.</span></span> |
| <span data-ttu-id="cd6b5-203">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="cd6b5-203">renderOverflow</span></span> | <span data-ttu-id="cd6b5-204">呈现值以外的剩余人的 `show-max` 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd6b5-204">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
