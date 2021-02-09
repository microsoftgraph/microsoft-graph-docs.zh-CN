---
title: People-Picker组件
description: 可以使用 mgt-people-picker Web 组件搜索指定数量的人，然后通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 691955aa64ff0afc42b5f8912658a6f36e1d77ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161374"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="125e5-103">People-Picker Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="125e5-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="125e5-104">您可以使用 Web `mgt-people-picker` 组件搜索用户和/或组。</span><span class="sxs-lookup"><span data-stu-id="125e5-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="125e5-105">默认情况下，该组件将搜索组织的所有人员及用户，但您可以将行为更改为同时搜索组或仅搜索组。</span><span class="sxs-lookup"><span data-stu-id="125e5-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="125e5-106">还可以将搜索筛选到特定组。</span><span class="sxs-lookup"><span data-stu-id="125e5-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="125e5-107">示例</span><span class="sxs-lookup"><span data-stu-id="125e5-107">Example</span></span>

<span data-ttu-id="125e5-108">以下示例显示 `mgt-people-picker` 组件。</span><span class="sxs-lookup"><span data-stu-id="125e5-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="125e5-109">开始搜索名称以查看结果呈现情况，并使用代码编辑器查看属性 [如何更改组件](#properties) 的行为。</span><span class="sxs-lookup"><span data-stu-id="125e5-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="125e5-110">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="125e5-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="125e5-111">属性</span><span class="sxs-lookup"><span data-stu-id="125e5-111">Properties</span></span>

<span data-ttu-id="125e5-112">默认情况下， `mgt-people-picker` 该组件从和终结点 `/me/people` 提取 `/users` 人员。</span><span class="sxs-lookup"><span data-stu-id="125e5-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="125e5-113">使用以下属性可更改此行为。</span><span class="sxs-lookup"><span data-stu-id="125e5-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="125e5-114">属性</span><span class="sxs-lookup"><span data-stu-id="125e5-114">Attribute</span></span> | <span data-ttu-id="125e5-115">属性</span><span class="sxs-lookup"><span data-stu-id="125e5-115">Property</span></span> | <span data-ttu-id="125e5-116">说明</span><span class="sxs-lookup"><span data-stu-id="125e5-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="125e5-117">show-max</span><span class="sxs-lookup"><span data-stu-id="125e5-117">show-max</span></span> | <span data-ttu-id="125e5-118">showMax</span><span class="sxs-lookup"><span data-stu-id="125e5-118">showMax</span></span>   | <span data-ttu-id="125e5-119">一个数字值，指示要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="125e5-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="125e5-120">默认值为 6。</span><span class="sxs-lookup"><span data-stu-id="125e5-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="125e5-121">group-id</span><span class="sxs-lookup"><span data-stu-id="125e5-121">group-id</span></span>    | <span data-ttu-id="125e5-122">groupId</span><span class="sxs-lookup"><span data-stu-id="125e5-122">groupId</span></span>     | <span data-ttu-id="125e5-123">一个字符串值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="125e5-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="125e5-124">type</span><span class="sxs-lookup"><span data-stu-id="125e5-124">type</span></span>     | <span data-ttu-id="125e5-125">type</span><span class="sxs-lookup"><span data-stu-id="125e5-125">type</span></span>      | <span data-ttu-id="125e5-126">要搜索的实体的类型。</span><span class="sxs-lookup"><span data-stu-id="125e5-126">The type of entities to search for.</span></span> <span data-ttu-id="125e5-127">可用选项有： `person` ， `group` 。 `any`</span><span class="sxs-lookup"><span data-stu-id="125e5-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="125e5-128">默认值为 `person`。</span><span class="sxs-lookup"><span data-stu-id="125e5-128">Default value is `person`.</span></span> <span data-ttu-id="125e5-129">如果设置了属性， `group-id` 则此属性无效。</span><span class="sxs-lookup"><span data-stu-id="125e5-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="125e5-130">transitive-search</span><span class="sxs-lookup"><span data-stu-id="125e5-130">transitive-search</span></span>     | <span data-ttu-id="125e5-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="125e5-131">transitiveSearch</span></span>      | <span data-ttu-id="125e5-132">用于执行可传递搜索的布尔值简单列表所有嵌套成员返回一个值 ，默认情况下，不使用可传递搜索。</span><span class="sxs-lookup"><span data-stu-id="125e5-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="125e5-133">group-type</span><span class="sxs-lookup"><span data-stu-id="125e5-133">group-type</span></span>     | <span data-ttu-id="125e5-134">groupType</span><span class="sxs-lookup"><span data-stu-id="125e5-134">groupType</span></span>      | <span data-ttu-id="125e5-135">要搜索的组类型。</span><span class="sxs-lookup"><span data-stu-id="125e5-135">The group type to search for.</span></span> <span data-ttu-id="125e5-136">可用选项有： `unified` `security` ， ， ， `mailenabledsecurity` `distribution` `any` 。</span><span class="sxs-lookup"><span data-stu-id="125e5-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="125e5-137">默认值为 `any`。</span><span class="sxs-lookup"><span data-stu-id="125e5-137">Default value is `any`.</span></span> <span data-ttu-id="125e5-138">如果该属性设置为 ，则 `type` 此属性不起作用 `person` 。</span><span class="sxs-lookup"><span data-stu-id="125e5-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="125e5-139">selected-people</span><span class="sxs-lookup"><span data-stu-id="125e5-139">selected-people</span></span>  | <span data-ttu-id="125e5-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="125e5-140">selectedPeople</span></span>     | <span data-ttu-id="125e5-141">所选人员数组。</span><span class="sxs-lookup"><span data-stu-id="125e5-141">An array of selected people.</span></span> <span data-ttu-id="125e5-142">设置此值以编程方式选择人员。</span><span class="sxs-lookup"><span data-stu-id="125e5-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="125e5-143">people</span><span class="sxs-lookup"><span data-stu-id="125e5-143">people</span></span>   | <span data-ttu-id="125e5-144">people</span><span class="sxs-lookup"><span data-stu-id="125e5-144">people</span></span>    | <span data-ttu-id="125e5-145">在搜索结果中找到并呈现的一组人员</span><span class="sxs-lookup"><span data-stu-id="125e5-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="125e5-146">占位符</span><span class="sxs-lookup"><span data-stu-id="125e5-146">placeholder</span></span>   | <span data-ttu-id="125e5-147">占位符</span><span class="sxs-lookup"><span data-stu-id="125e5-147">placeholder</span></span>    | <span data-ttu-id="125e5-148">解释如何使用组件的默认文本。</span><span class="sxs-lookup"><span data-stu-id="125e5-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="125e5-149">默认值为 `Start typing a name`。</span><span class="sxs-lookup"><span data-stu-id="125e5-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="125e5-150">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="125e5-150">default-selected-user-ids</span></span> | <span data-ttu-id="125e5-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="125e5-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="125e5-152">当提供以逗号分隔的 Microsoft Graph 用户 ID 的字符串时，组件在初始化时呈现选定各个用户。</span><span class="sxs-lookup"><span data-stu-id="125e5-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="125e5-153">选择模式</span><span class="sxs-lookup"><span data-stu-id="125e5-153">selection-mode</span></span> | <span data-ttu-id="125e5-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="125e5-154">selectionMode</span></span> | <span data-ttu-id="125e5-155">用于指示是允许为用户或组选择多个 (组) 单个项目。</span><span class="sxs-lookup"><span data-stu-id="125e5-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="125e5-156">可用选项包括： `single` `multiple` 。</span><span class="sxs-lookup"><span data-stu-id="125e5-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="125e5-157">默认值为 `multiple`。</span><span class="sxs-lookup"><span data-stu-id="125e5-157">Default value is `multiple`.</span></span>

<span data-ttu-id="125e5-158">下面是一 `show-max` 个示例。</span><span class="sxs-lookup"><span data-stu-id="125e5-158">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="125e5-159">选定人员</span><span class="sxs-lookup"><span data-stu-id="125e5-159">Selected people</span></span>

<span data-ttu-id="125e5-160">组件的"所选人员"部分呈现开发人员或用户选择的每个人。</span><span class="sxs-lookup"><span data-stu-id="125e5-160">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="125e5-162">可以通过执行以下操作之一填充所选人员数据：</span><span class="sxs-lookup"><span data-stu-id="125e5-162">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="125e5-163">直接 `selectedPeople` 设置属性，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="125e5-163">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="125e5-164">使用此方法 `selectUsersById()` ，该方法接受 Microsoft graph 用户 [ID](/graph/api/resources/users) 数组，以查找相关用户详细信息进行选择。</span><span class="sxs-lookup"><span data-stu-id="125e5-164">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="125e5-165">**注意：** 如果未找到用户， `id` 则不会为此呈现任何数据 `id` 。</span><span class="sxs-lookup"><span data-stu-id="125e5-165">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="125e5-166">活动</span><span class="sxs-lookup"><span data-stu-id="125e5-166">Events</span></span>

<span data-ttu-id="125e5-167">从组件触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="125e5-167">The following events are fired from the component.</span></span>

| <span data-ttu-id="125e5-168">事件</span><span class="sxs-lookup"><span data-stu-id="125e5-168">Event</span></span> | <span data-ttu-id="125e5-169">说明</span><span class="sxs-lookup"><span data-stu-id="125e5-169">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="125e5-170">用户在选定/选取人员列表中添加或删除了人员。</span><span class="sxs-lookup"><span data-stu-id="125e5-170">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="125e5-171">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="125e5-171">CSS custom properties</span></span>

<span data-ttu-id="125e5-172">该 `mgt-people-picker` 组件定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="125e5-172">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="125e5-173">模板</span><span class="sxs-lookup"><span data-stu-id="125e5-173">Templates</span></span>

 <span data-ttu-id="125e5-174">`mgt-people-picker` 支持 [多个模板](../customize-components/templates.md) ，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="125e5-174">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="125e5-175">若要指定模板，请包含组件 `<template>` 中的元素，将值设置为下列 `data-type` 值之一。</span><span class="sxs-lookup"><span data-stu-id="125e5-175">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="125e5-176">数据类型</span><span class="sxs-lookup"><span data-stu-id="125e5-176">Data type</span></span> | <span data-ttu-id="125e5-177">数据上下文</span><span class="sxs-lookup"><span data-stu-id="125e5-177">Data context</span></span> | <span data-ttu-id="125e5-178">说明</span><span class="sxs-lookup"><span data-stu-id="125e5-178">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="125e5-179"> 默认值</span><span class="sxs-lookup"><span data-stu-id="125e5-179">default</span></span> | <span data-ttu-id="125e5-180">null：无数据</span><span class="sxs-lookup"><span data-stu-id="125e5-180">null: no data</span></span> | <span data-ttu-id="125e5-181">用于覆盖整个组件的呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="125e5-181">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="125e5-182">loading</span><span class="sxs-lookup"><span data-stu-id="125e5-182">loading</span></span> | <span data-ttu-id="125e5-183">null：无数据</span><span class="sxs-lookup"><span data-stu-id="125e5-183">null: no data</span></span> | <span data-ttu-id="125e5-184">在请求图形时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="125e5-184">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="125e5-185">error</span><span class="sxs-lookup"><span data-stu-id="125e5-185">error</span></span> | <span data-ttu-id="125e5-186">null：无数据</span><span class="sxs-lookup"><span data-stu-id="125e5-186">null: no data</span></span> | <span data-ttu-id="125e5-187">如果用户搜索未返回任何用户，则使用的模板。</span><span class="sxs-lookup"><span data-stu-id="125e5-187">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="125e5-188">no-data</span><span class="sxs-lookup"><span data-stu-id="125e5-188">no-data</span></span> | <span data-ttu-id="125e5-189">null：无数据</span><span class="sxs-lookup"><span data-stu-id="125e5-189">null: no data</span></span> | <span data-ttu-id="125e5-190">如果用户搜索未返回任何用户，则使用备用模板。</span><span class="sxs-lookup"><span data-stu-id="125e5-190">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="125e5-191">selected-person</span><span class="sxs-lookup"><span data-stu-id="125e5-191">selected-person</span></span> | <span data-ttu-id="125e5-192">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="125e5-192">person: The person details object</span></span> | <span data-ttu-id="125e5-193">用于呈现选定人员模板。</span><span class="sxs-lookup"><span data-stu-id="125e5-193">The template to render selected people.</span></span> |
| <span data-ttu-id="125e5-194">person</span><span class="sxs-lookup"><span data-stu-id="125e5-194">person</span></span> | <span data-ttu-id="125e5-195">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="125e5-195">person: The person details object</span></span> | <span data-ttu-id="125e5-196">在下拉列表中呈现人员模板。</span><span class="sxs-lookup"><span data-stu-id="125e5-196">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="125e5-197">以下示例显示如何使用 `error` 模板。</span><span class="sxs-lookup"><span data-stu-id="125e5-197">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="125e5-198">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="125e5-198">Microsoft Graph permissions</span></span>

<span data-ttu-id="125e5-199">此组件使用以下 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="125e5-199">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="125e5-200">API</span><span class="sxs-lookup"><span data-stu-id="125e5-200">API</span></span>                                                                                                              | <span data-ttu-id="125e5-201">权限</span><span class="sxs-lookup"><span data-stu-id="125e5-201">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="125e5-202">/me/people</span><span class="sxs-lookup"><span data-stu-id="125e5-202">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="125e5-203">People.Read</span><span class="sxs-lookup"><span data-stu-id="125e5-203">People.Read</span></span>        |
| [<span data-ttu-id="125e5-204">/users</span><span class="sxs-lookup"><span data-stu-id="125e5-204">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="125e5-205">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="125e5-205">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="125e5-206">/groups</span><span class="sxs-lookup"><span data-stu-id="125e5-206">/groups</span></span>](/group-list)  | <span data-ttu-id="125e5-207">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="125e5-207">Group.Read.All</span></span> |
| [<span data-ttu-id="125e5-208">/groups/ \$ {groupId}/members</span><span class="sxs-lookup"><span data-stu-id="125e5-208">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="125e5-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="125e5-209">User.ReadBasic.All</span></span>        |
| [<span data-ttu-id="125e5-210">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="125e5-210">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="125e5-211">User.Read</span><span class="sxs-lookup"><span data-stu-id="125e5-211">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="125e5-212">身份验证</span><span class="sxs-lookup"><span data-stu-id="125e5-212">Authentication</span></span>

<span data-ttu-id="125e5-213">该控件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="125e5-213">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="125e5-214">扩展以更多控制</span><span class="sxs-lookup"><span data-stu-id="125e5-214">Extend for more control</span></span>

<span data-ttu-id="125e5-215">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展中 `protected render*` 替代的方法。</span><span class="sxs-lookup"><span data-stu-id="125e5-215">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="125e5-216">方法</span><span class="sxs-lookup"><span data-stu-id="125e5-216">Method</span></span> | <span data-ttu-id="125e5-217">说明</span><span class="sxs-lookup"><span data-stu-id="125e5-217">Description</span></span> |
| - | - |
| <span data-ttu-id="125e5-218">renderInput</span><span class="sxs-lookup"><span data-stu-id="125e5-218">renderInput</span></span> | <span data-ttu-id="125e5-219">呈现输入文本框。</span><span class="sxs-lookup"><span data-stu-id="125e5-219">Renders the input text box.</span></span> |
| <span data-ttu-id="125e5-220">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="125e5-220">renderSelectedPeople</span></span> | <span data-ttu-id="125e5-221">呈现所选人员令牌。</span><span class="sxs-lookup"><span data-stu-id="125e5-221">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="125e5-222">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="125e5-222">renderSelectedPerson</span></span> | <span data-ttu-id="125e5-223">呈现个人个人令牌。</span><span class="sxs-lookup"><span data-stu-id="125e5-223">Renders an individual person token.</span></span> |
| <span data-ttu-id="125e5-224">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="125e5-224">renderFlyout</span></span> | <span data-ttu-id="125e5-225">呈现飞出部件版式。</span><span class="sxs-lookup"><span data-stu-id="125e5-225">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="125e5-226">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="125e5-226">renderFlyoutContent</span></span> | <span data-ttu-id="125e5-227">在结果飞出中呈现适当的状态。</span><span class="sxs-lookup"><span data-stu-id="125e5-227">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="125e5-228">renderLoading</span><span class="sxs-lookup"><span data-stu-id="125e5-228">renderLoading</span></span> | <span data-ttu-id="125e5-229">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="125e5-229">Renders the loading state.</span></span> |
| <span data-ttu-id="125e5-230">renderNoData</span><span class="sxs-lookup"><span data-stu-id="125e5-230">renderNoData</span></span> | <span data-ttu-id="125e5-231">当未找到搜索查询的结果时呈现状态。</span><span class="sxs-lookup"><span data-stu-id="125e5-231">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="125e5-232">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="125e5-232">renderSearchResults</span></span> | <span data-ttu-id="125e5-233">呈现搜索结果列表。</span><span class="sxs-lookup"><span data-stu-id="125e5-233">Renders the list of search results.</span></span> |
| <span data-ttu-id="125e5-234">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="125e5-234">renderPersonResult</span></span> | <span data-ttu-id="125e5-235">呈现个人搜索结果。</span><span class="sxs-lookup"><span data-stu-id="125e5-235">Renders an individual person search result.</span></span> |
