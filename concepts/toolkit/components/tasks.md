---
title: Microsoft 服务中的任务Graph Toolkit
description: 任务组件使用户能够查看、添加、删除、完成或编辑任务。 它适用于 Microsoft Planner 中的任何任务。
localization_priority: Normal
author: benotter
ms.openlocfilehash: 35191c778c957c1c9c6c316fb4755b57e6690ff2
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334736"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="58d36-104">Microsoft 服务中的任务Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="58d36-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="58d36-105">任务组件使用户能够查看、添加、删除、完成或编辑 Microsoft Planner 中的任务。</span><span class="sxs-lookup"><span data-stu-id="58d36-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks from Microsoft Planner.</span></span>  

<span data-ttu-id="58d36-106">此外，用户能够将单个或多个 Microsoft Graph分配给任务。</span><span class="sxs-lookup"><span data-stu-id="58d36-106">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="58d36-107">有关 Microsoft 工作分配Graph的详细信息，请参阅[plannerAssignments](/graph/api/resources/plannerassignments)。</span><span class="sxs-lookup"><span data-stu-id="58d36-107">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments).</span></span>

## <a name="example"></a><span data-ttu-id="58d36-108">示例</span><span class="sxs-lookup"><span data-stu-id="58d36-108">Example</span></span>

<span data-ttu-id="58d36-109">以下示例使用 组件显示已登录用户的 Microsoft Planner `mgt-tasks` 任务。</span><span class="sxs-lookup"><span data-stu-id="58d36-109">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="58d36-110">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="58d36-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="58d36-111">在 mgt.dev 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="58d36-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="58d36-112">属性</span><span class="sxs-lookup"><span data-stu-id="58d36-112">Properties</span></span>

| <span data-ttu-id="58d36-113">属性</span><span class="sxs-lookup"><span data-stu-id="58d36-113">Attribute</span></span> | <span data-ttu-id="58d36-114">属性</span><span class="sxs-lookup"><span data-stu-id="58d36-114">Property</span></span> | <span data-ttu-id="58d36-115">说明</span><span class="sxs-lookup"><span data-stu-id="58d36-115">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="58d36-116">只读</span><span class="sxs-lookup"><span data-stu-id="58d36-116">read-only</span></span> | <span data-ttu-id="58d36-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="58d36-117">readOnly</span></span> | <span data-ttu-id="58d36-118">一个布尔值，用于将任务界面设置为只读， (添加或删除任务) 。</span><span class="sxs-lookup"><span data-stu-id="58d36-118">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="58d36-119">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="58d36-119">Default is `false`.</span></span> |
| <span data-ttu-id="58d36-120">hide-header</span><span class="sxs-lookup"><span data-stu-id="58d36-120">hide-header</span></span> | <span data-ttu-id="58d36-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="58d36-121">hideHeader</span></span> | <span data-ttu-id="58d36-122">显示或隐藏组件标头的布尔值。</span><span class="sxs-lookup"><span data-stu-id="58d36-122">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="58d36-123">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="58d36-123">Default is `false`.</span></span> |
| <span data-ttu-id="58d36-124">hide-options</span><span class="sxs-lookup"><span data-stu-id="58d36-124">hide-options</span></span> | <span data-ttu-id="58d36-125">hideOptions</span><span class="sxs-lookup"><span data-stu-id="58d36-125">hideOptions</span></span> | <span data-ttu-id="58d36-126">用于显示或隐藏任务中的选项的布尔值。</span><span class="sxs-lookup"><span data-stu-id="58d36-126">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="58d36-127">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="58d36-127">Default is `false`.</span></span>
| <span data-ttu-id="58d36-128">initial-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="58d36-128">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="58d36-129">initialId</span><span class="sxs-lookup"><span data-stu-id="58d36-129">initialId</span></span> | <span data-ttu-id="58d36-130">一个字符串 ID，用于将最初显示的规划器或文件夹设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="58d36-130">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="58d36-131">initial-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="58d36-131">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="58d36-132">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="58d36-132">initialBucketId</span></span> | <span data-ttu-id="58d36-133">一个字符串 ID，用于将最初显示的存储桶 (Planner Data-Source仅) 设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="58d36-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="58d36-134">target-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="58d36-134">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="58d36-135">targetId</span><span class="sxs-lookup"><span data-stu-id="58d36-135">targetId</span></span> | <span data-ttu-id="58d36-136">一个字符串 ID，用于将任务接口锁定为提供的规划器或文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="58d36-136">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="58d36-137">target-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="58d36-137">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="58d36-138">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="58d36-138">targetBucketId</span></span>  | <span data-ttu-id="58d36-139">一个字符串 ID，用于将任务接口锁定为 Planner (提供的Data-Source ID) 。</span><span class="sxs-lookup"><span data-stu-id="58d36-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="58d36-140">group-id</span><span class="sxs-lookup"><span data-stu-id="58d36-140">group-id</span></span> | <span data-ttu-id="58d36-141">groupId</span><span class="sxs-lookup"><span data-stu-id="58d36-141">groupId</span></span>  | <span data-ttu-id="58d36-142">用于将任务接口锁定为组 ID 的字符串 ID。</span><span class="sxs-lookup"><span data-stu-id="58d36-142">A string ID to lock the tasks interface to the group ID.</span></span> |
| <span data-ttu-id="58d36-143">无</span><span class="sxs-lookup"><span data-stu-id="58d36-143">N/A</span></span> | <span data-ttu-id="58d36-144">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="58d36-144">isNewTaskVisible</span></span>  | <span data-ttu-id="58d36-145">确定新任务视图在呈现时是否可见。</span><span class="sxs-lookup"><span data-stu-id="58d36-145">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="58d36-146">无</span><span class="sxs-lookup"><span data-stu-id="58d36-146">N/A</span></span> | <span data-ttu-id="58d36-147">taskFilter</span><span class="sxs-lookup"><span data-stu-id="58d36-147">taskFilter</span></span>  | <span data-ttu-id="58d36-148">可选函数，用于筛选向用户显示的任务。</span><span class="sxs-lookup"><span data-stu-id="58d36-148">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="58d36-149">以下示例仅显示来自 ID *为 12345* 的 Planner 中的任务，并且不允许用户创建新任务。</span><span class="sxs-lookup"><span data-stu-id="58d36-149">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="58d36-150">以下示例演示如何筛选仅设置了 *category3* 的任务。</span><span class="sxs-lookup"><span data-stu-id="58d36-150">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="58d36-151">自定义 CSS 变量</span><span class="sxs-lookup"><span data-stu-id="58d36-151">Custom CSS variables</span></span>

````css
mgt-tasks {
--tasks-header-padding
--tasks-header-margin 

--tasks-title-padding
--tasks-plan-title-font-size
--tasks-plan-title-padding

--tasks-new-button-width
--tasks-new-button-height
--tasks-new-button-color
--tasks-new-button-background
--tasks-new-button-border
--tasks-new-button-hover-background
--tasks-new-button-active-background

--tasks-new-task-name-margin

--task-margin
--task-box-shadow
--task-background
--task-border

--task-header-color
--task-header-margin

--task-detail-icon-margin

--task-new-margin
--task-new-border
--task-new-line-margin
--tasks-new-line-border
--task-new-input-margin
--task-new-input-padding
--task-new-input-font-size
--task-new-input-active-border
--task-new-select-border

--task-new-add-button-background
--task-new-add-button-disabled-background
--task-new-cancel-button-color

--task-complete-background
--task-complete-border
--task-complete-header-color
--task-complete-detail-color
--task-complete-detail-icon-color

--task-icon-background-completed
--task-icon-background

--task-icon-border-completed
--task-icon-border

--task-icon-color
--task-icon-color-completed

--task-icon-border-radius

--task-icon-alignment: flex-start (default) | center | flex-end
}
````

## <a name="events"></a><span data-ttu-id="58d36-152">活动</span><span class="sxs-lookup"><span data-stu-id="58d36-152">Events</span></span>

<span data-ttu-id="58d36-153">事件</span><span class="sxs-lookup"><span data-stu-id="58d36-153">Event</span></span> | <span data-ttu-id="58d36-154">何时发出</span><span class="sxs-lookup"><span data-stu-id="58d36-154">When is it emitted</span></span> | <span data-ttu-id="58d36-155">自定义数据</span><span class="sxs-lookup"><span data-stu-id="58d36-155">Custom data</span></span> | <span data-ttu-id="58d36-156">Cancelable</span><span class="sxs-lookup"><span data-stu-id="58d36-156">Cancelable</span></span> | <span data-ttu-id="58d36-157">气泡</span><span class="sxs-lookup"><span data-stu-id="58d36-157">Bubbles</span></span> | <span data-ttu-id="58d36-158">使用自定义模板</span><span class="sxs-lookup"><span data-stu-id="58d36-158">Works with custom template</span></span>
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`taskAdded` | <span data-ttu-id="58d36-159">新建任务后触发</span><span class="sxs-lookup"><span data-stu-id="58d36-159">Fires when a new task has been created</span></span> | <span data-ttu-id="58d36-160">新创建的任务，可以是 [plannerTask](/graph/api/resources/plannertask) [我们的 outlookTask](/graph/api/resources/outlooktask)</span><span class="sxs-lookup"><span data-stu-id="58d36-160">Newly created task which can be a [plannerTask](/graph/api/resources/plannertask) our [outlookTask](/graph/api/resources/outlooktask)</span></span> | <span data-ttu-id="58d36-161">否</span><span class="sxs-lookup"><span data-stu-id="58d36-161">No</span></span> | <span data-ttu-id="58d36-162">否</span><span class="sxs-lookup"><span data-stu-id="58d36-162">No</span></span> | <span data-ttu-id="58d36-163">是</span><span class="sxs-lookup"><span data-stu-id="58d36-163">Yes</span></span>
`taskChanged` | <span data-ttu-id="58d36-164">更改任务元数据（如标记已完成）时触发</span><span class="sxs-lookup"><span data-stu-id="58d36-164">Fires when task metadata has been changed, such as marking completed</span></span> | <span data-ttu-id="58d36-165">更新的任务，可以是 [plannerTask](/graph/api/resources/plannertask) [我们的 outlookTask](/graph/api/resources/outlooktask)</span><span class="sxs-lookup"><span data-stu-id="58d36-165">Updated task which can be a [plannerTask](/graph/api/resources/plannertask) our [outlookTask](/graph/api/resources/outlooktask)</span></span> | <span data-ttu-id="58d36-166">否</span><span class="sxs-lookup"><span data-stu-id="58d36-166">No</span></span> | <span data-ttu-id="58d36-167">否</span><span class="sxs-lookup"><span data-stu-id="58d36-167">No</span></span> | <span data-ttu-id="58d36-168">否</span><span class="sxs-lookup"><span data-stu-id="58d36-168">No</span></span>
`taskClick` | <span data-ttu-id="58d36-169">当用户单击或点击任务时触发</span><span class="sxs-lookup"><span data-stu-id="58d36-169">Fires when the user clicks or taps on a task</span></span> | <span data-ttu-id="58d36-170">`task` 属性与选定的 [plannerTask](/graph/api/resources/plannertask) 我们的 [outlookTask](/graph/api/resources/outlooktask)</span><span class="sxs-lookup"><span data-stu-id="58d36-170">`task` property with the selected [plannerTask](/graph/api/resources/plannertask) our [outlookTask](/graph/api/resources/outlooktask)</span></span> | <span data-ttu-id="58d36-171">否</span><span class="sxs-lookup"><span data-stu-id="58d36-171">No</span></span> | <span data-ttu-id="58d36-172">否</span><span class="sxs-lookup"><span data-stu-id="58d36-172">No</span></span> | <span data-ttu-id="58d36-173">否</span><span class="sxs-lookup"><span data-stu-id="58d36-173">No</span></span>
`taskRemoved` | <span data-ttu-id="58d36-174">删除现有任务后触发</span><span class="sxs-lookup"><span data-stu-id="58d36-174">Fires when an existing task has been deleted</span></span> | <span data-ttu-id="58d36-175">`task` 属性与选定的 [plannerTask](/graph/api/resources/plannertask) 我们的 [outlookTask](/graph/api/resources/outlooktask)</span><span class="sxs-lookup"><span data-stu-id="58d36-175">`task` property with the selected [plannerTask](/graph/api/resources/plannertask) our [outlookTask](/graph/api/resources/outlooktask)</span></span> | <span data-ttu-id="58d36-176">否</span><span class="sxs-lookup"><span data-stu-id="58d36-176">No</span></span> | <span data-ttu-id="58d36-177">否</span><span class="sxs-lookup"><span data-stu-id="58d36-177">No</span></span> | <span data-ttu-id="58d36-178">否</span><span class="sxs-lookup"><span data-stu-id="58d36-178">No</span></span>

<span data-ttu-id="58d36-179">有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。</span><span class="sxs-lookup"><span data-stu-id="58d36-179">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="58d36-180">模板</span><span class="sxs-lookup"><span data-stu-id="58d36-180">Templates</span></span>

<span data-ttu-id="58d36-181">组件 `tasks` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="58d36-181">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="58d36-182">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="58d36-182">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="58d36-183">数据类型</span><span class="sxs-lookup"><span data-stu-id="58d36-183">Data type</span></span>     | <span data-ttu-id="58d36-184">数据上下文</span><span class="sxs-lookup"><span data-stu-id="58d36-184">Data context</span></span>              | <span data-ttu-id="58d36-185">说明</span><span class="sxs-lookup"><span data-stu-id="58d36-185">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="58d36-186">task</span><span class="sxs-lookup"><span data-stu-id="58d36-186">task</span></span>     | <span data-ttu-id="58d36-187">任务：计划工具任务对象</span><span class="sxs-lookup"><span data-stu-id="58d36-187">task: a planner task object</span></span> | <span data-ttu-id="58d36-188">替换整个默认任务。</span><span class="sxs-lookup"><span data-stu-id="58d36-188">replaces the whole default task.</span></span> |
| <span data-ttu-id="58d36-189">task-details</span><span class="sxs-lookup"><span data-stu-id="58d36-189">task-details</span></span> | <span data-ttu-id="58d36-190">任务：计划工具任务对象</span><span class="sxs-lookup"><span data-stu-id="58d36-190">task: a planner task object</span></span> | <span data-ttu-id="58d36-191">template 将替换任务的详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="58d36-191">template replaces the details section of the task.</span></span> |

<span data-ttu-id="58d36-192">下面的示例定义任务组件的模板。</span><span class="sxs-lookup"><span data-stu-id="58d36-192">The following example defines a template for the tasks component.</span></span>

```html
    <mgt-tasks>
      <template data-type="task-details">
        <div>
          Owner: {{task.owner}}
        </div>
        <div>
          Importance Level: {{task.importance}}
        </div>
      </template>
    </mgt-tasks>
```

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="58d36-193">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="58d36-193">Microsoft Graph permissions</span></span>

<span data-ttu-id="58d36-194">此控件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="58d36-194">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="58d36-195">配置</span><span class="sxs-lookup"><span data-stu-id="58d36-195">Configuration</span></span> | <span data-ttu-id="58d36-196">权限</span><span class="sxs-lookup"><span data-stu-id="58d36-196">Permission</span></span> | <span data-ttu-id="58d36-197">API</span><span class="sxs-lookup"><span data-stu-id="58d36-197">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="58d36-198">`groupId` set and `dataSource` set to `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="58d36-198">`groupId` set and `dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="58d36-199">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="58d36-199">Group.Read.All</span></span> | <span data-ttu-id="58d36-200">[/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?view=graph-rest-1.0&tabs=http)、 [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http)、 [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="58d36-200">[/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="58d36-201">`targetId` set and `dataSource` set to `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="58d36-201">`targetId` set and `dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="58d36-202">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="58d36-202">Tasks.Read</span></span> | <span data-ttu-id="58d36-203">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0) [、/me/outlook/taskGroups/${groupId}/taskFolders、/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http) [](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="58d36-203">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span></span> |
| <span data-ttu-id="58d36-204">`targetId` set and `dataSource` set to something else than `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="58d36-204">`targetId` set and `dataSource` set to something else than `TasksSource.todo`</span></span> | <span data-ttu-id="58d36-205">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="58d36-205">Group.Read.All</span></span> | <span data-ttu-id="58d36-206">[/planner/plans/${planId}](/graph/api/plannerplan-get?view=graph-rest-1.0&tabs=http)、 [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http)、 [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="58d36-206">[/planner/plans/${planId}](/graph/api/plannerplan-get?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="58d36-207">`dataSource` 设置为 `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="58d36-207">`dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="58d36-208">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="58d36-208">Group.Read.All</span></span> | <span data-ttu-id="58d36-209">[/me/planner/plans](/graph/api/planneruser-list-plans?view=graph-rest-1.0&tabs=http)、 [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http)、 [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="58d36-209">[/me/planner/plans](/graph/api/planneruser-list-plans?view=graph-rest-1.0&tabs=http), [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http), [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http)</span></span> |
| <span data-ttu-id="58d36-210">`dataSource` 设置为 `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="58d36-210">`dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="58d36-211">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="58d36-211">Tasks.Read</span></span> | <span data-ttu-id="58d36-212">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0) [、/me/outlook/taskGroups/${groupId}/taskFolders、/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http) [](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span><span class="sxs-lookup"><span data-stu-id="58d36-212">[/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0), [/me/outlook/taskGroups/${groupId}/taskFolders](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http), [/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http)</span></span> |
| <span data-ttu-id="58d36-213">`addTask` 设置为 `true` ， `dataSource` 设置为 `TasksSource.planner`</span><span class="sxs-lookup"><span data-stu-id="58d36-213">`addTask` set to `true` and `dataSource` set to `TasksSource.planner`</span></span> | <span data-ttu-id="58d36-214">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58d36-214">Group.ReadWrite.All</span></span> | [<span data-ttu-id="58d36-215">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="58d36-215">/planner/tasks</span></span>](/graph/api/planner-post-tasks?view=graph-rest-1.0&tabs=http) |
| <span data-ttu-id="58d36-216">`addTask` 设置为 `true` ， `dataSource` 设置为 `TasksSource.todo`</span><span class="sxs-lookup"><span data-stu-id="58d36-216">`addTask` set to `true` and `dataSource` set to `TasksSource.todo`</span></span> | <span data-ttu-id="58d36-217">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58d36-217">Tasks.ReadWrite</span></span> | [<span data-ttu-id="58d36-218">/me/outlook/taskFolders/${parentFolderId}/tasks</span><span class="sxs-lookup"><span data-stu-id="58d36-218">/me/outlook/taskFolders/${parentFolderId}/tasks</span></span>](/graph/api/outlookuser-post-tasks?view=graph-rest-beta&tabs=csharp) |

<span data-ttu-id="58d36-219">对于 Microsoft Planner 数据源，提取和读取任务需要 Groups.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="58d36-219">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="58d36-220">添加、更新或删除任务需要 Groups.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="58d36-220">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="58d36-221">身份验证</span><span class="sxs-lookup"><span data-stu-id="58d36-221">Authentication</span></span>

<span data-ttu-id="58d36-222">任务组件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="58d36-222">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="58d36-223">缓存</span><span class="sxs-lookup"><span data-stu-id="58d36-223">Cache</span></span>

<span data-ttu-id="58d36-224">`mgt-tasks`组件不缓存任何数据。</span><span class="sxs-lookup"><span data-stu-id="58d36-224">The `mgt-tasks` component doesn't cache any data.</span></span>
