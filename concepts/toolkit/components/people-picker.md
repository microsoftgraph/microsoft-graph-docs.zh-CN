---
title: People-Picker组件
description: 可以使用 mgt-people-picker Web 组件搜索指定数量的人，然后通过 Microsoft Graph 呈现结果列表。
localization_priority: Normal
author: elisenyang
ms.openlocfilehash: 3531c32ae4f33898b11f7d92f91115aa1cbf43a3
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266813"
---
# <a name="people-picker-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="b5aba-103">People-Picker Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="b5aba-103">People-Picker component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="b5aba-104">您可以使用 Web `mgt-people-picker` 组件来搜索用户和/或组。</span><span class="sxs-lookup"><span data-stu-id="b5aba-104">You can use the `mgt-people-picker` web component to search for people and/or groups.</span></span> <span data-ttu-id="b5aba-105">默认情况下，组件将搜索组织中所有的用户和用户，但你可以将行为更改为同时搜索组或仅搜索组。</span><span class="sxs-lookup"><span data-stu-id="b5aba-105">By default, the component will search for all people and users in the organization, but you can change the behavior to also search for groups, or only groups.</span></span> <span data-ttu-id="b5aba-106">您还可以将搜索筛选到特定组。</span><span class="sxs-lookup"><span data-stu-id="b5aba-106">You can also filter the search to a specific group.</span></span>

## <a name="example"></a><span data-ttu-id="b5aba-107">示例</span><span class="sxs-lookup"><span data-stu-id="b5aba-107">Example</span></span>

<span data-ttu-id="b5aba-108">以下示例显示 `mgt-people-picker` 组件。</span><span class="sxs-lookup"><span data-stu-id="b5aba-108">The following example shows the `mgt-people-picker` component.</span></span> <span data-ttu-id="b5aba-109">开始搜索名称以查看结果呈现，并使用代码编辑器查看属性 [如何更改组件](#properties) 的行为。</span><span class="sxs-lookup"><span data-stu-id="b5aba-109">Start searching for a name to see the results render and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-people-picker--people-picker&source=docs" height="450"></iframe>

[<span data-ttu-id="b5aba-110">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="b5aba-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-people-picker--people-picker&source=docs)

## <a name="properties"></a><span data-ttu-id="b5aba-111">属性</span><span class="sxs-lookup"><span data-stu-id="b5aba-111">Properties</span></span>

<span data-ttu-id="b5aba-112">默认情况下， `mgt-people-picker` 组件从 和 终结点 `/me/people` 提取 `/users` 人员。</span><span class="sxs-lookup"><span data-stu-id="b5aba-112">By default, the `mgt-people-picker` component fetches people from the `/me/people` and `/users` endpoints.</span></span> <span data-ttu-id="b5aba-113">使用以下属性更改此行为。</span><span class="sxs-lookup"><span data-stu-id="b5aba-113">Use the following attributes to change this behavior.</span></span>

| <span data-ttu-id="b5aba-114">属性</span><span class="sxs-lookup"><span data-stu-id="b5aba-114">Attribute</span></span> | <span data-ttu-id="b5aba-115">属性</span><span class="sxs-lookup"><span data-stu-id="b5aba-115">Property</span></span> | <span data-ttu-id="b5aba-116">说明</span><span class="sxs-lookup"><span data-stu-id="b5aba-116">Description</span></span>                                                                                                                                                                            |
| -------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b5aba-117">show-max</span><span class="sxs-lookup"><span data-stu-id="b5aba-117">show-max</span></span> | <span data-ttu-id="b5aba-118">showMax</span><span class="sxs-lookup"><span data-stu-id="b5aba-118">showMax</span></span>   | <span data-ttu-id="b5aba-119">一个数字值，指示要显示的最大人数。</span><span class="sxs-lookup"><span data-stu-id="b5aba-119">A number value to indicate the maximum number of people to show.</span></span> <span data-ttu-id="b5aba-120">默认值为 6。</span><span class="sxs-lookup"><span data-stu-id="b5aba-120">the default value is 6.</span></span>                                                                                             |
| <span data-ttu-id="b5aba-121">group-id</span><span class="sxs-lookup"><span data-stu-id="b5aba-121">group-id</span></span>    | <span data-ttu-id="b5aba-122">groupId</span><span class="sxs-lookup"><span data-stu-id="b5aba-122">groupId</span></span>     | <span data-ttu-id="b5aba-123">一个字符串值，属于 Microsoft Graph 定义的组，用于进一步筛选搜索结果。</span><span class="sxs-lookup"><span data-stu-id="b5aba-123">A string value that belongs to a Microsoft Graph defined group for further filtering of the search results.</span></span>                                                                            |
| <span data-ttu-id="b5aba-124">type</span><span class="sxs-lookup"><span data-stu-id="b5aba-124">type</span></span>     | <span data-ttu-id="b5aba-125">type</span><span class="sxs-lookup"><span data-stu-id="b5aba-125">type</span></span>      | <span data-ttu-id="b5aba-126">要搜索的实体类型。</span><span class="sxs-lookup"><span data-stu-id="b5aba-126">The type of entities to search for.</span></span> <span data-ttu-id="b5aba-127">可用选项包括 `person` `group` `any` ：、、。</span><span class="sxs-lookup"><span data-stu-id="b5aba-127">Available options are: `person`, `group`, `any`.</span></span> <span data-ttu-id="b5aba-128">默认值为 `person`。</span><span class="sxs-lookup"><span data-stu-id="b5aba-128">Default value is `person`.</span></span> <span data-ttu-id="b5aba-129">如果设置了属性， `group-id` 则此属性无效。</span><span class="sxs-lookup"><span data-stu-id="b5aba-129">This attribute has no effect if `group-id` property is set.</span></span>         
| <span data-ttu-id="b5aba-130">transitive-search</span><span class="sxs-lookup"><span data-stu-id="b5aba-130">transitive-search</span></span>     | <span data-ttu-id="b5aba-131">transitiveSearch</span><span class="sxs-lookup"><span data-stu-id="b5aba-131">transitiveSearch</span></span>      | <span data-ttu-id="b5aba-132">一个布尔值，用于执行可传递简单列表返回所有嵌套成员的成员的索引 - 默认情况下，不会使用可传递搜索。</span><span class="sxs-lookup"><span data-stu-id="b5aba-132">A Boolean value to perform a transitive search returning a flat list of all nested members - by default transitive search is not used.</span></span>|
| <span data-ttu-id="b5aba-133">group-type</span><span class="sxs-lookup"><span data-stu-id="b5aba-133">group-type</span></span>     | <span data-ttu-id="b5aba-134">groupType</span><span class="sxs-lookup"><span data-stu-id="b5aba-134">groupType</span></span>      | <span data-ttu-id="b5aba-135">要搜索的组类型。</span><span class="sxs-lookup"><span data-stu-id="b5aba-135">The group type to search for.</span></span> <span data-ttu-id="b5aba-136">可用选项包括 `unified` `security` `mailenabledsecurity` ：、、、、。 `distribution` `any`</span><span class="sxs-lookup"><span data-stu-id="b5aba-136">Available options are: `unified`, `security`, `mailenabledsecurity`, `distribution`, `any`.</span></span> <span data-ttu-id="b5aba-137">默认值为 `any`。</span><span class="sxs-lookup"><span data-stu-id="b5aba-137">Default value is `any`.</span></span> <span data-ttu-id="b5aba-138">如果该属性设置为 ， `type` 则此属性无效 `person` 。</span><span class="sxs-lookup"><span data-stu-id="b5aba-138">This attribute has no effect if the `type` property is set to `person`.</span></span>                                                                           |
|  <span data-ttu-id="b5aba-139">selected-people</span><span class="sxs-lookup"><span data-stu-id="b5aba-139">selected-people</span></span>  | <span data-ttu-id="b5aba-140">selectedPeople</span><span class="sxs-lookup"><span data-stu-id="b5aba-140">selectedPeople</span></span>     | <span data-ttu-id="b5aba-141">所选人员数组。</span><span class="sxs-lookup"><span data-stu-id="b5aba-141">An array of selected people.</span></span> <span data-ttu-id="b5aba-142">设置此值以编程方式选择人员。</span><span class="sxs-lookup"><span data-stu-id="b5aba-142">Set this value to select people programmatically.</span></span>|
| <span data-ttu-id="b5aba-143">people</span><span class="sxs-lookup"><span data-stu-id="b5aba-143">people</span></span>   | <span data-ttu-id="b5aba-144">people</span><span class="sxs-lookup"><span data-stu-id="b5aba-144">people</span></span>    | <span data-ttu-id="b5aba-145">在搜索结果中找到并呈现的一组人员</span><span class="sxs-lookup"><span data-stu-id="b5aba-145">An array of people found and rendered in the search result</span></span> |
| <span data-ttu-id="b5aba-146">占位符</span><span class="sxs-lookup"><span data-stu-id="b5aba-146">placeholder</span></span>   | <span data-ttu-id="b5aba-147">占位符</span><span class="sxs-lookup"><span data-stu-id="b5aba-147">placeholder</span></span>    | <span data-ttu-id="b5aba-148">用于说明如何使用该组件的默认文本。</span><span class="sxs-lookup"><span data-stu-id="b5aba-148">The default text that appears to explain how to use the component.</span></span> <span data-ttu-id="b5aba-149">默认值为 `Start typing a name`。</span><span class="sxs-lookup"><span data-stu-id="b5aba-149">Default value is `Start typing a name`.</span></span>
| <span data-ttu-id="b5aba-150">default-selected-user-ids</span><span class="sxs-lookup"><span data-stu-id="b5aba-150">default-selected-user-ids</span></span> | <span data-ttu-id="b5aba-151">defaultSelectedUserIds</span><span class="sxs-lookup"><span data-stu-id="b5aba-151">defaultSelectedUserIds</span></span> | <span data-ttu-id="b5aba-152">当提供以逗号分隔的 Microsoft Graph 用户 ID 的字符串时，组件在初始化时将呈现选择各自的用户。</span><span class="sxs-lookup"><span data-stu-id="b5aba-152">When provided a string of comma-separated Microsoft Graph user IDs, the component renders the respective users as selected upon initialization.</span></span>
| <span data-ttu-id="b5aba-153">选择模式</span><span class="sxs-lookup"><span data-stu-id="b5aba-153">selection-mode</span></span> | <span data-ttu-id="b5aba-154">selectionMode</span><span class="sxs-lookup"><span data-stu-id="b5aba-154">selectionMode</span></span> | <span data-ttu-id="b5aba-155">用于指示是允许为用户或组选择 (项目，还是) 一个项目。</span><span class="sxs-lookup"><span data-stu-id="b5aba-155">Used to indicate whether to allow selecting multiple items (users or groups) or just a single item.</span></span> <span data-ttu-id="b5aba-156">可用选项包括 `single` `multiple` ：、。</span><span class="sxs-lookup"><span data-stu-id="b5aba-156">Available options are: `single`, `multiple`.</span></span> <span data-ttu-id="b5aba-157">默认值为 `multiple`。</span><span class="sxs-lookup"><span data-stu-id="b5aba-157">Default value is `multiple`.</span></span>
| <span data-ttu-id="b5aba-158">disabled</span><span class="sxs-lookup"><span data-stu-id="b5aba-158">disabled</span></span> | <span data-ttu-id="b5aba-159">disabled</span><span class="sxs-lookup"><span data-stu-id="b5aba-159">disabled</span></span> | <span data-ttu-id="b5aba-160">设置是否禁用人员选取器。</span><span class="sxs-lookup"><span data-stu-id="b5aba-160">Sets whether the people picker is disabled.</span></span> <span data-ttu-id="b5aba-161">禁用后，用户将无法搜索或选择人员。</span><span class="sxs-lookup"><span data-stu-id="b5aba-161">When disabled, the user is not able to search or select people.</span></span>

<span data-ttu-id="b5aba-162">下面是一 `show-max` 个示例。</span><span class="sxs-lookup"><span data-stu-id="b5aba-162">The following is a `show-max` example.</span></span>

```html
<mgt-people-picker show-max="4"> </mgt-people-picker>
```

## <a name="selected-people"></a><span data-ttu-id="b5aba-163">选定人员</span><span class="sxs-lookup"><span data-stu-id="b5aba-163">Selected people</span></span>

<span data-ttu-id="b5aba-164">组件的"所选人员"部分呈现开发人员或用户选择的每个人。</span><span class="sxs-lookup"><span data-stu-id="b5aba-164">The selected people section of the component renders each person chosen by the developer or user.</span></span> 

![mgt-people-picker](./images/selected-people.png)

<span data-ttu-id="b5aba-166">可以通过执行以下操作之一填充所选人员数据：</span><span class="sxs-lookup"><span data-stu-id="b5aba-166">You can populate selected people data by doing one of the following:</span></span>

- <span data-ttu-id="b5aba-167">直接 `selectedPeople` 设置属性，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="b5aba-167">Setting the `selectedPeople` property directly, as shown in the following example.</span></span>  

    ```javascript
    // personObject = User or Person from Microsoft Graph
    document.querySelector('mgt-people-picker').selectedPeople.push(personObject);
    ```

- <span data-ttu-id="b5aba-168">使用 `selectUsersById()` 方法，该方法接受 Microsoft graph 用户 [ID](/graph/api/resources/users) 数组，以查找关联的用户详细信息进行选择。</span><span class="sxs-lookup"><span data-stu-id="b5aba-168">Using the `selectUsersById()` method, which accepts an array of Microsoft graph [user ids](/graph/api/resources/users) to find associated user details for selection.</span></span>

     ><span data-ttu-id="b5aba-169">**注意：** 如果没有为 找到用户 `id` ，则不会为此呈现任何数据 `id` 。</span><span class="sxs-lookup"><span data-stu-id="b5aba-169">**Note:** If no user is found for an `id`, no data will be rendered for that `id`.</span></span>

    ```javascript
    // id = Microsoft graph User "id"
    document.querySelector('mgt-people-picker').selectUsersById(["id","id"])
    ```

## <a name="events"></a><span data-ttu-id="b5aba-170">事件</span><span class="sxs-lookup"><span data-stu-id="b5aba-170">Events</span></span>

<span data-ttu-id="b5aba-171">从组件中触发以下事件。</span><span class="sxs-lookup"><span data-stu-id="b5aba-171">The following events are fired from the component.</span></span>

| <span data-ttu-id="b5aba-172">事件</span><span class="sxs-lookup"><span data-stu-id="b5aba-172">Event</span></span> | <span data-ttu-id="b5aba-173">说明</span><span class="sxs-lookup"><span data-stu-id="b5aba-173">Description</span></span> |
| --- | --- |
| `selectionChanged` | <span data-ttu-id="b5aba-174">用户在选定/选取的人列表中添加或删除了人员。</span><span class="sxs-lookup"><span data-stu-id="b5aba-174">The user added or removed a person from the list of selected/picked people.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="b5aba-175">CSS 自定义属性</span><span class="sxs-lookup"><span data-stu-id="b5aba-175">CSS custom properties</span></span>

<span data-ttu-id="b5aba-176">组件 `mgt-people-picker` 定义以下 CSS 自定义属性。</span><span class="sxs-lookup"><span data-stu-id="b5aba-176">The `mgt-people-picker` component defines the following CSS custom properties.</span></span>

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

## <a name="templates"></a><span data-ttu-id="b5aba-177">模板</span><span class="sxs-lookup"><span data-stu-id="b5aba-177">Templates</span></span>

 <span data-ttu-id="b5aba-178">`mgt-people-picker` 支持 [多个](../customize-components/templates.md) 模板，您可以使用这些模板替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="b5aba-178">`mgt-people-picker` supports several [templates](../customize-components/templates.md) that you can use to replace certain parts of the component.</span></span> <span data-ttu-id="b5aba-179">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。</span><span class="sxs-lookup"><span data-stu-id="b5aba-179">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="b5aba-180">数据类型</span><span class="sxs-lookup"><span data-stu-id="b5aba-180">Data type</span></span> | <span data-ttu-id="b5aba-181">数据上下文</span><span class="sxs-lookup"><span data-stu-id="b5aba-181">Data context</span></span> | <span data-ttu-id="b5aba-182">说明</span><span class="sxs-lookup"><span data-stu-id="b5aba-182">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="b5aba-183">default</span><span class="sxs-lookup"><span data-stu-id="b5aba-183">default</span></span> | <span data-ttu-id="b5aba-184">null：无数据</span><span class="sxs-lookup"><span data-stu-id="b5aba-184">null: no data</span></span> | <span data-ttu-id="b5aba-185">用于替代整个组件的呈现的模板。</span><span class="sxs-lookup"><span data-stu-id="b5aba-185">The template used to override the rendering of the entire component.</span></span>
| <span data-ttu-id="b5aba-186">loading</span><span class="sxs-lookup"><span data-stu-id="b5aba-186">loading</span></span> | <span data-ttu-id="b5aba-187">null：无数据</span><span class="sxs-lookup"><span data-stu-id="b5aba-187">null: no data</span></span> | <span data-ttu-id="b5aba-188">在请求图形时用于呈现选取器状态的模板。</span><span class="sxs-lookup"><span data-stu-id="b5aba-188">The template used to render the state of picker while request to graph is being made.</span></span> |
| <span data-ttu-id="b5aba-189">error</span><span class="sxs-lookup"><span data-stu-id="b5aba-189">error</span></span> | <span data-ttu-id="b5aba-190">null：无数据</span><span class="sxs-lookup"><span data-stu-id="b5aba-190">null: no data</span></span> | <span data-ttu-id="b5aba-191">当用户搜索未返回任何用户时所使用的模板。</span><span class="sxs-lookup"><span data-stu-id="b5aba-191">The template used if user search returns no users.</span></span> |
| <span data-ttu-id="b5aba-192">no-data</span><span class="sxs-lookup"><span data-stu-id="b5aba-192">no-data</span></span> | <span data-ttu-id="b5aba-193">null：无数据</span><span class="sxs-lookup"><span data-stu-id="b5aba-193">null: no data</span></span> | <span data-ttu-id="b5aba-194">如果用户搜索未返回任何用户，则使用备用模板。</span><span class="sxs-lookup"><span data-stu-id="b5aba-194">An alternative template used if user search returns no users.</span></span> |
| <span data-ttu-id="b5aba-195">selected-person</span><span class="sxs-lookup"><span data-stu-id="b5aba-195">selected-person</span></span> | <span data-ttu-id="b5aba-196">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="b5aba-196">person: The person details object</span></span> | <span data-ttu-id="b5aba-197">用于呈现选定人员的模板。</span><span class="sxs-lookup"><span data-stu-id="b5aba-197">The template to render selected people.</span></span> |
| <span data-ttu-id="b5aba-198">person</span><span class="sxs-lookup"><span data-stu-id="b5aba-198">person</span></span> | <span data-ttu-id="b5aba-199">person： The person details object</span><span class="sxs-lookup"><span data-stu-id="b5aba-199">person: The person details object</span></span> | <span data-ttu-id="b5aba-200">下拉列表中用于呈现人员的模板。</span><span class="sxs-lookup"><span data-stu-id="b5aba-200">The template to render people in the dropdown.</span></span> |

<span data-ttu-id="b5aba-201">以下示例演示如何使用 `error` 模板。</span><span class="sxs-lookup"><span data-stu-id="b5aba-201">The following examples shows how to use the `error` template.</span></span>

```html
<mgt-people-picker>
  <template data-type="error">
    <p>Sorry, no people were found</p>
  </template>
</mgt-people-picker>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="b5aba-202">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="b5aba-202">Microsoft Graph permissions</span></span>

<span data-ttu-id="b5aba-203">此组件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="b5aba-203">This component uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="b5aba-204">API</span><span class="sxs-lookup"><span data-stu-id="b5aba-204">API</span></span>                                                                                                              | <span data-ttu-id="b5aba-205">权限</span><span class="sxs-lookup"><span data-stu-id="b5aba-205">Permission</span></span>  |
| ---------------------------------------------------------------------------------------------------------------- | ----------- |
| [<span data-ttu-id="b5aba-206">/me/people</span><span class="sxs-lookup"><span data-stu-id="b5aba-206">/me/people</span></span>](/graph/api/user-list-people)                    | <span data-ttu-id="b5aba-207">People.Read</span><span class="sxs-lookup"><span data-stu-id="b5aba-207">People.Read</span></span>        |
| [<span data-ttu-id="b5aba-208">/users</span><span class="sxs-lookup"><span data-stu-id="b5aba-208">/users</span></span>](/graph/api/user-list)  | <span data-ttu-id="b5aba-209">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="b5aba-209">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="b5aba-210">/groups</span><span class="sxs-lookup"><span data-stu-id="b5aba-210">/groups</span></span>](/group-list)  | <span data-ttu-id="b5aba-211">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5aba-211">Group.Read.All</span></span> |
| [<span data-ttu-id="b5aba-212">/groups/ \$ {groupId}/members</span><span class="sxs-lookup"><span data-stu-id="b5aba-212">/groups/\${groupId}/members</span></span>](/graph/api/group-list-members) | <span data-ttu-id="b5aba-213">GroupMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5aba-213">GroupMember.Read.All</span></span>        |
| [<span data-ttu-id="b5aba-214">/users/${userPrincipleName} </span><span class="sxs-lookup"><span data-stu-id="b5aba-214">/users/${userPrincipleName} </span></span>](/graph/api/user-get)  | <span data-ttu-id="b5aba-215">User.Read</span><span class="sxs-lookup"><span data-stu-id="b5aba-215">User.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="b5aba-216">身份验证</span><span class="sxs-lookup"><span data-stu-id="b5aba-216">Authentication</span></span>

<span data-ttu-id="b5aba-217">该控件使用身份验证文档中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="b5aba-217">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="b5aba-218">缓存</span><span class="sxs-lookup"><span data-stu-id="b5aba-218">Cache</span></span>

|<span data-ttu-id="b5aba-219">对象存储</span><span class="sxs-lookup"><span data-stu-id="b5aba-219">Object store</span></span>|<span data-ttu-id="b5aba-220">缓存数据</span><span class="sxs-lookup"><span data-stu-id="b5aba-220">Cached data</span></span>|<span data-ttu-id="b5aba-221">备注</span><span class="sxs-lookup"><span data-stu-id="b5aba-221">Remarks</span></span>|
|---------|-----------|-------|
|`groups`|<span data-ttu-id="b5aba-222">组列表</span><span class="sxs-lookup"><span data-stu-id="b5aba-222">List of groups</span></span>|<span data-ttu-id="b5aba-223">设置为 `type` 时使用 `PersonType.group`</span><span class="sxs-lookup"><span data-stu-id="b5aba-223">Used when `type` is set to `PersonType.group`</span></span>|
|`people`|<span data-ttu-id="b5aba-224">人员列表</span><span class="sxs-lookup"><span data-stu-id="b5aba-224">List of people</span></span>|<span data-ttu-id="b5aba-225">设置为 或 `type` `PersonType.person` 时使用 `PersonType.any`</span><span class="sxs-lookup"><span data-stu-id="b5aba-225">Used when `type` is set to `PersonType.person` or `PersonType.any`</span></span>|
|`users`|<span data-ttu-id="b5aba-226">用户列表</span><span class="sxs-lookup"><span data-stu-id="b5aba-226">List of users</span></span>|<span data-ttu-id="b5aba-227">指定时 `groupId` 使用</span><span class="sxs-lookup"><span data-stu-id="b5aba-227">Used when `groupId` specified</span></span>|

<span data-ttu-id="b5aba-228">若要 [详细了解](../customize-components/cache.md) 如何配置缓存，请参阅缓存。</span><span class="sxs-lookup"><span data-stu-id="b5aba-228">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
## <a name="extend-for-more-control"></a><span data-ttu-id="b5aba-229">扩展以了解更多控件</span><span class="sxs-lookup"><span data-stu-id="b5aba-229">Extend for more control</span></span>

<span data-ttu-id="b5aba-230">对于更复杂的方案或真正自定义的 UX，此组件公开了多个在组件扩展 `protected render*` 中替代的方法。</span><span class="sxs-lookup"><span data-stu-id="b5aba-230">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="b5aba-231">方法</span><span class="sxs-lookup"><span data-stu-id="b5aba-231">Method</span></span> | <span data-ttu-id="b5aba-232">说明</span><span class="sxs-lookup"><span data-stu-id="b5aba-232">Description</span></span> |
| - | - |
| <span data-ttu-id="b5aba-233">renderInput</span><span class="sxs-lookup"><span data-stu-id="b5aba-233">renderInput</span></span> | <span data-ttu-id="b5aba-234">呈现输入文本框。</span><span class="sxs-lookup"><span data-stu-id="b5aba-234">Renders the input text box.</span></span> |
| <span data-ttu-id="b5aba-235">renderSelectedPeople</span><span class="sxs-lookup"><span data-stu-id="b5aba-235">renderSelectedPeople</span></span> | <span data-ttu-id="b5aba-236">呈现所选人员令牌。</span><span class="sxs-lookup"><span data-stu-id="b5aba-236">Renders the selected people tokens.</span></span> |
| <span data-ttu-id="b5aba-237">renderSelectedPerson</span><span class="sxs-lookup"><span data-stu-id="b5aba-237">renderSelectedPerson</span></span> | <span data-ttu-id="b5aba-238">呈现个人个人令牌。</span><span class="sxs-lookup"><span data-stu-id="b5aba-238">Renders an individual person token.</span></span> |
| <span data-ttu-id="b5aba-239">renderFlyout</span><span class="sxs-lookup"><span data-stu-id="b5aba-239">renderFlyout</span></span> | <span data-ttu-id="b5aba-240">呈现飞出部件版式。</span><span class="sxs-lookup"><span data-stu-id="b5aba-240">Renders the flyout chrome.</span></span> |
| <span data-ttu-id="b5aba-241">renderFlyoutContent</span><span class="sxs-lookup"><span data-stu-id="b5aba-241">renderFlyoutContent</span></span> | <span data-ttu-id="b5aba-242">在结果飞出控件中呈现相应的状态。</span><span class="sxs-lookup"><span data-stu-id="b5aba-242">Renders the appropriate state in the results flyout.</span></span> |
| <span data-ttu-id="b5aba-243">renderLoading</span><span class="sxs-lookup"><span data-stu-id="b5aba-243">renderLoading</span></span> | <span data-ttu-id="b5aba-244">呈现加载状态。</span><span class="sxs-lookup"><span data-stu-id="b5aba-244">Renders the loading state.</span></span> |
| <span data-ttu-id="b5aba-245">renderNoData</span><span class="sxs-lookup"><span data-stu-id="b5aba-245">renderNoData</span></span> | <span data-ttu-id="b5aba-246">当未找到搜索查询的结果时呈现状态。</span><span class="sxs-lookup"><span data-stu-id="b5aba-246">Renders the state when no results are found for the search query.</span></span> |
| <span data-ttu-id="b5aba-247">renderSearchResults</span><span class="sxs-lookup"><span data-stu-id="b5aba-247">renderSearchResults</span></span> | <span data-ttu-id="b5aba-248">呈现搜索结果列表。</span><span class="sxs-lookup"><span data-stu-id="b5aba-248">Renders the list of search results.</span></span> |
| <span data-ttu-id="b5aba-249">renderPersonResult</span><span class="sxs-lookup"><span data-stu-id="b5aba-249">renderPersonResult</span></span> | <span data-ttu-id="b5aba-250">呈现个人搜索结果。</span><span class="sxs-lookup"><span data-stu-id="b5aba-250">Renders an individual person search result.</span></span> |
