---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: bdfb4951151876d79dede974654747d25a54c833
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510880"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="3d6c5-103">Microsoft Graph 工具包中的人员选取器组件</span><span class="sxs-lookup"><span data-stu-id="3d6c5-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="3d6c5-104">您可以使用`mgt-people-picker` web 组件搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-104">You can use the `mgt-people-picker` web component search for a specified number of people and render the list of results via Microsoft Graph.</span></span> <span data-ttu-id="3d6c5-105">默认情况下，组件将搜索所有人员;您还可以定义组属性以进一步筛选结果。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-105">By default, the component will search for all people; you can also define a group property to further filter the results.</span></span>

<span data-ttu-id="3d6c5-106">如果要显示的用户数超过此`show-max`值，则不会在搜索列表中显示所有返回的人员数。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-106">If the number of people to display exceeds the `show-max` value, not all people returned will be displayed in the search list.</span></span>

## <a name="example"></a><span data-ttu-id="3d6c5-107">示例</span><span class="sxs-lookup"><span data-stu-id="3d6c5-107">Example</span></span>

<span data-ttu-id="3d6c5-108">下面的示例演示了`mgt-people-picker`该组件。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="3d6c5-109">开始搜索名称以查看结果呈现，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="3d6c5-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="3d6c5-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="3d6c5-111">属性</span><span class="sxs-lookup"><span data-stu-id="3d6c5-111">Properties</span></span>

<span data-ttu-id="3d6c5-112">默认情况下， `mgt-people-picker`组件从`/me/people`终结点中提取人员。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` endpoint.</span></span> <span data-ttu-id="3d6c5-113">使用以下属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="3d6c5-114">属性</span><span class="sxs-lookup"><span data-stu-id="3d6c5-114">Attribute</span></span> | <span data-ttu-id="3d6c5-115">属性</span><span class="sxs-lookup"><span data-stu-id="3d6c5-115">Property</span></span> | <span data-ttu-id="3d6c5-116">说明</span><span class="sxs-lookup"><span data-stu-id="3d6c5-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3d6c5-117">show-max</span><span class="sxs-lookup"><span data-stu-id="3d6c5-117">show-max</span></span> | <span data-ttu-id="3d6c5-118">showMax</span><span class="sxs-lookup"><span data-stu-id="3d6c5-118">showMax</span></span>   | <span data-ttu-id="3d6c5-119">一个指示要显示的最大用户数的数字值。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="3d6c5-120">默认值为6。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="3d6c5-121">people</span><span class="sxs-lookup"><span data-stu-id="3d6c5-121">people</span></span>   | <span data-ttu-id="3d6c5-122">people</span><span class="sxs-lookup"><span data-stu-id="3d6c5-122">people</span></span>    | <span data-ttu-id="3d6c5-123">获取或设置组件呈现的人员列表的人员数组。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-123">An array of people to get or set the list of people rendered by the component.</span></span> <span data-ttu-id="3d6c5-124">使用此属性可访问组件加载的人员。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-124">Use this property to access the people loaded by the component.</span></span> <span data-ttu-id="3d6c5-125">设置此值可加载自己的人员。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-125">Set this value to load your own people.</span></span> |
| <span data-ttu-id="3d6c5-126">group</span><span class="sxs-lookup"><span data-stu-id="3d6c5-126">group</span></span>    | <span data-ttu-id="3d6c5-127">group</span><span class="sxs-lookup"><span data-stu-id="3d6c5-127">group</span></span>     | <span data-ttu-id="3d6c5-128">一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-128">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
|  <span data-ttu-id="3d6c5-129">选定-人员</span><span class="sxs-lookup"><span data-stu-id="3d6c5-129">selected-people</span></span>  | <span data-ttu-id="3d6c5-130">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="3d6c5-130">selectedPeople</span></span>     | <span data-ttu-id="3d6c5-131">一个类型`person`的数组，表示在组件中选定的人员。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-131">An array of type  `person`, representing people selected in the component.</span></span> <span data-ttu-id="3d6c5-132">将此值设置为 "默认情况下选择所选人员"。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-132">Set this value to choose selected people by default.</span></span>|

<span data-ttu-id="3d6c5-133">下面是一个`show-max`示例。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-133">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="3d6c5-134">选定人员</span><span class="sxs-lookup"><span data-stu-id="3d6c5-134">Selected people</span></span>

<span data-ttu-id="3d6c5-135">组件的 "选定人员" 部分将呈现由开发人员或用户选择的每个人。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-135">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![组织-人员-选取器](./images/selected-people.png)

<span data-ttu-id="3d6c5-137">您可以通过执行下列操作之一来填充所选的人员数据：</span><span class="sxs-lookup"><span data-stu-id="3d6c5-137">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="3d6c5-138">直接设置`selectedPeople`属性，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-138">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="3d6c5-139">使用此`selectUsersById()`方法可接受 Microsoft graph[用户 id](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0)的数组，以查找有关所选内容的相关用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-139">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="3d6c5-140">**注意：** 如果找不到用户，则`id`不会为其呈现任何数据`id`。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-140">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="3d6c5-141">活动</span><span class="sxs-lookup"><span data-stu-id="3d6c5-141">Events</span></span>

<span data-ttu-id="3d6c5-142">将从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-142">The following events are fired from the component.</span></span>

| <span data-ttu-id="3d6c5-143">事件</span><span class="sxs-lookup"><span data-stu-id="3d6c5-143">Event</span></span> | <span data-ttu-id="3d6c5-144">说明</span><span class="sxs-lookup"><span data-stu-id="3d6c5-144">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="3d6c5-145">用户在所选/选取的人员列表中添加或删除了人员。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-145">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="3d6c5-146">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="3d6c5-146">CSS custom properties</span></span>

<span data-ttu-id="3d6c5-147">`mgt-people-picker`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-147">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
  --people-list-background-color: blue; /* Background-color for people under search */
  --accent-color: green; /* Color for separator of search input box and people */
}
```

## <a name="templates"></a><span data-ttu-id="3d6c5-148">模板</span><span class="sxs-lookup"><span data-stu-id="3d6c5-148">Templates</span></span>

 <span data-ttu-id="3d6c5-149">`mgt-people-picker`支持多个模板，这些[模板](../templates.md)可用于替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-149">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="3d6c5-150">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-150">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="3d6c5-151">数据类型</span><span class="sxs-lookup"><span data-stu-id="3d6c5-151">Data type</span></span> | <span data-ttu-id="3d6c5-152">数据上下文</span><span class="sxs-lookup"><span data-stu-id="3d6c5-152">Data context</span></span> | <span data-ttu-id="3d6c5-153">说明</span><span class="sxs-lookup"><span data-stu-id="3d6c5-153">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="3d6c5-154"> 默认值</span><span class="sxs-lookup"><span data-stu-id="3d6c5-154">default</span></span> | <span data-ttu-id="3d6c5-155">null：无数据</span><span class="sxs-lookup"><span data-stu-id="3d6c5-155">null: no data</span></span> | <span data-ttu-id="3d6c5-156">用于覆盖整个组件的呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-156">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="3d6c5-157">装载</span><span class="sxs-lookup"><span data-stu-id="3d6c5-157">loading</span></span> | <span data-ttu-id="3d6c5-158">null：无数据</span><span class="sxs-lookup"><span data-stu-id="3d6c5-158">null: no data</span></span> | <span data-ttu-id="3d6c5-159">在发出对 graph 的请求时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-159">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="3d6c5-160">error</span><span class="sxs-lookup"><span data-stu-id="3d6c5-160">error</span></span> | <span data-ttu-id="3d6c5-161">null：无数据</span><span class="sxs-lookup"><span data-stu-id="3d6c5-161">null: no data</span></span> | <span data-ttu-id="3d6c5-162">用户搜索不返回用户时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-162">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="3d6c5-163">无数据</span><span class="sxs-lookup"><span data-stu-id="3d6c5-163">no-data</span></span> | <span data-ttu-id="3d6c5-164">null：无数据</span><span class="sxs-lookup"><span data-stu-id="3d6c5-164">null: no data</span></span> | <span data-ttu-id="3d6c5-165">如果用户搜索不返回用户，则使用备用模板。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-165">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="3d6c5-166">选定的人员</span><span class="sxs-lookup"><span data-stu-id="3d6c5-166">selected-person</span></span> | <span data-ttu-id="3d6c5-167">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="3d6c5-167">person: The person details object</span></span> | <span data-ttu-id="3d6c5-168">呈现所选人员的模板。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-168">The template to render selected people.</span></span> |
| <span data-ttu-id="3d6c5-169">朋友</span><span class="sxs-lookup"><span data-stu-id="3d6c5-169">person</span></span> | <span data-ttu-id="3d6c5-170">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="3d6c5-170">person: The person details object</span></span> | <span data-ttu-id="3d6c5-171">用于在下拉列表中呈现人员的模板。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-171">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="3d6c5-172">下面的示例演示如何使用`error`模板。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-172">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="3d6c5-173">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="3d6c5-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="3d6c5-174">此组件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-174">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="3d6c5-175">API</span><span class="sxs-lookup"><span data-stu-id="3d6c5-175">API</span></span>                                                                                                              | <span data-ttu-id="3d6c5-176">权限</span><span class="sxs-lookup"><span data-stu-id="3d6c5-176">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="3d6c5-177">/me/people</span><span class="sxs-lookup"><span data-stu-id="3d6c5-177">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="3d6c5-178">People.Read</span><span class="sxs-lookup"><span data-stu-id="3d6c5-178">People.Read</span></span>        |
| [<span data-ttu-id="3d6c5-179">/groups/\${groupId}/members</span><span class="sxs-lookup"><span data-stu-id="3d6c5-179">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="3d6c5-180">People.Read</span><span class="sxs-lookup"><span data-stu-id="3d6c5-180">People.Read</span></span>        |
| [<span data-ttu-id="3d6c5-181">/users/$ {userPrincipleName}</span><span class="sxs-lookup"><span data-stu-id="3d6c5-181">/users/${userPrincipleName} </span></span>](/graph/api/user-list-people?view=graph-rest-1.0)  | <span data-ttu-id="3d6c5-182">User.readbasic.all</span><span class="sxs-lookup"><span data-stu-id="3d6c5-182">User.Readbasic.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="3d6c5-183">身份验证</span><span class="sxs-lookup"><span data-stu-id="3d6c5-183">Authentication</span></span>

<span data-ttu-id="3d6c5-184">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-184">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="3d6c5-185">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="3d6c5-185">Extend for more control</span></span>

<span data-ttu-id="3d6c5-186">对于更复杂的方案或真正的自定义 UX，此组件`protected render*`将公开几种用于在组件扩展中进行重写的方法。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-186">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="3d6c5-187">方法</span><span class="sxs-lookup"><span data-stu-id="3d6c5-187">Method</span></span> | <span data-ttu-id="3d6c5-188">说明</span><span class="sxs-lookup"><span data-stu-id="3d6c5-188">Description</span></span> |
| - | - |
| <span data-ttu-id="3d6c5-189">renderInput</span><span class="sxs-lookup"><span data-stu-id="3d6c5-189">renderInput</span></span> | <span data-ttu-id="3d6c5-190">呈现输入文本框。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-190">Renders the input text box.</span></span> |
| <span data-ttu-id="3d6c5-191">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="3d6c5-191">renderSelectedPeople</span></span> | <span data-ttu-id="3d6c5-192">呈现所选人员标记。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-192">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="3d6c5-193">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="3d6c5-193">renderSelectedPerson</span></span> | <span data-ttu-id="3d6c5-194">呈现单个人员标记。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-194">Renders an individual person token.</span></span> |
| <span data-ttu-id="3d6c5-195">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="3d6c5-195">renderFlyout</span></span> | <span data-ttu-id="3d6c5-196">呈现浮出控件的镶边。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-196">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="3d6c5-197">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="3d6c5-197">renderFlyoutContent</span></span> | <span data-ttu-id="3d6c5-198">在 "结果" 浮出控件中呈现适当的状态。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-198">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="3d6c5-199">renderLoading</span><span class="sxs-lookup"><span data-stu-id="3d6c5-199">renderLoading</span></span> | <span data-ttu-id="3d6c5-200">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-200">Renders the loading state.</span></span> |
| <span data-ttu-id="3d6c5-201">renderNoData</span><span class="sxs-lookup"><span data-stu-id="3d6c5-201">renderNoData</span></span> | <span data-ttu-id="3d6c5-202">在未找到搜索查询的结果时呈现状态。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-202">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="3d6c5-203">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="3d6c5-203">renderSearchResults</span></span> | <span data-ttu-id="3d6c5-204">呈现搜索结果的列表。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-204">Renders the list of search results.</span></span> |
| <span data-ttu-id="3d6c5-205">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="3d6c5-205">renderPersonResult</span></span> | <span data-ttu-id="3d6c5-206">呈现单个个人的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="3d6c5-206">Renders an individual person search result.</span></span> |
