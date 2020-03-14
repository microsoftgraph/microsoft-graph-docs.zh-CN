---
title: Microsoft Graph 工具包中的任务组件
description: 通过 "任务" 组件，用户可以查看、添加、删除、完成或编辑任务。 它适用于 Microsoft Planner 或 Microsoft 中的任何任务。
localization_priority: Normal
author: benotter
ms.openlocfilehash: 80da5522b73051df4d5c264e5289845b9521058f
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639917"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="13231-104">Microsoft Graph 工具包中的任务组件</span><span class="sxs-lookup"><span data-stu-id="13231-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="13231-105">通过 "任务" 组件，用户可以查看、添加、删除、完成或编辑任务。</span><span class="sxs-lookup"><span data-stu-id="13231-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="13231-106">它与 Microsoft Planner 或 Microsoft To Do 中的任务一起使用。</span><span class="sxs-lookup"><span data-stu-id="13231-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>  

<span data-ttu-id="13231-107">此外，用户还可以将一个或多个 Microsoft Graph 用户分配给一个任务。</span><span class="sxs-lookup"><span data-stu-id="13231-107">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="13231-108">有关 Microsoft Graph 分配的更多详细信息，请参阅[plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="13231-108">For more details about Microsoft Graph assignments, see [plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0).</span></span>

## <a name="example"></a><span data-ttu-id="13231-109">示例</span><span class="sxs-lookup"><span data-stu-id="13231-109">Example</span></span>

<span data-ttu-id="13231-110">下面的示例使用`mgt-tasks`组件显示已登录用户的 Microsoft Planner 任务。</span><span class="sxs-lookup"><span data-stu-id="13231-110">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="13231-111">您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="13231-111">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="13231-112">在 "dev" 中打开此示例</span><span class="sxs-lookup"><span data-stu-id="13231-112">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="13231-113">属性</span><span class="sxs-lookup"><span data-stu-id="13231-113">Properties</span></span>

| <span data-ttu-id="13231-114">属性</span><span class="sxs-lookup"><span data-stu-id="13231-114">Attribute</span></span> | <span data-ttu-id="13231-115">属性</span><span class="sxs-lookup"><span data-stu-id="13231-115">Property</span></span> | <span data-ttu-id="13231-116">说明</span><span class="sxs-lookup"><span data-stu-id="13231-116">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="13231-117">数据源 = "todo/planner"</span><span class="sxs-lookup"><span data-stu-id="13231-117">data-source="todo/planner"</span></span> | <span data-ttu-id="13231-118">dataSource</span><span class="sxs-lookup"><span data-stu-id="13231-118">dataSource</span></span> | <span data-ttu-id="13231-119">用于配置任务的数据源的枚举-Microsoft To Do 或 Microsoft Planner。</span><span class="sxs-lookup"><span data-stu-id="13231-119">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="13231-120">默认值为 `planner`。</span><span class="sxs-lookup"><span data-stu-id="13231-120">Default is `planner`.</span></span> |
| <span data-ttu-id="13231-121">只读</span><span class="sxs-lookup"><span data-stu-id="13231-121">read-only</span></span> | <span data-ttu-id="13231-122">只读</span><span class="sxs-lookup"><span data-stu-id="13231-122">readOnly</span></span> | <span data-ttu-id="13231-123">一个布尔值，用于将任务接口设置为只读（不添加或删除任务）。</span><span class="sxs-lookup"><span data-stu-id="13231-123">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="13231-124">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="13231-124">Default is `false`.</span></span> |
| <span data-ttu-id="13231-125">隐藏-页眉</span><span class="sxs-lookup"><span data-stu-id="13231-125">hide-header</span></span> | <span data-ttu-id="13231-126">hideHeader</span><span class="sxs-lookup"><span data-stu-id="13231-126">hideHeader</span></span> | <span data-ttu-id="13231-127">一个 Boolean 类型的值，用于显示或隐藏组件的标题。</span><span class="sxs-lookup"><span data-stu-id="13231-127">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="13231-128">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="13231-128">Default is `false`.</span></span> |
| <span data-ttu-id="13231-129">初始 id = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="13231-129">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="13231-130">initialId</span><span class="sxs-lookup"><span data-stu-id="13231-130">initialId</span></span> | <span data-ttu-id="13231-131">一个字符串 ID，用于将最初显示的 planner 或文件夹设置为所提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="13231-131">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="13231-132">初始存储桶-id = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="13231-132">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="13231-133">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="13231-133">initialBucketId</span></span> | <span data-ttu-id="13231-134">一个字符串 ID，用于将最初显示的存储桶（仅 Planner 数据源）设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="13231-134">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="13231-135">目标-id = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="13231-135">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="13231-136">targetId</span><span class="sxs-lookup"><span data-stu-id="13231-136">targetId</span></span> | <span data-ttu-id="13231-137">一个字符串 ID，用于将任务界面锁定为提供的 planner 或文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="13231-137">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="13231-138">目标存储段-id = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="13231-138">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="13231-139">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="13231-139">targetBucketId</span></span>  | <span data-ttu-id="13231-140">一个字符串 ID，用于将任务接口锁定为提供的存储桶 ID （仅 Planner 数据源）。</span><span class="sxs-lookup"><span data-stu-id="13231-140">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="13231-141">组 id</span><span class="sxs-lookup"><span data-stu-id="13231-141">group-id</span></span> | <span data-ttu-id="13231-142">groupId</span><span class="sxs-lookup"><span data-stu-id="13231-142">groupId</span></span>  | <span data-ttu-id="13231-143">一个字符串 ID，用于将任务接口锁定到组 ID （仅限 Planner 数据源）。</span><span class="sxs-lookup"><span data-stu-id="13231-143">A string ID to lock the tasks interface to the group ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="13231-144">不适用</span><span class="sxs-lookup"><span data-stu-id="13231-144">N/A</span></span> | <span data-ttu-id="13231-145">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="13231-145">isNewTaskVisible</span></span>  | <span data-ttu-id="13231-146">确定新任务视图在呈现时是否可见。</span><span class="sxs-lookup"><span data-stu-id="13231-146">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="13231-147">不适用</span><span class="sxs-lookup"><span data-stu-id="13231-147">N/A</span></span> | <span data-ttu-id="13231-148">taskFilter</span><span class="sxs-lookup"><span data-stu-id="13231-148">taskFilter</span></span>  | <span data-ttu-id="13231-149">一个可选函数，用于筛选向用户显示的任务。</span><span class="sxs-lookup"><span data-stu-id="13231-149">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="13231-150">下面的示例仅演示来自 ID 为*12345*的 Planner 的任务，并且不允许用户创建新任务。</span><span class="sxs-lookup"><span data-stu-id="13231-150">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="13231-151">下面的示例演示如何筛选仅具有*category3*集的任务。</span><span class="sxs-lookup"><span data-stu-id="13231-151">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="13231-152">自定义 CSS 变量</span><span class="sxs-lookup"><span data-stu-id="13231-152">Custom CSS variables</span></span>

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
}
````

## <a name="events"></a><span data-ttu-id="13231-153">活动</span><span class="sxs-lookup"><span data-stu-id="13231-153">Events</span></span>
| <span data-ttu-id="13231-154">事件</span><span class="sxs-lookup"><span data-stu-id="13231-154">Event</span></span> | <span data-ttu-id="13231-155">详细信息</span><span class="sxs-lookup"><span data-stu-id="13231-155">Detail</span></span> | <span data-ttu-id="13231-156">说明</span><span class="sxs-lookup"><span data-stu-id="13231-156">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="13231-157">taskClick</span><span class="sxs-lookup"><span data-stu-id="13231-157">taskClick</span></span> | <span data-ttu-id="13231-158">详细信息包含各自`task`的对象</span><span class="sxs-lookup"><span data-stu-id="13231-158">The detail contains the respective `task` object</span></span> | <span data-ttu-id="13231-159">当用户单击或点击某项任务时激发。</span><span class="sxs-lookup"><span data-stu-id="13231-159">Fired when the user clicks or taps on a task.</span></span> |

## <a name="templates"></a><span data-ttu-id="13231-160">模板</span><span class="sxs-lookup"><span data-stu-id="13231-160">Templates</span></span>

<span data-ttu-id="13231-161">组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 `tasks`</span><span class="sxs-lookup"><span data-stu-id="13231-161">The `tasks` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="13231-162">若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="13231-162">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="13231-163">数据类型</span><span class="sxs-lookup"><span data-stu-id="13231-163">Data type</span></span>     | <span data-ttu-id="13231-164">数据上下文</span><span class="sxs-lookup"><span data-stu-id="13231-164">Data context</span></span>              | <span data-ttu-id="13231-165">说明</span><span class="sxs-lookup"><span data-stu-id="13231-165">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="13231-166">task</span><span class="sxs-lookup"><span data-stu-id="13231-166">task</span></span>     | <span data-ttu-id="13231-167">任务： planner 或待办事项任务对象</span><span class="sxs-lookup"><span data-stu-id="13231-167">task: a planner or to-do task object</span></span> | <span data-ttu-id="13231-168">替换整个默认任务。</span><span class="sxs-lookup"><span data-stu-id="13231-168">replaces the whole default task.</span></span> |
| <span data-ttu-id="13231-169">任务-详细信息</span><span class="sxs-lookup"><span data-stu-id="13231-169">task-details</span></span> | <span data-ttu-id="13231-170">任务： planner 或待办事项任务对象</span><span class="sxs-lookup"><span data-stu-id="13231-170">task: a planner or to-do task object</span></span> | <span data-ttu-id="13231-171">模板将替换该任务的 "详细信息" 部分。</span><span class="sxs-lookup"><span data-stu-id="13231-171">template replaces the details section of the task.</span></span> |

<span data-ttu-id="13231-172">下面的示例定义了 tasks 组件的模板。</span><span class="sxs-lookup"><span data-stu-id="13231-172">The following example defines a template for the tasks component.</span></span>

```html
    <mgt-tasks data-source="todo">
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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="13231-173">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="13231-173">Microsoft Graph permissions</span></span>

<span data-ttu-id="13231-174">此控件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="13231-174">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="13231-175">Resource</span><span class="sxs-lookup"><span data-stu-id="13231-175">Resource</span></span> | <span data-ttu-id="13231-176">权限</span><span class="sxs-lookup"><span data-stu-id="13231-176">Permission</span></span> |
| - | - |
| <span data-ttu-id="13231-177">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="13231-177">/me/planner/plans</span></span> | <span data-ttu-id="13231-178">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="13231-178">Group.Read.All</span></span> |
| <span data-ttu-id="13231-179">/planner/plans/$ {id}</span><span class="sxs-lookup"><span data-stu-id="13231-179">/planner/plans/${id}</span></span> | <span data-ttu-id="13231-180">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13231-180">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="13231-181">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="13231-181">/planner/tasks</span></span> | <span data-ttu-id="13231-182">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13231-182">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="13231-183">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="13231-183">/me/outlook/taskGroups</span></span> | <span data-ttu-id="13231-184">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="13231-184">Tasks.Read</span></span> |
| <span data-ttu-id="13231-185">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="13231-185">/me/outlook/taskFolders</span></span> | <span data-ttu-id="13231-186">Read、Task、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13231-186">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="13231-187">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="13231-187">/me/outlook/tasks</span></span> | <span data-ttu-id="13231-188">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13231-188">Tasks.ReadWrite</span></span> |
| <span data-ttu-id="13231-189">/groups/$ {group-id}/planner/plans</span><span class="sxs-lookup"><span data-stu-id="13231-189">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="13231-190">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13231-190">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="13231-191">对于 Microsoft Planner 数据源，提取和读取任务需要组。读取。所有权限。</span><span class="sxs-lookup"><span data-stu-id="13231-191">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="13231-192">添加、更新或删除任务需要组的 ReadWrite。所有权限。</span><span class="sxs-lookup"><span data-stu-id="13231-192">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="13231-193">对于 Microsoft Todo 数据源，需要执行任务。读取和读取任务需要读取权限。</span><span class="sxs-lookup"><span data-stu-id="13231-193">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="13231-194">添加、更新或删除任务需要任务的 ReadWrite 权限。</span><span class="sxs-lookup"><span data-stu-id="13231-194">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="13231-195">身份验证</span><span class="sxs-lookup"><span data-stu-id="13231-195">Authentication</span></span>

<span data-ttu-id="13231-196">"任务" 组件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="13231-196">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
