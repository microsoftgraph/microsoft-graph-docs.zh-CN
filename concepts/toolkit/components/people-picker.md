---
title: 人员-选取器组件
description: 您可以使用 "人员-选取器 web 组件" 搜索指定数量的人员，并通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: e3e656c6aef0ab2af9878fb3e4738ade912c4685
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681884"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="e5f42-103">Microsoft Graph 工具包中的人员选取器组件</span><span class="sxs-lookup"><span data-stu-id="e5f42-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="e5f42-104">您可以使用 `mgt-people-picker` web 组件搜索人员和/或组。</span><span class="sxs-lookup"><span data-stu-id="e5f42-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="e5f42-105">默认情况下，该组件将搜索组织中的所有人员和用户，但您也可以将该行为更改为同时搜索组或仅搜索组。</span><span class="sxs-lookup"><span data-stu-id="e5f42-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="e5f42-106">您还可以将搜索筛选到特定的组。</span><span class="sxs-lookup"><span data-stu-id="e5f42-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="e5f42-107">示例</span><span class="sxs-lookup"><span data-stu-id="e5f42-107">Example</span></span>

<span data-ttu-id="e5f42-108">下面的示例演示了该 `mgt-people-picker` 组件。</span><span class="sxs-lookup"><span data-stu-id="e5f42-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="e5f42-109">开始搜索名称以查看结果呈现，并使用代码编辑器查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="e5f42-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="e5f42-110">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="e5f42-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="e5f42-111">属性</span><span class="sxs-lookup"><span data-stu-id="e5f42-111">Properties</span></span>

<span data-ttu-id="e5f42-112">默认情况下， `mgt-people-picker` 组件从 `/me/people` 和 `/users` 终结点提取人员。</span><span class="sxs-lookup"><span data-stu-id="e5f42-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="e5f42-113">使用以下属性来更改此行为。</span><span class="sxs-lookup"><span data-stu-id="e5f42-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="e5f42-114">属性</span><span class="sxs-lookup"><span data-stu-id="e5f42-114">Attribute</span></span> | <span data-ttu-id="e5f42-115">属性</span><span class="sxs-lookup"><span data-stu-id="e5f42-115">Property</span></span> | <span data-ttu-id="e5f42-116">说明</span><span class="sxs-lookup"><span data-stu-id="e5f42-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e5f42-117">show-max</span><span class="sxs-lookup"><span data-stu-id="e5f42-117">show-max</span></span> | <span data-ttu-id="e5f42-118">showMax</span><span class="sxs-lookup"><span data-stu-id="e5f42-118">showMax</span></span>   | <span data-ttu-id="e5f42-119">一个指示要显示的最大用户数的数字值。</span><span class="sxs-lookup"><span data-stu-id="e5f42-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="e5f42-120">默认值为6。</span><span class="sxs-lookup"><span data-stu-id="e5f42-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="e5f42-121">组 id</span><span class="sxs-lookup"><span data-stu-id="e5f42-121">group-id</span></span>    | <span data-ttu-id="e5f42-122">groupId</span><span class="sxs-lookup"><span data-stu-id="e5f42-122">groupId</span></span>     | <span data-ttu-id="e5f42-123">一个 string 值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="e5f42-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="e5f42-124">type</span><span class="sxs-lookup"><span data-stu-id="e5f42-124">type</span></span>     | <span data-ttu-id="e5f42-125">type</span><span class="sxs-lookup"><span data-stu-id="e5f42-125">type</span></span>      | <span data-ttu-id="e5f42-126">要搜索的实体的类型。</span><span class="sxs-lookup"><span data-stu-id="e5f42-126">The type of entities to search for.</span></span> <span data-ttu-id="e5f42-127">可用选项包括： `person` 、 `group` 、 `any` 。</span><span class="sxs-lookup"><span data-stu-id="e5f42-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="e5f42-128">默认值为 `person`。</span><span class="sxs-lookup"><span data-stu-id="e5f42-128">Default value is `person`.</span></span> <span data-ttu-id="e5f42-129">如果设置了属性，则此属性不起作用 `group-id` 。</span><span class="sxs-lookup"><span data-stu-id="e5f42-129">This attribute has no effect if `group-id` property is set.</span></span>                                                                            |
| <span data-ttu-id="e5f42-130">group 类型</span><span class="sxs-lookup"><span data-stu-id="e5f42-130">group-type</span></span>     | <span data-ttu-id="e5f42-131">groupType</span><span class="sxs-lookup"><span data-stu-id="e5f42-131">groupType</span></span>      | <span data-ttu-id="e5f42-132">要搜索的组类型。</span><span class="sxs-lookup"><span data-stu-id="e5f42-132">The group type to search for.</span></span> <span data-ttu-id="e5f42-133">可用选项包括： `unified` 、 `security` 、 `mailenabledsecurity` 、 `distribution` 、 `any` 。</span><span class="sxs-lookup"><span data-stu-id="e5f42-133">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="e5f42-134">默认值为 `any`。</span><span class="sxs-lookup"><span data-stu-id="e5f42-134">Default value is `any`.</span></span> <span data-ttu-id="e5f42-135">如果该 `type` 属性设置为，则此属性不起作用 `person` 。</span><span class="sxs-lookup"><span data-stu-id="e5f42-135">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="e5f42-136">选定-人员</span><span class="sxs-lookup"><span data-stu-id="e5f42-136">selected-people</span></span>  | <span data-ttu-id="e5f42-137">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="e5f42-137">selectedPeople</span></span>     | <span data-ttu-id="e5f42-138">选定人员的数组。</span><span class="sxs-lookup"><span data-stu-id="e5f42-138">An array of selected people.</span></span> <span data-ttu-id="e5f42-139">将此值设置为以编程方式选择人员。</span><span class="sxs-lookup"><span data-stu-id="e5f42-139">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="e5f42-140">people</span><span class="sxs-lookup"><span data-stu-id="e5f42-140">people</span></span>   | <span data-ttu-id="e5f42-141">people</span><span class="sxs-lookup"><span data-stu-id="e5f42-141">people</span></span>    | <span data-ttu-id="e5f42-142">在搜索结果中找到并呈现的人员的数组</span><span class="sxs-lookup"><span data-stu-id="e5f42-142">An array of people found and rendered in the search result</span></span> |

<span data-ttu-id="e5f42-143">下面是一个 `show-max` 示例。</span><span class="sxs-lookup"><span data-stu-id="e5f42-143">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="e5f42-144">选定人员</span><span class="sxs-lookup"><span data-stu-id="e5f42-144">Selected people</span></span>

<span data-ttu-id="e5f42-145">组件的 "选定人员" 部分将呈现由开发人员或用户选择的每个人。</span><span class="sxs-lookup"><span data-stu-id="e5f42-145">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![组织-人员-选取器](./images/selected-people.png)

<span data-ttu-id="e5f42-147">您可以通过执行下列操作之一来填充所选的人员数据：</span><span class="sxs-lookup"><span data-stu-id="e5f42-147">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="e5f42-148">直接设置 `selectedPeople` 属性，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="e5f42-148">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="e5f42-149">使用此 `selectUsersById()` 方法可接受 Microsoft graph[用户 id](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0)的数组，以查找有关所选内容的相关用户详细信息。</span><span class="sxs-lookup"><span data-stu-id="e5f42-149">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](https://docs.microsoft.com/graph/api/resources/users?view=graph-rest-1.0) to find associated user details for selection.</span></span>

     ><span data-ttu-id="e5f42-150">**注意：** 如果找不到用户，则 `id` 不会为其呈现任何数据 `id` 。</span><span class="sxs-lookup"><span data-stu-id="e5f42-150">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Mirosoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="e5f42-151">活动</span><span class="sxs-lookup"><span data-stu-id="e5f42-151">Events</span></span>

<span data-ttu-id="e5f42-152">将从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="e5f42-152">The following events are fired from the component.</span></span>

| <span data-ttu-id="e5f42-153">事件</span><span class="sxs-lookup"><span data-stu-id="e5f42-153">Event</span></span> | <span data-ttu-id="e5f42-154">说明</span><span class="sxs-lookup"><span data-stu-id="e5f42-154">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="e5f42-155">用户在所选/选取的人员列表中添加或删除了人员。</span><span class="sxs-lookup"><span data-stu-id="e5f42-155">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="e5f42-156">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="e5f42-156">CSS custom properties</span></span>

<span data-ttu-id="e5f42-157">`mgt-people-picker`组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="e5f42-157">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

    --font-color: white; /* input area border focus color */
    --placeholder-default-color: #f1f1f1; /* placeholder text color default*/
    --placeholder-focus-color: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a><span data-ttu-id="e5f42-158">模板</span><span class="sxs-lookup"><span data-stu-id="e5f42-158">Templates</span></span>

 <span data-ttu-id="e5f42-159">`mgt-people-picker`支持多个模板，这些[模板](../templates.md)可用于替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="e5f42-159">`mgt-people-picker` supports several [templates](../templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="e5f42-160">若要指定模板，请在 `<template>` 组件内添加一个元素，并将 `data-type` 值设置为下列值之一。</span><span class="sxs-lookup"><span data-stu-id="e5f42-160">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="e5f42-161">数据类型</span><span class="sxs-lookup"><span data-stu-id="e5f42-161">Data type</span></span> | <span data-ttu-id="e5f42-162">数据上下文</span><span class="sxs-lookup"><span data-stu-id="e5f42-162">Data context</span></span> | <span data-ttu-id="e5f42-163">Description</span><span class="sxs-lookup"><span data-stu-id="e5f42-163">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="e5f42-164"> 默认值</span><span class="sxs-lookup"><span data-stu-id="e5f42-164">default</span></span> | <span data-ttu-id="e5f42-165">null：无数据</span><span class="sxs-lookup"><span data-stu-id="e5f42-165">null: no data</span></span> | <span data-ttu-id="e5f42-166">用于覆盖整个组件的呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="e5f42-166">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="e5f42-167">装载</span><span class="sxs-lookup"><span data-stu-id="e5f42-167">loading</span></span> | <span data-ttu-id="e5f42-168">null：无数据</span><span class="sxs-lookup"><span data-stu-id="e5f42-168">null: no data</span></span> | <span data-ttu-id="e5f42-169">在发出对 graph 的请求时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="e5f42-169">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="e5f42-170">error</span><span class="sxs-lookup"><span data-stu-id="e5f42-170">error</span></span> | <span data-ttu-id="e5f42-171">null：无数据</span><span class="sxs-lookup"><span data-stu-id="e5f42-171">null: no data</span></span> | <span data-ttu-id="e5f42-172">用户搜索不返回用户时使用的模板。</span><span class="sxs-lookup"><span data-stu-id="e5f42-172">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="e5f42-173">无数据</span><span class="sxs-lookup"><span data-stu-id="e5f42-173">no-data</span></span> | <span data-ttu-id="e5f42-174">null：无数据</span><span class="sxs-lookup"><span data-stu-id="e5f42-174">null: no data</span></span> | <span data-ttu-id="e5f42-175">如果用户搜索不返回用户，则使用备用模板。</span><span class="sxs-lookup"><span data-stu-id="e5f42-175">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="e5f42-176">选定的人员</span><span class="sxs-lookup"><span data-stu-id="e5f42-176">selected-person</span></span> | <span data-ttu-id="e5f42-177">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="e5f42-177">person: The person details object</span></span> | <span data-ttu-id="e5f42-178">呈现所选人员的模板。</span><span class="sxs-lookup"><span data-stu-id="e5f42-178">The template to render selected people.</span></span> |
| <span data-ttu-id="e5f42-179">朋友</span><span class="sxs-lookup"><span data-stu-id="e5f42-179">person</span></span> | <span data-ttu-id="e5f42-180">人员：人员详细信息对象</span><span class="sxs-lookup"><span data-stu-id="e5f42-180">person: The person details object</span></span> | <span data-ttu-id="e5f42-181">用于在下拉列表中呈现人员的模板。</span><span class="sxs-lookup"><span data-stu-id="e5f42-181">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="e5f42-182">下面的示例演示如何使用 `error` 模板。</span><span class="sxs-lookup"><span data-stu-id="e5f42-182">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="e5f42-183">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="e5f42-183">Microsoft Graph permissions</span></span>

<span data-ttu-id="e5f42-184">此组件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="e5f42-184">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="e5f42-185">API</span><span class="sxs-lookup"><span data-stu-id="e5f42-185">API</span></span>                                                                                                              | <span data-ttu-id="e5f42-186">Permission</span><span class="sxs-lookup"><span data-stu-id="e5f42-186">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="e5f42-187">/me/people</span><span class="sxs-lookup"><span data-stu-id="e5f42-187">/me/people</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)                    | <span data-ttu-id="e5f42-188">People.Read</span><span class="sxs-lookup"><span data-stu-id="e5f42-188">People.Read</span></span>        |
| [<span data-ttu-id="e5f42-189">/users</span><span class="sxs-lookup"><span data-stu-id="e5f42-189">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0)  | <span data-ttu-id="e5f42-190">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e5f42-190">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="e5f42-191">/groups</span><span class="sxs-lookup"><span data-stu-id="e5f42-191">/groups</span></span>](/group-list?view=graph-rest-beta)  | <span data-ttu-id="e5f42-192">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5f42-192">Group.Read.All</span></span> |
| [<span data-ttu-id="e5f42-193">/groups/ \$ {groupId}/members</span><span class="sxs-lookup"><span data-stu-id="e5f42-193">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members?view=graph-rest-1.0) | <span data-ttu-id="e5f42-194">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e5f42-194">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="e5f42-195">/users/$ {userPrincipleName}</span><span class="sxs-lookup"><span data-stu-id="e5f42-195">/users/${userPrincipleName} </span></span>](/graph/api/user-get?view=graph-rest-1.0)  | <span data-ttu-id="e5f42-196">User.Read</span><span class="sxs-lookup"><span data-stu-id="e5f42-196">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="e5f42-197">身份验证</span><span class="sxs-lookup"><span data-stu-id="e5f42-197">Authentication</span></span>

<span data-ttu-id="e5f42-198">该控件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="e5f42-198">The control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="e5f42-199">扩展以实现更多控制</span><span class="sxs-lookup"><span data-stu-id="e5f42-199">Extend for more control</span></span>

<span data-ttu-id="e5f42-200">对于更复杂的方案或真正的自定义 UX，此组件将公开几种 `protected render*` 用于在组件扩展中进行重写的方法。</span><span class="sxs-lookup"><span data-stu-id="e5f42-200">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="e5f42-201">方法</span><span class="sxs-lookup"><span data-stu-id="e5f42-201">Method</span></span> | <span data-ttu-id="e5f42-202">说明</span><span class="sxs-lookup"><span data-stu-id="e5f42-202">Description</span></span> |
| - | - |
| <span data-ttu-id="e5f42-203">renderInput</span><span class="sxs-lookup"><span data-stu-id="e5f42-203">renderInput</span></span> | <span data-ttu-id="e5f42-204">呈现输入文本框。</span><span class="sxs-lookup"><span data-stu-id="e5f42-204">Renders the input text box.</span></span> |
| <span data-ttu-id="e5f42-205">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="e5f42-205">renderSelectedPeople</span></span> | <span data-ttu-id="e5f42-206">呈现所选人员标记。</span><span class="sxs-lookup"><span data-stu-id="e5f42-206">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="e5f42-207">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="e5f42-207">renderSelectedPerson</span></span> | <span data-ttu-id="e5f42-208">呈现单个人员标记。</span><span class="sxs-lookup"><span data-stu-id="e5f42-208">Renders an individual person token.</span></span> |
| <span data-ttu-id="e5f42-209">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="e5f42-209">renderFlyout</span></span> | <span data-ttu-id="e5f42-210">呈现浮出控件的镶边。</span><span class="sxs-lookup"><span data-stu-id="e5f42-210">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="e5f42-211">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="e5f42-211">renderFlyoutContent</span></span> | <span data-ttu-id="e5f42-212">在 "结果" 浮出控件中呈现适当的状态。</span><span class="sxs-lookup"><span data-stu-id="e5f42-212">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="e5f42-213">renderLoading</span><span class="sxs-lookup"><span data-stu-id="e5f42-213">renderLoading</span></span> | <span data-ttu-id="e5f42-214">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="e5f42-214">Renders the loading state.</span></span> |
| <span data-ttu-id="e5f42-215">renderNoData</span><span class="sxs-lookup"><span data-stu-id="e5f42-215">renderNoData</span></span> | <span data-ttu-id="e5f42-216">在未找到搜索查询的结果时呈现状态。</span><span class="sxs-lookup"><span data-stu-id="e5f42-216">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="e5f42-217">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="e5f42-217">renderSearchResults</span></span> | <span data-ttu-id="e5f42-218">呈现搜索结果的列表。</span><span class="sxs-lookup"><span data-stu-id="e5f42-218">Renders the list of search results.</span></span> |
| <span data-ttu-id="e5f42-219">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="e5f42-219">renderPersonResult</span></span> | <span data-ttu-id="e5f42-220">呈现单个个人的搜索结果。</span><span class="sxs-lookup"><span data-stu-id="e5f42-220">Renders an individual person search result.</span></span> |
