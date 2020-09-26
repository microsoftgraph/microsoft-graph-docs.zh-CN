---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: eca2ad4c0b56ff3475480a36eab2e943e3b6d9e4
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288614"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="deda5-103">Microsoft Graph 工具包中的人员选取器组件</span><span class="sxs-lookup"><span data-stu-id="deda5-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="deda5-104">您可以使用 `mgt-people-picker` web 组件搜索人员和/或组。</span><span class="sxs-lookup"><span data-stu-id="deda5-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="deda5-105">默认情况下，该组件将搜索组织中的所有人员和用户，但您也可以将该行为更改为同时搜索组或仅搜索组。</span><span class="sxs-lookup"><span data-stu-id="deda5-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="deda5-106">您还可以将搜索筛选到特定的组。</span><span class="sxs-lookup"><span data-stu-id="deda5-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="deda5-107">示例</span><span class="sxs-lookup"><span data-stu-id="deda5-107">Example</span></span>

<span data-ttu-id="deda5-108">下面的示例演示了该 `mgt-people-picker` 组件。</span><span class="sxs-lookup"><span data-stu-id="deda5-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="deda5-109">开始搜索名称以查看结果呈现，并使用代码编辑器查看 [属性](#properties) 如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="deda5-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="deda5-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="deda5-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="deda5-111">属性</span><span class="sxs-lookup"><span data-stu-id="deda5-111">Properties</span></span>

<span data-ttu-id="deda5-112">默认情况下， `mgt-people-picker` 组件从 `/me/people` 和 `/users` 终结点提取人员。</span><span class="sxs-lookup"><span data-stu-id="deda5-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="deda5-113">使用以下属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="deda5-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="deda5-114">属性</span><span class="sxs-lookup"><span data-stu-id="deda5-114">Attribute</span></span> | <span data-ttu-id="deda5-115">属性</span><span class="sxs-lookup"><span data-stu-id="deda5-115">Property</span></span> | <span data-ttu-id="deda5-116">说明</span><span class="sxs-lookup"><span data-stu-id="deda5-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="deda5-117">show-max</span><span class="sxs-lookup"><span data-stu-id="deda5-117">show-max</span></span> | <span data-ttu-id="deda5-118">showMax</span><span class="sxs-lookup"><span data-stu-id="deda5-118">showMax</span></span>   | <span data-ttu-id="deda5-119">一个指示要显示的最大用户数的数字值。</span><span class="sxs-lookup"><span data-stu-id="deda5-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="deda5-120">默认值为6。</span><span class="sxs-lookup"><span data-stu-id="deda5-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="deda5-121">组 id</span><span class="sxs-lookup"><span data-stu-id="deda5-121">group-id</span></span>    | <span data-ttu-id="deda5-122">groupId</span><span class="sxs-lookup"><span data-stu-id="deda5-122">groupId</span></span>     | <span data-ttu-id="deda5-123">一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="deda5-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="deda5-124">type</span><span class="sxs-lookup"><span data-stu-id="deda5-124">type</span></span>     | <span data-ttu-id="deda5-125">type</span><span class="sxs-lookup"><span data-stu-id="deda5-125">type</span></span>      | <span data-ttu-id="deda5-126">要搜索的实体的类型。</span><span class="sxs-lookup"><span data-stu-id="deda5-126">The type of entities to search for.</span></span> <span data-ttu-id="deda5-127">可用选项包括： `person` 、 `group` 、 `any` 。</span><span class="sxs-lookup"><span data-stu-id="deda5-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="deda5-128">默认值为 `person`。</span><span class="sxs-lookup"><span data-stu-id="deda5-128">Default value is `person`.</span></span> <span data-ttu-id="deda5-129">如果设置了属性，则此属性不起作用 `group-id` 。</span><span class="sxs-lookup"><span data-stu-id="deda5-129">This attribute has no effect if `group-id` property is set.</span></span>                                                                            |
| <span data-ttu-id="deda5-130">group 类型</span><span class="sxs-lookup"><span data-stu-id="deda5-130">group-type</span></span>     | <span data-ttu-id="deda5-131">groupType</span><span class="sxs-lookup"><span data-stu-id="deda5-131">groupType</span></span>      | <span data-ttu-id="deda5-132">要搜索的组类型。</span><span class="sxs-lookup"><span data-stu-id="deda5-132">The group type to search for.</span></span> <span data-ttu-id="deda5-133">可用选项包括： `unified` 、 `security` 、 `mailenabledsecurity` 、 `distribution` 、 `any` 。</span><span class="sxs-lookup"><span data-stu-id="deda5-133">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="deda5-134">默认值为 `any`。</span><span class="sxs-lookup"><span data-stu-id="deda5-134">Default value is `any`.</span></span> <span data-ttu-id="deda5-135">如果该 `type` 属性设置为，则此属性不起作用 `person` 。</span><span class="sxs-lookup"><span data-stu-id="deda5-135">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="deda5-136">选定-人员</span><span class="sxs-lookup"><span data-stu-id="deda5-136">selected-people</span></span>  | <span data-ttu-id="deda5-137">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="deda5-137">selectedPeople</span></span>     | <span data-ttu-id="deda5-138">选定人员的数组。</span><span class="sxs-lookup"><span data-stu-id="deda5-138">An array of selected people.</span></span> <span data-ttu-id="deda5-139">将此值设置为以编程方式选择人员。</span><span class="sxs-lookup"><span data-stu-id="deda5-139">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="deda5-140">people</span><span class="sxs-lookup"><span data-stu-id="deda5-140">people</span></span>   | <span data-ttu-id="deda5-141">people</span><span class="sxs-lookup"><span data-stu-id="deda5-141">people</span></span>    | <span data-ttu-id="deda5-142">在搜索结果中找到并呈现的人员的数组</span><span class="sxs-lookup"><span data-stu-id="deda5-142">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="deda5-143">默认选择的用户 id</span><span class="sxs-lookup"><span data-stu-id="deda5-143">default-selected-user-ids</span></span> | <span data-ttu-id="deda5-144">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="deda5-144">defaultSelectedUserIds</span></span> | <span data-ttu-id="deda5-145">当提供了以逗号分隔的 Microsoft Graph 用户 Id 的字符串时，组件将呈现在初始化时选择的各个用户。</span><span class="sxs-lookup"><span data-stu-id="deda5-145">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>

<span data-ttu-id="deda5-146">下面是一个 `show-max` 示例。</span><span class="sxs-lookup"><span data-stu-id="deda5-146">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="deda5-147">选定人员</span><span class="sxs-lookup"><span data-stu-id="deda5-147">Selected people</span></span>

<span data-ttu-id="deda5-148">组件的 "选定人员" 部分将呈现由开发人员或用户选择的每个人。</span><span class="sxs-lookup"><span data-stu-id="deda5-148">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![组织-人员-选取器](./images/selected-people.png)

<span data-ttu-id="deda5-150">您可以通过执行下列操作之一来填充所选的人员数据：</span><span class="sxs-lookup"><span data-stu-id="deda5-150">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="deda5-151">直接设置 `selectedPeople` 属性，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="deda5-151">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="deda5-152">使用此 `selectUsersById()` 方法可接受 Microsoft graph [用户 id](/graph/api/resources/users?view=graph-rest-1.0) 的数组，以查找有关所选内容的相关用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="deda5-152">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="deda5-153">**注意：** 如果找不到用户，则 `id` 不会为其呈现任何数据 `id` 。</span><span class="sxs-lookup"><span data-stu-id="deda5-153">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="deda5-154">活动</span><span class="sxs-lookup"><span data-stu-id="deda5-154">Events</span></span>

<span data-ttu-id="deda5-155">将从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="deda5-155">The following events are fired from the component.</span></span>

| <span data-ttu-id="deda5-156">事件</span><span class="sxs-lookup"><span data-stu-id="deda5-156">Event</span></span> | <span data-ttu-id="deda5-157">说明</span><span class="sxs-lookup"><span data-stu-id="deda5-157">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="deda5-158">用户在所选/选取的人员列表中添加或删除了人员。</span><span class="sxs-lookup"><span data-stu-id="deda5-158">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="deda5-159">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="deda5-159">CSS custom properties</span></span>

<span data-ttu-id="deda5-160">`mgt-people-picker`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="deda5-160">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-hover-color: #008394; /* input area border hover color */
    --input-focus-color: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a><span data-ttu-id="deda5-161">模板</span><span class="sxs-lookup"><span data-stu-id="deda5-161">Templates</span></span>

 <span data-ttu-id="deda5-162">`mgt-people-picker` 支持多个模板，这些 [模板](../templates.md) 可用于替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="deda5-162">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="deda5-163">若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="deda5-163">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="deda5-164">数据类型</span><span class="sxs-lookup"><span data-stu-id="deda5-164">Data type</span></span> | <span data-ttu-id="deda5-165">数据上下文</span><span class="sxs-lookup"><span data-stu-id="deda5-165">Data context</span></span> | <span data-ttu-id="deda5-166">说明</span><span class="sxs-lookup"><span data-stu-id="deda5-166">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="deda5-167">设置</span><span class="sxs-lookup"><span data-stu-id="deda5-167">default</span></span> | <span data-ttu-id="deda5-168">null：无数据</span><span class="sxs-lookup"><span data-stu-id="deda5-168">null: no data</span></span> | <span data-ttu-id="deda5-169">用于覆盖整个组件的呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="deda5-169">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="deda5-170">装载</span><span class="sxs-lookup"><span data-stu-id="deda5-170">loading</span></span> | <span data-ttu-id="deda5-171">null：无数据</span><span class="sxs-lookup"><span data-stu-id="deda5-171">null: no data</span></span> | <span data-ttu-id="deda5-172">在发出对 graph 的请求时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="deda5-172">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="deda5-173">error</span><span class="sxs-lookup"><span data-stu-id="deda5-173">error</span></span> | <span data-ttu-id="deda5-174">null：无数据</span><span class="sxs-lookup"><span data-stu-id="deda5-174">null: no data</span></span> | <span data-ttu-id="deda5-175">用户搜索不返回用户时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="deda5-175">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="deda5-176">无数据</span><span class="sxs-lookup"><span data-stu-id="deda5-176">no-data</span></span> | <span data-ttu-id="deda5-177">null：无数据</span><span class="sxs-lookup"><span data-stu-id="deda5-177">null: no data</span></span> | <span data-ttu-id="deda5-178">如果用户搜索不返回用户，则使用备用模板。</span><span class="sxs-lookup"><span data-stu-id="deda5-178">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="deda5-179">选定的人员</span><span class="sxs-lookup"><span data-stu-id="deda5-179">selected-person</span></span> | <span data-ttu-id="deda5-180">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="deda5-180">person: The person details object</span></span> | <span data-ttu-id="deda5-181">呈现所选人员的模板。</span><span class="sxs-lookup"><span data-stu-id="deda5-181">The template to render selected people.</span></span> |
| <span data-ttu-id="deda5-182">朋友</span><span class="sxs-lookup"><span data-stu-id="deda5-182">person</span></span> | <span data-ttu-id="deda5-183">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="deda5-183">person: The person details object</span></span> | <span data-ttu-id="deda5-184">用于在下拉列表中呈现人员的模板。</span><span class="sxs-lookup"><span data-stu-id="deda5-184">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="deda5-185">下面的示例演示如何使用 `error` 模板。</span><span class="sxs-lookup"><span data-stu-id="deda5-185">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="deda5-186">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="deda5-186">Microsoft Graph permissions</span></span>

<span data-ttu-id="deda5-187">此组件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="deda5-187">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="deda5-188">API</span><span class="sxs-lookup"><span data-stu-id="deda5-188">API</span></span>                                                                                                              | <span data-ttu-id="deda5-189">权限</span><span class="sxs-lookup"><span data-stu-id="deda5-189">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="deda5-190">/me/people</span><span class="sxs-lookup"><span data-stu-id="deda5-190">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="deda5-191">People.Read</span><span class="sxs-lookup"><span data-stu-id="deda5-191">People.Read</span></span>        |
| [<span data-ttu-id="deda5-192">/users</span><span class="sxs-lookup"><span data-stu-id="deda5-192">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0)  | <span data-ttu-id="deda5-193">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="deda5-193">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="deda5-194">/groups</span><span class="sxs-lookup"><span data-stu-id="deda5-194">/groups</span></span>](/group-list?view=graph-rest-beta)  | <span data-ttu-id="deda5-195">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="deda5-195">Group.Read.All</span></span> |
| [<span data-ttu-id="deda5-196">/groups/ \$ {groupId}/members</span><span class="sxs-lookup"><span data-stu-id="deda5-196">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="deda5-197">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="deda5-197">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="deda5-198">/users/$ {userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="deda5-198">/users/${userPrincipleName} </span></span>](/graph/api/user-get?view=graph-rest-1.0)  | <span data-ttu-id="deda5-199">User.Read</span><span class="sxs-lookup"><span data-stu-id="deda5-199">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="deda5-200">身份验证</span><span class="sxs-lookup"><span data-stu-id="deda5-200">Authentication</span></span>

<span data-ttu-id="deda5-201">该控件使用 [身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="deda5-201">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="deda5-202">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="deda5-202">Extend for more control</span></span>

<span data-ttu-id="deda5-203">对于更复杂的方案或真正的自定义 UX，此组件将公开几种 `protected render*` 用于在组件扩展中进行重写的方法。</span><span class="sxs-lookup"><span data-stu-id="deda5-203">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="deda5-204">方法</span><span class="sxs-lookup"><span data-stu-id="deda5-204">Method</span></span> | <span data-ttu-id="deda5-205">说明</span><span class="sxs-lookup"><span data-stu-id="deda5-205">Description</span></span> |
| - | - |
| <span data-ttu-id="deda5-206">renderInput</span><span class="sxs-lookup"><span data-stu-id="deda5-206">renderInput</span></span> | <span data-ttu-id="deda5-207">呈现输入文本框。</span><span class="sxs-lookup"><span data-stu-id="deda5-207">Renders the input text box.</span></span> |
| <span data-ttu-id="deda5-208">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="deda5-208">renderSelectedPeople</span></span> | <span data-ttu-id="deda5-209">呈现所选人员标记。</span><span class="sxs-lookup"><span data-stu-id="deda5-209">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="deda5-210">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="deda5-210">renderSelectedPerson</span></span> | <span data-ttu-id="deda5-211">呈现单个人员标记。</span><span class="sxs-lookup"><span data-stu-id="deda5-211">Renders an individual person token.</span></span> |
| <span data-ttu-id="deda5-212">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="deda5-212">renderFlyout</span></span> | <span data-ttu-id="deda5-213">呈现浮出控件的镶边。</span><span class="sxs-lookup"><span data-stu-id="deda5-213">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="deda5-214">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="deda5-214">renderFlyoutContent</span></span> | <span data-ttu-id="deda5-215">在 "结果" 浮出控件中呈现适当的状态。</span><span class="sxs-lookup"><span data-stu-id="deda5-215">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="deda5-216">renderLoading</span><span class="sxs-lookup"><span data-stu-id="deda5-216">renderLoading</span></span> | <span data-ttu-id="deda5-217">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="deda5-217">Renders the loading state.</span></span> |
| <span data-ttu-id="deda5-218">renderNoData</span><span class="sxs-lookup"><span data-stu-id="deda5-218">renderNoData</span></span> | <span data-ttu-id="deda5-219">在未找到搜索查询的结果时呈现状态。</span><span class="sxs-lookup"><span data-stu-id="deda5-219">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="deda5-220">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="deda5-220">renderSearchResults</span></span> | <span data-ttu-id="deda5-221">呈现搜索结果的列表。</span><span class="sxs-lookup"><span data-stu-id="deda5-221">Renders the list of search results.</span></span> |
| <span data-ttu-id="deda5-222">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="deda5-222">renderPersonResult</span></span> | <span data-ttu-id="deda5-223">呈现单个个人的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="deda5-223">Renders an individual person search result.</span></span> |