---
title: People-Picker组件
description: 您可以使用 mgt-people-picker Web 组件搜索指定数量的人，然后通过 Microsoft Graph。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 36a8208b2425bc74922427f7ffcb4c6ec3a10788
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780741"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="793b3-103">People-Picker Microsoft Graph Toolkit 中的组件</span><span class="sxs-lookup"><span data-stu-id="793b3-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="793b3-104">您可以使用 Web `mgt-people-picker` 组件来搜索用户和/或组。</span><span class="sxs-lookup"><span data-stu-id="793b3-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="793b3-105">默认情况下，组件将搜索组织中所有的用户和用户，但你可以将行为更改为同时搜索组或仅搜索组。</span><span class="sxs-lookup"><span data-stu-id="793b3-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="793b3-106">您还可以将搜索筛选到特定组。</span><span class="sxs-lookup"><span data-stu-id="793b3-106">You can also filter the search to a specific group.</span></span> <span data-ttu-id="793b3-107">此外，还可以允许用户输入并选择任何电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="793b3-107">Additionally, you can allow the user to enter and select any email address.</span></span>

## <a name="example"></a><span data-ttu-id="793b3-108">示例</span><span class="sxs-lookup"><span data-stu-id="793b3-108">Example</span></span>

<span data-ttu-id="793b3-109">以下示例显示 `mgt-people-picker` 组件。</span><span class="sxs-lookup"><span data-stu-id="793b3-109">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="793b3-110">开始搜索名称以查看结果呈现，并使用代码编辑器查看属性 [如何更改组件](#properties) 的行为。</span><span class="sxs-lookup"><span data-stu-id="793b3-110">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="793b3-111">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="793b3-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="793b3-112">属性</span><span class="sxs-lookup"><span data-stu-id="793b3-112">Properties</span></span>

<span data-ttu-id="793b3-113">默认情况下， `mgt-people-picker` 组件从 和 终结点 `/me/people` 提取 `/users` 人员。</span><span class="sxs-lookup"><span data-stu-id="793b3-113">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="793b3-114">使用以下属性更改此行为。</span><span class="sxs-lookup"><span data-stu-id="793b3-114">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="793b3-115">属性</span><span class="sxs-lookup"><span data-stu-id="793b3-115">Attribute</span></span> | <span data-ttu-id="793b3-116">属性</span><span class="sxs-lookup"><span data-stu-id="793b3-116">Property</span></span> | <span data-ttu-id="793b3-117">说明</span><span class="sxs-lookup"><span data-stu-id="793b3-117">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="793b3-118">show-max</span><span class="sxs-lookup"><span data-stu-id="793b3-118">show-max</span></span> | <span data-ttu-id="793b3-119">showMax</span><span class="sxs-lookup"><span data-stu-id="793b3-119">showMax</span></span>   | <span data-ttu-id="793b3-120">一个数字值，指示要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="793b3-120">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="793b3-121">默认值为 6。</span><span class="sxs-lookup"><span data-stu-id="793b3-121">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="793b3-122">group-id</span><span class="sxs-lookup"><span data-stu-id="793b3-122">group-id</span></span>    | <span data-ttu-id="793b3-123">groupId</span><span class="sxs-lookup"><span data-stu-id="793b3-123">groupId</span></span>     | <span data-ttu-id="793b3-124">一个字符串值，属于 Microsoft Graph定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="793b3-124">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="793b3-125">transitive-search</span><span class="sxs-lookup"><span data-stu-id="793b3-125">transitive-search</span></span>     | <span data-ttu-id="793b3-126">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="793b3-126">transitiveSearch</span></span>      | <span data-ttu-id="793b3-127">一个布尔值，用于执行可传递简单列表返回所有嵌套成员的成员的索引 - 默认情况下，不会使用可传递搜索。</span><span class="sxs-lookup"><span data-stu-id="793b3-127">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="793b3-128">type</span><span class="sxs-lookup"><span data-stu-id="793b3-128">type</span></span>     | <span data-ttu-id="793b3-129">type</span><span class="sxs-lookup"><span data-stu-id="793b3-129">type</span></span>      | <span data-ttu-id="793b3-130">要搜索的实体类型。</span><span class="sxs-lookup"><span data-stu-id="793b3-130">The type of entities to search for.</span></span> <span data-ttu-id="793b3-131">可用选项包括 `person` `group` `any` ：、、。</span><span class="sxs-lookup"><span data-stu-id="793b3-131">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="793b3-132">默认值为 `person`。</span><span class="sxs-lookup"><span data-stu-id="793b3-132">Default value is `person`.</span></span> <span data-ttu-id="793b3-133">如果设置了属性， `group-id` 则此属性无效。</span><span class="sxs-lookup"><span data-stu-id="793b3-133">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="793b3-134">user-type</span><span class="sxs-lookup"><span data-stu-id="793b3-134">user-type</span></span>     | <span data-ttu-id="793b3-135">userType</span><span class="sxs-lookup"><span data-stu-id="793b3-135">userType</span></span>      | <span data-ttu-id="793b3-136">要搜索的用户的类型。</span><span class="sxs-lookup"><span data-stu-id="793b3-136">The type of user to search for.</span></span> <span data-ttu-id="793b3-137">可用选项包括 `any` `user` ：、、组织用户或 `contact` 联系人。</span><span class="sxs-lookup"><span data-stu-id="793b3-137">Available options are: `any`, `user` for organizational users, or `contact` for contacts.</span></span> <span data-ttu-id="793b3-138">默认值为 `any`。</span><span class="sxs-lookup"><span data-stu-id="793b3-138">Default value is `any`.</span></span> |
| <span data-ttu-id="793b3-139">group-type</span><span class="sxs-lookup"><span data-stu-id="793b3-139">group-type</span></span>     | <span data-ttu-id="793b3-140">groupType</span><span class="sxs-lookup"><span data-stu-id="793b3-140">groupType</span></span>      | <span data-ttu-id="793b3-141">要搜索的组类型。</span><span class="sxs-lookup"><span data-stu-id="793b3-141">The group type to search for.</span></span> <span data-ttu-id="793b3-142">可用选项包括 `unified` `security` `mailenabledsecurity` ：、、、、。 `distribution` `any`</span><span class="sxs-lookup"><span data-stu-id="793b3-142">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="793b3-143">默认值为 `any`。</span><span class="sxs-lookup"><span data-stu-id="793b3-143">Default value is `any`.</span></span> <span data-ttu-id="793b3-144">如果该属性设置为 ， `type` 则此属性无效 `person` 。</span><span class="sxs-lookup"><span data-stu-id="793b3-144">This attribute has no effect if the `type` property is set to `person`.</span></span>  |
| <span data-ttu-id="793b3-145">selected-people</span><span class="sxs-lookup"><span data-stu-id="793b3-145">selected-people</span></span>  | <span data-ttu-id="793b3-146">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="793b3-146">selectedPeople</span></span>     | <span data-ttu-id="793b3-147">所选人员数组。</span><span class="sxs-lookup"><span data-stu-id="793b3-147">An array of selected people.</span></span> <span data-ttu-id="793b3-148">设置此值以编程方式选择人员。</span><span class="sxs-lookup"><span data-stu-id="793b3-148">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="793b3-149">people</span><span class="sxs-lookup"><span data-stu-id="793b3-149">people</span></span>   | <span data-ttu-id="793b3-150">people</span><span class="sxs-lookup"><span data-stu-id="793b3-150">people</span></span>    | <span data-ttu-id="793b3-151">在搜索结果中找到并呈现的一组人员</span><span class="sxs-lookup"><span data-stu-id="793b3-151">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="793b3-152">占位符</span><span class="sxs-lookup"><span data-stu-id="793b3-152">placeholder</span></span>   | <span data-ttu-id="793b3-153">占位符</span><span class="sxs-lookup"><span data-stu-id="793b3-153">placeholder</span></span>    | <span data-ttu-id="793b3-154">用于说明如何使用该组件的默认文本。</span><span class="sxs-lookup"><span data-stu-id="793b3-154">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="793b3-155">默认值为 `Start typing a name`。</span><span class="sxs-lookup"><span data-stu-id="793b3-155">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="793b3-156">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="793b3-156">default-selected-user-ids</span></span> | <span data-ttu-id="793b3-157">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="793b3-157">defaultSelectedUserIds</span></span> | <span data-ttu-id="793b3-158">当提供以逗号分隔的 Microsoft Graph用户 ID 时，组件在初始化时将呈现选择各自的用户。</span><span class="sxs-lookup"><span data-stu-id="793b3-158">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="793b3-159">default-selected-group-ids</span><span class="sxs-lookup"><span data-stu-id="793b3-159">default-selected-group-ids</span></span> | <span data-ttu-id="793b3-160">defaultSelectedGroupIds</span><span class="sxs-lookup"><span data-stu-id="793b3-160">defaultSelectedGroupIds</span></span> | <span data-ttu-id="793b3-161">类似于 default-selected-user-ids，当提供以逗号分隔的 Microsoft Graph 组 ID 的字符串时，组件在初始化时呈现选择各自的组。</span><span class="sxs-lookup"><span data-stu-id="793b3-161">Similar to default-selected-user-ids, when provided a string of comma-separated Microsoft Graph group IDs, the component renders the respective groups as selected upon initialization.</span></span>
| <span data-ttu-id="793b3-162">选择模式</span><span class="sxs-lookup"><span data-stu-id="793b3-162">selection-mode</span></span> | <span data-ttu-id="793b3-163">selectionMode</span><span class="sxs-lookup"><span data-stu-id="793b3-163">selectionMode</span></span> | <span data-ttu-id="793b3-164">用于指示是允许为用户或组选择 (项目，还是) 一个项目。</span><span class="sxs-lookup"><span data-stu-id="793b3-164">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="793b3-165">可用选项包括 `single` `multiple` ：、。</span><span class="sxs-lookup"><span data-stu-id="793b3-165">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="793b3-166">默认值为 `multiple`。</span><span class="sxs-lookup"><span data-stu-id="793b3-166">Default value is `multiple`.</span></span>
| <span data-ttu-id="793b3-167">disabled</span><span class="sxs-lookup"><span data-stu-id="793b3-167">disabled</span></span> | <span data-ttu-id="793b3-168">disabled</span><span class="sxs-lookup"><span data-stu-id="793b3-168">disabled</span></span> | <span data-ttu-id="793b3-169">设置是否禁用人员选取器。</span><span class="sxs-lookup"><span data-stu-id="793b3-169">Sets whether the people picker is disabled.</span></span> <span data-ttu-id="793b3-170">禁用后，用户将无法搜索或选择人员。</span><span class="sxs-lookup"><span data-stu-id="793b3-170">When disabled, the user is not able to search or select people.</span></span>
| <span data-ttu-id="793b3-171">allow-any-email</span><span class="sxs-lookup"><span data-stu-id="793b3-171">allow-any-email</span></span> | <span data-ttu-id="793b3-172">allowAnyEmail</span><span class="sxs-lookup"><span data-stu-id="793b3-172">allowAnyEmail</span></span> | <span data-ttu-id="793b3-173">指示人员选取器是否可以在不选择人员的情况下接受电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="793b3-173">Indicates whether the people picker can accept email addresses without selecting a person.</span></span> <span data-ttu-id="793b3-174">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="793b3-174">Default value is `false`.</span></span> <span data-ttu-id="793b3-175">键入完电子邮件地址后，可以按逗号 () ，用分号 () ，按 Tab 键或输入键进行 `,` `;` 添加。</span><span class="sxs-lookup"><span data-stu-id="793b3-175">When you finish typing an email address, you can press comma (`,`), semicolon (`;`), tab or enter keys to add it.</span></span>

<span data-ttu-id="793b3-176">下面是一 `show-max` 个示例。</span><span class="sxs-lookup"><span data-stu-id="793b3-176">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="793b3-177">选定人员</span><span class="sxs-lookup"><span data-stu-id="793b3-177">Selected people</span></span>

<span data-ttu-id="793b3-178">组件的"所选人员"部分呈现开发人员或用户选择的每个人。</span><span class="sxs-lookup"><span data-stu-id="793b3-178">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="793b3-180">可以通过执行以下操作之一填充所选人员数据：</span><span class="sxs-lookup"><span data-stu-id="793b3-180">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="793b3-181">直接 `selectedPeople` 设置属性，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="793b3-181">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="793b3-182">使用 `selectUsersById()` 方法，该方法接受 Microsoft graph 用户 [ID](/graph/api/resources/users) 数组，以查找关联的用户详细信息进行选择。</span><span class="sxs-lookup"><span data-stu-id="793b3-182">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="793b3-183">**注意：** 如果没有为 找到用户 `id` ，则不会为此呈现任何数据 `id` 。</span><span class="sxs-lookup"><span data-stu-id="793b3-183">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="793b3-184">活动</span><span class="sxs-lookup"><span data-stu-id="793b3-184">Events</span></span>

<span data-ttu-id="793b3-185">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="793b3-185">The following events are fired from the component.</span></span>

| <span data-ttu-id="793b3-186">事件</span><span class="sxs-lookup"><span data-stu-id="793b3-186">Event</span></span> | <span data-ttu-id="793b3-187">说明</span><span class="sxs-lookup"><span data-stu-id="793b3-187">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="793b3-188">用户在选定/选取的人列表中添加或删除了人员。</span><span class="sxs-lookup"><span data-stu-id="793b3-188">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="793b3-189">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="793b3-189">CSS custom properties</span></span>

<span data-ttu-id="793b3-190">组件 `mgt-people-picker` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="793b3-190">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

```css
mgt-people-picker {
    --input-border: 2px rgba(255, 255, 255, 0.5) solid; /* sets all input area border */

      /* OR individual input border sides */
    --input-border-bottom: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-right: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-left: 2px rgba(255, 255, 255, 0.5) solid;
    --input-border-top: 2px rgba(255, 255, 255, 0.5) solid;

    --input-background-color: #1f1f1f; /* input area background color */
    --input-border-color--hover: #008394; /* input area border hover color */
    --input-border-color--focus: #0f78d4; /* input area border focus color */

    --dropdown-background-color: #1f1f1f; /* selection area background color */
    --dropdown-item-hover-background: #333d47; /* person background color on hover */
    
    --selected-person-background-color: #f1f1f1; /* person item background color */
    
    --color: white; /* input area border focus color */
    --placeholder-color: #f1f1f1; /* placeholder text color */
    --placeholder-color--focus: rgba(255, 255, 255, 0.8); /* placeholder text focus color */
}
```

## <a name="templates"></a><span data-ttu-id="793b3-191">模板</span><span class="sxs-lookup"><span data-stu-id="793b3-191">Templates</span></span>

 <span data-ttu-id="793b3-192">`mgt-people-picker` 支持 [多个](../customize-components/templates.md) 模板，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="793b3-192">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="793b3-193">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。</span><span class="sxs-lookup"><span data-stu-id="793b3-193">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="793b3-194">数据类型</span><span class="sxs-lookup"><span data-stu-id="793b3-194">Data type</span></span> | <span data-ttu-id="793b3-195">数据上下文</span><span class="sxs-lookup"><span data-stu-id="793b3-195">Data context</span></span> | <span data-ttu-id="793b3-196">说明</span><span class="sxs-lookup"><span data-stu-id="793b3-196">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="793b3-197">default</span><span class="sxs-lookup"><span data-stu-id="793b3-197">default</span></span> | <span data-ttu-id="793b3-198">null：无数据</span><span class="sxs-lookup"><span data-stu-id="793b3-198">null: no data</span></span> | <span data-ttu-id="793b3-199">用于替代整个组件的呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="793b3-199">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="793b3-200">loading</span><span class="sxs-lookup"><span data-stu-id="793b3-200">loading</span></span> | <span data-ttu-id="793b3-201">null：无数据</span><span class="sxs-lookup"><span data-stu-id="793b3-201">null: no data</span></span> | <span data-ttu-id="793b3-202">在请求图形时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="793b3-202">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="793b3-203">error</span><span class="sxs-lookup"><span data-stu-id="793b3-203">error</span></span> | <span data-ttu-id="793b3-204">null：无数据</span><span class="sxs-lookup"><span data-stu-id="793b3-204">null: no data</span></span> | <span data-ttu-id="793b3-205">当用户搜索未返回任何用户时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="793b3-205">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="793b3-206">no-data</span><span class="sxs-lookup"><span data-stu-id="793b3-206">no-data</span></span> | <span data-ttu-id="793b3-207">null：无数据</span><span class="sxs-lookup"><span data-stu-id="793b3-207">null: no data</span></span> | <span data-ttu-id="793b3-208">如果用户搜索未返回任何用户，则使用备用模板。</span><span class="sxs-lookup"><span data-stu-id="793b3-208">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="793b3-209">selected-person</span><span class="sxs-lookup"><span data-stu-id="793b3-209">selected-person</span></span> | <span data-ttu-id="793b3-210">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="793b3-210">person: The person details object</span></span> | <span data-ttu-id="793b3-211">用于呈现选定人员的模板。</span><span class="sxs-lookup"><span data-stu-id="793b3-211">The template to render selected people.</span></span> |
| <span data-ttu-id="793b3-212">person</span><span class="sxs-lookup"><span data-stu-id="793b3-212">person</span></span> | <span data-ttu-id="793b3-213">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="793b3-213">person: The person details object</span></span> | <span data-ttu-id="793b3-214">下拉列表中用于呈现人员的模板。</span><span class="sxs-lookup"><span data-stu-id="793b3-214">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="793b3-215">以下示例演示如何使用 `error` 模板。</span><span class="sxs-lookup"><span data-stu-id="793b3-215">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="793b3-216">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="793b3-216">Microsoft Graph permissions</span></span>

<span data-ttu-id="793b3-217">此组件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="793b3-217">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="793b3-218">配置</span><span class="sxs-lookup"><span data-stu-id="793b3-218">Configuration</span></span> | <span data-ttu-id="793b3-219">权限</span><span class="sxs-lookup"><span data-stu-id="793b3-219">Permission</span></span> | <span data-ttu-id="793b3-220">API</span><span class="sxs-lookup"><span data-stu-id="793b3-220">API</span></span>
| --- | ---------- | ------- |
| <span data-ttu-id="793b3-221">`group-id` set</span><span class="sxs-lookup"><span data-stu-id="793b3-221">`group-id` set</span></span> | <span data-ttu-id="793b3-222">People.Read、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="793b3-222">People.Read, User.Read.All</span></span> | [<span data-ttu-id="793b3-223">/groups/ \$ {groupId}/members</span><span class="sxs-lookup"><span data-stu-id="793b3-223">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) |
| <span data-ttu-id="793b3-224">`type` 设置为 `Person` 或 `any`</span><span class="sxs-lookup"><span data-stu-id="793b3-224">`type` set to `Person` or `any`</span></span> | <span data-ttu-id="793b3-225">People.Read</span><span class="sxs-lookup"><span data-stu-id="793b3-225">People.Read</span></span> | [<span data-ttu-id="793b3-226">/me/people</span><span class="sxs-lookup"><span data-stu-id="793b3-226">/me/people</span></span>](/graph/api/user-list-people) |
| <span data-ttu-id="793b3-227">`type` 设置为 `Group` 或 搜索用户， `type` 并设置为 `Group` 或 `any`</span><span class="sxs-lookup"><span data-stu-id="793b3-227">`type` set to `Group` or searching for users and `type` set to `Group` or `any`</span></span> | <span data-ttu-id="793b3-228">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="793b3-228">Group.Read.All</span></span> | [<span data-ttu-id="793b3-229">/groups</span><span class="sxs-lookup"><span data-stu-id="793b3-229">/groups</span></span>](/graph/api/group-list) |
| <span data-ttu-id="793b3-230">`default-selected-user-ids` set</span><span class="sxs-lookup"><span data-stu-id="793b3-230">`default-selected-user-ids` set</span></span> | <span data-ttu-id="793b3-231">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="793b3-231">User.ReadBasic.All</span></span> | [<span data-ttu-id="793b3-232">/users</span><span class="sxs-lookup"><span data-stu-id="793b3-232">/users</span></span>](/graph/api/user-list) |
| <span data-ttu-id="793b3-233">搜索用户， `type` 并设置为 `Person` 或 `any`</span><span class="sxs-lookup"><span data-stu-id="793b3-233">searching for users and `type` set to `Person` or `any`</span></span> | <span data-ttu-id="793b3-234">People.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="793b3-234">People.Read, User.ReadBasic.All</span></span> | <span data-ttu-id="793b3-235">[/me/people](/graph/api/user-list-people)、 [/users](/graph/api/user-list)</span><span class="sxs-lookup"><span data-stu-id="793b3-235">[/me/people](/graph/api/user-list-people), [/users](/graph/api/user-list)</span></span> |

## <a name="authentication"></a><span data-ttu-id="793b3-236">身份验证</span><span class="sxs-lookup"><span data-stu-id="793b3-236">Authentication</span></span>

<span data-ttu-id="793b3-237">该控件使用身份验证文档中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="793b3-237">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="793b3-238">缓存</span><span class="sxs-lookup"><span data-stu-id="793b3-238">Cache</span></span>

|<span data-ttu-id="793b3-239">对象存储</span><span class="sxs-lookup"><span data-stu-id="793b3-239">Object store</span></span>|<span data-ttu-id="793b3-240">缓存数据</span><span class="sxs-lookup"><span data-stu-id="793b3-240">Cached data</span></span>|<span data-ttu-id="793b3-241">备注</span><span class="sxs-lookup"><span data-stu-id="793b3-241">Remarks</span></span>|
|---------|-----------|-------|
|`groups`|<span data-ttu-id="793b3-242">组列表</span><span class="sxs-lookup"><span data-stu-id="793b3-242">List of groups</span></span>|<span data-ttu-id="793b3-243">设置为 `type` 时使用 `PersonType.group`</span><span class="sxs-lookup"><span data-stu-id="793b3-243">Used when `type` is set to `PersonType.group`</span></span>|
|`people`|<span data-ttu-id="793b3-244">人员列表</span><span class="sxs-lookup"><span data-stu-id="793b3-244">List of people</span></span>|<span data-ttu-id="793b3-245">设置为 或 `type` `PersonType.person` 时使用 `PersonType.any`</span><span class="sxs-lookup"><span data-stu-id="793b3-245">Used when `type` is set to `PersonType.person` or `PersonType.any`</span></span>|
|`users`|<span data-ttu-id="793b3-246">用户列表</span><span class="sxs-lookup"><span data-stu-id="793b3-246">List of users</span></span>|<span data-ttu-id="793b3-247">指定时 `groupId` 使用</span><span class="sxs-lookup"><span data-stu-id="793b3-247">Used when `groupId` specified</span></span>|

<span data-ttu-id="793b3-248">请参阅[Caching，](../customize-components/cache.md)了解有关如何配置缓存的更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="793b3-248">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="793b3-249">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="793b3-249">Extend for more control</span></span>

<span data-ttu-id="793b3-250">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="793b3-250">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="793b3-251">方法</span><span class="sxs-lookup"><span data-stu-id="793b3-251">Method</span></span> | <span data-ttu-id="793b3-252">说明</span><span class="sxs-lookup"><span data-stu-id="793b3-252">Description</span></span> |
| - | - |
| <span data-ttu-id="793b3-253">renderInput</span><span class="sxs-lookup"><span data-stu-id="793b3-253">renderInput</span></span> | <span data-ttu-id="793b3-254">呈现输入文本框。</span><span class="sxs-lookup"><span data-stu-id="793b3-254">Renders the input text box.</span></span> |
| <span data-ttu-id="793b3-255">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="793b3-255">renderSelectedPeople</span></span> | <span data-ttu-id="793b3-256">呈现所选人员令牌。</span><span class="sxs-lookup"><span data-stu-id="793b3-256">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="793b3-257">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="793b3-257">renderSelectedPerson</span></span> | <span data-ttu-id="793b3-258">呈现个人个人令牌。</span><span class="sxs-lookup"><span data-stu-id="793b3-258">Renders an individual person token.</span></span> |
| <span data-ttu-id="793b3-259">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="793b3-259">renderFlyout</span></span> | <span data-ttu-id="793b3-260">呈现飞出部件版式。</span><span class="sxs-lookup"><span data-stu-id="793b3-260">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="793b3-261">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="793b3-261">renderFlyoutContent</span></span> | <span data-ttu-id="793b3-262">在结果飞出控件中呈现相应的状态。</span><span class="sxs-lookup"><span data-stu-id="793b3-262">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="793b3-263">renderLoading</span><span class="sxs-lookup"><span data-stu-id="793b3-263">renderLoading</span></span> | <span data-ttu-id="793b3-264">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="793b3-264">Renders the loading state.</span></span> |
| <span data-ttu-id="793b3-265">renderNoData</span><span class="sxs-lookup"><span data-stu-id="793b3-265">renderNoData</span></span> | <span data-ttu-id="793b3-266">当未找到搜索查询的结果时呈现状态。</span><span class="sxs-lookup"><span data-stu-id="793b3-266">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="793b3-267">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="793b3-267">renderSearchResults</span></span> | <span data-ttu-id="793b3-268">呈现搜索结果列表。</span><span class="sxs-lookup"><span data-stu-id="793b3-268">Renders the list of search results.</span></span> |
| <span data-ttu-id="793b3-269">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="793b3-269">renderPersonResult</span></span> | <span data-ttu-id="793b3-270">呈现个人搜索结果。</span><span class="sxs-lookup"><span data-stu-id="793b3-270">Renders an individual person search result.</span></span> |
