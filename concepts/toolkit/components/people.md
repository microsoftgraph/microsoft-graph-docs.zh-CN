---
title: Microsoft 服务中的人员Graph Toolkit
description: 可以使用 Web 组件通过用户的照片或缩写显示一组 `mgt-people` 人员或联系人。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 6bed8f2c06e3c6834533b8e881016c4bc6d54bac
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52580013"
---
# <a name="people-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="83e0b-103">Microsoft 服务中的人员Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="83e0b-103">People component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="83e0b-104">可以使用 Web 组件通过用户的照片或缩写显示一组 `mgt-people` 人员或联系人。</span><span class="sxs-lookup"><span data-stu-id="83e0b-104">You can use the `mgt-people` web component to display a group of people or contacts by using their photos or initials.</span></span> <span data-ttu-id="83e0b-105">默认情况下，它将显示已登录用户的最常见的联系人。</span><span class="sxs-lookup"><span data-stu-id="83e0b-105">By default, it will display the most frequent contacts for the signed in user.</span></span>

<span data-ttu-id="83e0b-106">此组件使用多个 [mgt-person](./person.md) 控件，但可以绑定到一组人员描述符。</span><span class="sxs-lookup"><span data-stu-id="83e0b-106">This component uses multiple [mgt-person](./person.md) controls, but it can be bound to a set of people descriptors.</span></span> <span data-ttu-id="83e0b-107">如果要显示的人数多于该值，将添加一个号码以 `show-max` 指示其他联系人的数量。</span><span class="sxs-lookup"><span data-stu-id="83e0b-107">If there are more people to display than the `show-max` value, a number will be added to indicate the number of additional contacts.</span></span>

## <a name="example"></a><span data-ttu-id="83e0b-108">示例</span><span class="sxs-lookup"><span data-stu-id="83e0b-108">Example</span></span>

<span data-ttu-id="83e0b-109">以下示例显示使用组件显示的一组 `mgt-people` 人员。</span><span class="sxs-lookup"><span data-stu-id="83e0b-109">The following example shows a group of people displayed using the `mgt-people` component.</span></span> <span data-ttu-id="83e0b-110">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="83e0b-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people--people&source=docs" height="350"></iframe>

[<span data-ttu-id="83e0b-111">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="83e0b-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people--people&source=docs)

## <a name="properties"></a><span data-ttu-id="83e0b-112">属性</span><span class="sxs-lookup"><span data-stu-id="83e0b-112">Properties</span></span>

<span data-ttu-id="83e0b-113">默认情况下，组件 `mgt-people` 通过筛选器从终结点 `/me/people` 提取事件 `personType/class eq 'Person'` 以显示经常联系的用户。</span><span class="sxs-lookup"><span data-stu-id="83e0b-113">By default, the `mgt-people` component fetches events from the `/me/people` endpoint with the `personType/class eq 'Person'` filter to display frequently contacted users.</span></span> <span data-ttu-id="83e0b-114">可以使用多个属性更改此行为。</span><span class="sxs-lookup"><span data-stu-id="83e0b-114">You can use several properties to change this behavior.</span></span>

| <span data-ttu-id="83e0b-115">属性</span><span class="sxs-lookup"><span data-stu-id="83e0b-115">Attribute</span></span> | <span data-ttu-id="83e0b-116">属性</span><span class="sxs-lookup"><span data-stu-id="83e0b-116">Property</span></span> | <span data-ttu-id="83e0b-117">说明</span><span class="sxs-lookup"><span data-stu-id="83e0b-117">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="83e0b-118">show-max</span><span class="sxs-lookup"><span data-stu-id="83e0b-118">show-max</span></span> | <span data-ttu-id="83e0b-119">showMax</span><span class="sxs-lookup"><span data-stu-id="83e0b-119">showMax</span></span> | <span data-ttu-id="83e0b-120">指示要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="83e0b-120">Indicates the maximum number of people to show.</span></span> <span data-ttu-id="83e0b-121">默认值为 3。</span><span class="sxs-lookup"><span data-stu-id="83e0b-121">Default value is 3.</span></span> |
| <span data-ttu-id="83e0b-122">people</span><span class="sxs-lookup"><span data-stu-id="83e0b-122">people</span></span> | <span data-ttu-id="83e0b-123">people</span><span class="sxs-lookup"><span data-stu-id="83e0b-123">people</span></span> | <span data-ttu-id="83e0b-124">用于获取或设置组件呈现的联系人列表的一组人员。</span><span class="sxs-lookup"><span data-stu-id="83e0b-124">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="83e0b-125">使用此属性访问组件加载的人。</span><span class="sxs-lookup"><span data-stu-id="83e0b-125">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="83e0b-126">设置此值以加载您自己的人员。</span><span class="sxs-lookup"><span data-stu-id="83e0b-126">Set this value to load your own people.</span></span> |
| <span data-ttu-id="83e0b-127">group-id</span><span class="sxs-lookup"><span data-stu-id="83e0b-127">group-id</span></span> | <span data-ttu-id="83e0b-128">groupId</span><span class="sxs-lookup"><span data-stu-id="83e0b-128">groupId</span></span> | <span data-ttu-id="83e0b-129">从特定 Microsoft Graph检索相应 ID 中的人员。</span><span class="sxs-lookup"><span data-stu-id="83e0b-129">Retrieves people from a specific Microsoft Graph from the respective ID.</span></span> |
| <span data-ttu-id="83e0b-130">user-ids</span><span class="sxs-lookup"><span data-stu-id="83e0b-130">user-ids</span></span> | <span data-ttu-id="83e0b-131">userIds</span><span class="sxs-lookup"><span data-stu-id="83e0b-131">userIds</span></span> | <span data-ttu-id="83e0b-132">给定一组 Microsoft `ids` Graph，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="83e0b-132">Given an array of Microsoft Graph user `ids`, the component will render these users.</span></span>  |
| <span data-ttu-id="83e0b-133">人员查询</span><span class="sxs-lookup"><span data-stu-id="83e0b-133">people-queries</span></span> | <span data-ttu-id="83e0b-134">peopleQueries</span><span class="sxs-lookup"><span data-stu-id="83e0b-134">peopleQueries</span></span> | <span data-ttu-id="83e0b-135">给定一组人员查询 (、更新、电子邮件) ，组件将呈现这些用户。</span><span class="sxs-lookup"><span data-stu-id="83e0b-135">Given an array of person queries (names, upns, emails), the component will render these users.</span></span> |
| <span data-ttu-id="83e0b-136">person-card</span><span class="sxs-lookup"><span data-stu-id="83e0b-136">person-card</span></span> | <span data-ttu-id="83e0b-137">personCard</span><span class="sxs-lookup"><span data-stu-id="83e0b-137">personCard</span></span> | <span data-ttu-id="83e0b-138">一个枚举，用于确定激活飞出面板或 所需的用户 `hover` 操作 `click` 。</span><span class="sxs-lookup"><span data-stu-id="83e0b-138">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="83e0b-139">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="83e0b-139">Default value is `none`.</span></span> |
| <span data-ttu-id="83e0b-140">show-presence</span><span class="sxs-lookup"><span data-stu-id="83e0b-140">show-presence</span></span> | <span data-ttu-id="83e0b-141">showPresence</span><span class="sxs-lookup"><span data-stu-id="83e0b-141">showPresence</span></span> | <span data-ttu-id="83e0b-142">一个布尔值，用于确定是否在人像上显示个人状态锁屏提醒。</span><span class="sxs-lookup"><span data-stu-id="83e0b-142">A boolean to determine whether to show person presence badge on person image.</span></span> |
| <span data-ttu-id="83e0b-143">resource</span><span class="sxs-lookup"><span data-stu-id="83e0b-143">resource</span></span> | <span data-ttu-id="83e0b-144">resource</span><span class="sxs-lookup"><span data-stu-id="83e0b-144">resource</span></span> | <span data-ttu-id="83e0b-145">从 Microsoft 获取的资源Graph (例如 `/me/people` ，) 。</span><span class="sxs-lookup"><span data-stu-id="83e0b-145">The resource to get from Microsoft Graph (for example, `/me/people`).</span></span> |
| <span data-ttu-id="83e0b-146">scopes</span><span class="sxs-lookup"><span data-stu-id="83e0b-146">scopes</span></span> | <span data-ttu-id="83e0b-147">scopes</span><span class="sxs-lookup"><span data-stu-id="83e0b-147">scopes</span></span> | <span data-ttu-id="83e0b-148">字符串的可选数组（如果使用 属性）或逗号分隔的范围（如果使用 属性）。</span><span class="sxs-lookup"><span data-stu-id="83e0b-148">Optional array of strings if using the property or a comma delimited scope if using the attribute.</span></span> <span data-ttu-id="83e0b-149">组件将使用这些作用域 (支持) ，以确保用户已同意适当的权限。</span><span class="sxs-lookup"><span data-stu-id="83e0b-149">The component will use these scopes (with a supported provider) to ensure that the user has consented to the right permission.</span></span> |
| <span data-ttu-id="83e0b-150">version</span><span class="sxs-lookup"><span data-stu-id="83e0b-150">version</span></span> | <span data-ttu-id="83e0b-151">version</span><span class="sxs-lookup"><span data-stu-id="83e0b-151">version</span></span> | <span data-ttu-id="83e0b-152">进行 GET 请求时使用的可选 API 版本。</span><span class="sxs-lookup"><span data-stu-id="83e0b-152">Optional API version to use when making the GET request.</span></span> <span data-ttu-id="83e0b-153">默认值为“`v1.0`”。</span><span class="sxs-lookup"><span data-stu-id="83e0b-153">Default is `v1.0`.</span></span>  |


<span data-ttu-id="83e0b-154">以下示例设置要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="83e0b-154">The following example sets the maximum number of people to show.</span></span>

```html
<mgt-people
  show-max="4">
</mgt-people>
```

## <a name="css-custom-properties"></a><span data-ttu-id="83e0b-155">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="83e0b-155">CSS custom properties</span></span>

<span data-ttu-id="83e0b-156">组件 `mgt-people` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="83e0b-156">The `mgt-people` component defines the following CSS custom properties.</span></span>

```css
mgt-people {
  --list-margin: 8px 4px 8px 8px; /* Margin for component */
  --avatar-margin: 0 4px 0 0; /* Margin for each person */
  --color: #000000 /* Text color *?
}
```

## <a name="templates"></a><span data-ttu-id="83e0b-157">模板</span><span class="sxs-lookup"><span data-stu-id="83e0b-157">Templates</span></span>

<span data-ttu-id="83e0b-158">`mgt-people`支持[多个模板](../customize-components/templates.md)，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="83e0b-158">The `mgt-people` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="83e0b-159">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。</span><span class="sxs-lookup"><span data-stu-id="83e0b-159">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="83e0b-160">数据类型</span><span class="sxs-lookup"><span data-stu-id="83e0b-160">Data type</span></span> | <span data-ttu-id="83e0b-161">数据上下文</span><span class="sxs-lookup"><span data-stu-id="83e0b-161">Data context</span></span> | <span data-ttu-id="83e0b-162">说明</span><span class="sxs-lookup"><span data-stu-id="83e0b-162">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="83e0b-163">`people`：人员对象列表</span><span class="sxs-lookup"><span data-stu-id="83e0b-163">`people`: list of person objects</span></span> | <span data-ttu-id="83e0b-164">默认模板将整个组件替换为你自己的组件。</span><span class="sxs-lookup"><span data-stu-id="83e0b-164">The default template replaces the entire component with your own.</span></span> |
| `person` | <span data-ttu-id="83e0b-165">`person`：person 对象</span><span class="sxs-lookup"><span data-stu-id="83e0b-165">`person`: person object</span></span> | <span data-ttu-id="83e0b-166">用于呈现每个人模板。</span><span class="sxs-lookup"><span data-stu-id="83e0b-166">The template used to render each person.</span></span> |
| `overflow` | <span data-ttu-id="83e0b-167">`people`：人员对象列表</span><span class="sxs-lookup"><span data-stu-id="83e0b-167">`people`: list of person objects</span></span> <br> <span data-ttu-id="83e0b-168">`max`：显示人数</span><span class="sxs-lookup"><span data-stu-id="83e0b-168">`max`: number of shown people</span></span> <br> <span data-ttu-id="83e0b-169">`extra`：额外人员的数量</span><span class="sxs-lookup"><span data-stu-id="83e0b-169">`extra`: number of extra people</span></span> | <span data-ttu-id="83e0b-170">用于呈现超过人员列表右侧最大值的号码的模板。</span><span class="sxs-lookup"><span data-stu-id="83e0b-170">The template used to render the number beyond the max to the right of the list of people.</span></span> |
| `no-data` | <span data-ttu-id="83e0b-171">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="83e0b-171">No data context is passed</span></span> | <span data-ttu-id="83e0b-172">没有可用数据时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="83e0b-172">The template used when no data is available.</span></span> |
| `loading` | <span data-ttu-id="83e0b-173">不传递任何数据上下文</span><span class="sxs-lookup"><span data-stu-id="83e0b-173">No data context is passed</span></span> | <span data-ttu-id="83e0b-174">组件加载状态时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="83e0b-174">The template used while the component loads state.</span></span>

<span data-ttu-id="83e0b-175">以下示例演示如何使用 `person` 模板。</span><span class="sxs-lookup"><span data-stu-id="83e0b-175">The following examples shows how to use the `person` template.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="83e0b-176">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="83e0b-176">Microsoft Graph permissions</span></span>

<span data-ttu-id="83e0b-177">此组件使用以下 Microsoft Graph API 和权限：</span><span class="sxs-lookup"><span data-stu-id="83e0b-177">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="83e0b-178">资源</span><span class="sxs-lookup"><span data-stu-id="83e0b-178">Resource</span></span> | <span data-ttu-id="83e0b-179">权限</span><span class="sxs-lookup"><span data-stu-id="83e0b-179">Permission</span></span> |
| - | - |
| [<span data-ttu-id="83e0b-180">/me/people</span><span class="sxs-lookup"><span data-stu-id="83e0b-180">/me/people</span></span>](/graph/api/user-list-people) | `People.Read` |

<span data-ttu-id="83e0b-181">使用默认模板时，需要其他 API 和权限。</span><span class="sxs-lookup"><span data-stu-id="83e0b-181">When using the default templates, additional APIs and permissions are required.</span></span> <span data-ttu-id="83e0b-182">此组件的默认模板使用 [mgt-person](person.md) 组件，这需要以下内容。</span><span class="sxs-lookup"><span data-stu-id="83e0b-182">The default template for this component uses a [mgt-person](person.md) component, which requires the following.</span></span>

| <span data-ttu-id="83e0b-183">资源</span><span class="sxs-lookup"><span data-stu-id="83e0b-183">Resource</span></span> | <span data-ttu-id="83e0b-184">权限</span><span class="sxs-lookup"><span data-stu-id="83e0b-184">Permission</span></span> |
| - | - |
| [<span data-ttu-id="83e0b-185">/users</span><span class="sxs-lookup"><span data-stu-id="83e0b-185">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="83e0b-186">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="83e0b-186">User.ReadBasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="83e0b-187">身份验证</span><span class="sxs-lookup"><span data-stu-id="83e0b-187">Authentication</span></span>

<span data-ttu-id="83e0b-188">该控件使用身份验证文档中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="83e0b-188">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="83e0b-189">缓存</span><span class="sxs-lookup"><span data-stu-id="83e0b-189">Cache</span></span>

|<span data-ttu-id="83e0b-190">对象存储</span><span class="sxs-lookup"><span data-stu-id="83e0b-190">Object store</span></span>|<span data-ttu-id="83e0b-191">缓存数据</span><span class="sxs-lookup"><span data-stu-id="83e0b-191">Cached data</span></span>|<span data-ttu-id="83e0b-192">备注</span><span class="sxs-lookup"><span data-stu-id="83e0b-192">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="83e0b-193">有关与查询匹配的人的信息</span><span class="sxs-lookup"><span data-stu-id="83e0b-193">Information about people matching the query</span></span>|<span data-ttu-id="83e0b-194">指定时 `resource` 使用</span><span class="sxs-lookup"><span data-stu-id="83e0b-194">Used when `resource` specified</span></span>|
|`users`|<span data-ttu-id="83e0b-195">有关与查询匹配的用户的信息</span><span class="sxs-lookup"><span data-stu-id="83e0b-195">Information about users matching the query</span></span>|<span data-ttu-id="83e0b-196">在 `groupId` 、 `userIds` 或 `peopleQueries` 未指定任何属性时使用</span><span class="sxs-lookup"><span data-stu-id="83e0b-196">Used when `groupId`, `userIds`, `peopleQueries` or no properties specified</span></span>|
|`presence`|<span data-ttu-id="83e0b-197">指定人员集状态</span><span class="sxs-lookup"><span data-stu-id="83e0b-197">Presence for the specified set of people</span></span>|<span data-ttu-id="83e0b-198">设置为 `showPresence` 时使用 `true`</span><span class="sxs-lookup"><span data-stu-id="83e0b-198">Used when `showPresence` set to `true`</span></span>|

> [!NOTE]
> <span data-ttu-id="83e0b-199">默认情况下， `mgt-people` 组件使用该 [`mgt-person`](./person.md) 组件来显示有关人员的信息。</span><span class="sxs-lookup"><span data-stu-id="83e0b-199">By default, the `mgt-people` component uses the [`mgt-person`](./person.md) component to display information about people.</span></span> <span data-ttu-id="83e0b-200">`mgt-person`组件自动下载并缓存每个人的照片。</span><span class="sxs-lookup"><span data-stu-id="83e0b-200">The `mgt-person` component automatically downloads and caches the photo for each person.</span></span>

<span data-ttu-id="83e0b-201">请参阅[Caching，](../customize-components/cache.md)了解有关如何配置缓存的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="83e0b-201">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="83e0b-202">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="83e0b-202">Extend for more control</span></span>

<span data-ttu-id="83e0b-203">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="83e0b-203">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="83e0b-204">方法</span><span class="sxs-lookup"><span data-stu-id="83e0b-204">Method</span></span> | <span data-ttu-id="83e0b-205">说明</span><span class="sxs-lookup"><span data-stu-id="83e0b-205">Description</span></span> |
| - | - |
| <span data-ttu-id="83e0b-206">renderLoading</span><span class="sxs-lookup"><span data-stu-id="83e0b-206">renderLoading</span></span> | <span data-ttu-id="83e0b-207">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="83e0b-207">Renders the loading state.</span></span> |
| <span data-ttu-id="83e0b-208">renderNoData</span><span class="sxs-lookup"><span data-stu-id="83e0b-208">renderNoData</span></span> | <span data-ttu-id="83e0b-209">呈现空数据状态。</span><span class="sxs-lookup"><span data-stu-id="83e0b-209">Renders the empty data state.</span></span> |
| <span data-ttu-id="83e0b-210">renderPeople</span><span class="sxs-lookup"><span data-stu-id="83e0b-210">renderPeople</span></span> | <span data-ttu-id="83e0b-211">呈现人员列表，最多呈现 `show-max` 值。</span><span class="sxs-lookup"><span data-stu-id="83e0b-211">Renders a list of people, up to the `show-max` value.</span></span> |
| <span data-ttu-id="83e0b-212">renderPerson</span><span class="sxs-lookup"><span data-stu-id="83e0b-212">renderPerson</span></span> | <span data-ttu-id="83e0b-213">呈现单个人员。</span><span class="sxs-lookup"><span data-stu-id="83e0b-213">Renders an individual person.</span></span> |
| <span data-ttu-id="83e0b-214">renderOverflow</span><span class="sxs-lookup"><span data-stu-id="83e0b-214">renderOverflow</span></span> | <span data-ttu-id="83e0b-215">呈现值以外的剩余人的 `show-max` 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83e0b-215">Renders a representation of remaining people beyond the `show-max` value.</span></span> |
