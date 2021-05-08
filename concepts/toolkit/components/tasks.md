---
title: Microsoft Graph 服务中的任务Toolkit
description: 任务组件使用户能够查看、添加、删除、完成或编辑任务。 它适用于 Microsoft Planner 中的任何任务。
localization_priority: Normal
author: benotter
ms.openlocfilehash: d07db8f1a261f1cff96175a25665f08eff615d67
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266799"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="39d1a-104">Microsoft Graph 服务中的任务Toolkit</span><span class="sxs-lookup"><span data-stu-id="39d1a-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="39d1a-105">任务组件使用户能够查看、添加、删除、完成或编辑 Microsoft Planner 中的任务。</span><span class="sxs-lookup"><span data-stu-id="39d1a-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks from Microsoft Planner.</span></span>  

<span data-ttu-id="39d1a-106">此外，用户能够向任务分配一个或多个 Microsoft Graph 用户。</span><span class="sxs-lookup"><span data-stu-id="39d1a-106">In addition, a user is able to assign a single or multiple Microsoft Graph users to a task.</span></span> <span data-ttu-id="39d1a-107">有关 Microsoft Graph 作业的更多详细信息，请参阅 [plannerAssignments](/graph/api/resources/plannerassignments)。</span><span class="sxs-lookup"><span data-stu-id="39d1a-107">For more details about Microsoft Graph assignments, see [plannerAssignments](/graph/api/resources/plannerassignments).</span></span>

## <a name="example"></a><span data-ttu-id="39d1a-108">示例</span><span class="sxs-lookup"><span data-stu-id="39d1a-108">Example</span></span>

<span data-ttu-id="39d1a-109">以下示例使用 组件显示已登录用户的 Microsoft Planner `mgt-tasks` 任务。</span><span class="sxs-lookup"><span data-stu-id="39d1a-109">The following example displays the signed-in user's Microsoft Planner tasks using the `mgt-tasks` component.</span></span> <span data-ttu-id="39d1a-110">可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。</span><span class="sxs-lookup"><span data-stu-id="39d1a-110">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[<span data-ttu-id="39d1a-111">在"打开"mgt.dev</span><span class="sxs-lookup"><span data-stu-id="39d1a-111">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a><span data-ttu-id="39d1a-112">属性</span><span class="sxs-lookup"><span data-stu-id="39d1a-112">Properties</span></span>

| <span data-ttu-id="39d1a-113">属性</span><span class="sxs-lookup"><span data-stu-id="39d1a-113">Attribute</span></span> | <span data-ttu-id="39d1a-114">属性</span><span class="sxs-lookup"><span data-stu-id="39d1a-114">Property</span></span> | <span data-ttu-id="39d1a-115">说明</span><span class="sxs-lookup"><span data-stu-id="39d1a-115">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="39d1a-116">只读</span><span class="sxs-lookup"><span data-stu-id="39d1a-116">read-only</span></span> | <span data-ttu-id="39d1a-117">readOnly</span><span class="sxs-lookup"><span data-stu-id="39d1a-117">readOnly</span></span> | <span data-ttu-id="39d1a-118">一个布尔值，用于将任务界面设置为只读， (添加或删除任务) 。</span><span class="sxs-lookup"><span data-stu-id="39d1a-118">A Boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="39d1a-119">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="39d1a-119">Default is `false`.</span></span> |
| <span data-ttu-id="39d1a-120">hide-header</span><span class="sxs-lookup"><span data-stu-id="39d1a-120">hide-header</span></span> | <span data-ttu-id="39d1a-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="39d1a-121">hideHeader</span></span> | <span data-ttu-id="39d1a-122">显示或隐藏组件标头的布尔值。</span><span class="sxs-lookup"><span data-stu-id="39d1a-122">A Boolean to show or hide the header of the component.</span></span> <span data-ttu-id="39d1a-123">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="39d1a-123">Default is `false`.</span></span> |
| <span data-ttu-id="39d1a-124">hide-options</span><span class="sxs-lookup"><span data-stu-id="39d1a-124">hide-options</span></span> | <span data-ttu-id="39d1a-125">hideOptions</span><span class="sxs-lookup"><span data-stu-id="39d1a-125">hideOptions</span></span> | <span data-ttu-id="39d1a-126">用于显示或隐藏任务中的选项的布尔值。</span><span class="sxs-lookup"><span data-stu-id="39d1a-126">A Boolean to show or hide the options in tasks.</span></span> <span data-ttu-id="39d1a-127">默认值为“`false`”。</span><span class="sxs-lookup"><span data-stu-id="39d1a-127">Default is `false`.</span></span>
| <span data-ttu-id="39d1a-128">initial-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="39d1a-128">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="39d1a-129">initialId</span><span class="sxs-lookup"><span data-stu-id="39d1a-129">initialId</span></span> | <span data-ttu-id="39d1a-130">一个字符串 ID，用于将最初显示的规划器或文件夹设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="39d1a-130">A string ID to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="39d1a-131">initial-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="39d1a-131">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="39d1a-132">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="39d1a-132">initialBucketId</span></span> | <span data-ttu-id="39d1a-133">一个字符串 ID，用于将最初显示的存储桶 (Planner Data-Source仅) 设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="39d1a-133">A string ID to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="39d1a-134">target-id="planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="39d1a-134">target-id="planner_id/folder_id"</span></span>| <span data-ttu-id="39d1a-135">targetId</span><span class="sxs-lookup"><span data-stu-id="39d1a-135">targetId</span></span> | <span data-ttu-id="39d1a-136">一个字符串 ID，用于将任务接口锁定为提供的规划器或文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="39d1a-136">A string ID to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="39d1a-137">target-bucket-id="bucket_id"</span><span class="sxs-lookup"><span data-stu-id="39d1a-137">target-bucket-id="bucket_id"</span></span> |<span data-ttu-id="39d1a-138">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="39d1a-138">targetBucketId</span></span>  | <span data-ttu-id="39d1a-139">一个字符串 ID，用于将任务接口锁定为 Planner (提供的Data-Source ID) 。</span><span class="sxs-lookup"><span data-stu-id="39d1a-139">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |
| <span data-ttu-id="39d1a-140">group-id</span><span class="sxs-lookup"><span data-stu-id="39d1a-140">group-id</span></span> | <span data-ttu-id="39d1a-141">groupId</span><span class="sxs-lookup"><span data-stu-id="39d1a-141">groupId</span></span>  | <span data-ttu-id="39d1a-142">用于将任务接口锁定为组 ID 的字符串 ID。</span><span class="sxs-lookup"><span data-stu-id="39d1a-142">A string ID to lock the tasks interface to the group ID.</span></span> |
| <span data-ttu-id="39d1a-143">不适用</span><span class="sxs-lookup"><span data-stu-id="39d1a-143">N/A</span></span> | <span data-ttu-id="39d1a-144">isNewTaskVisible</span><span class="sxs-lookup"><span data-stu-id="39d1a-144">isNewTaskVisible</span></span>  | <span data-ttu-id="39d1a-145">确定新任务视图在呈现时是否可见。</span><span class="sxs-lookup"><span data-stu-id="39d1a-145">Determines whether new task view is visible at render.</span></span> |
| <span data-ttu-id="39d1a-146">不适用</span><span class="sxs-lookup"><span data-stu-id="39d1a-146">N/A</span></span> | <span data-ttu-id="39d1a-147">taskFilter</span><span class="sxs-lookup"><span data-stu-id="39d1a-147">taskFilter</span></span>  | <span data-ttu-id="39d1a-148">可选函数，用于筛选向用户显示的任务。</span><span class="sxs-lookup"><span data-stu-id="39d1a-148">An optional function to filter which tasks are shown to the user.</span></span> |

<span data-ttu-id="39d1a-149">以下示例仅显示来自 ID *为 12345* 的 Planner 中的任务，并且不允许用户创建新任务。</span><span class="sxs-lookup"><span data-stu-id="39d1a-149">The following example shows only tasks from Planner with ID *12345* and does not allow the user to create new tasks.</span></span>

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

<span data-ttu-id="39d1a-150">以下示例演示如何筛选仅设置了 *category3* 的任务。</span><span class="sxs-lookup"><span data-stu-id="39d1a-150">The following example shows how to filter tasks that only have *category3* set.</span></span>

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

## <a name="custom-css-variables"></a><span data-ttu-id="39d1a-151">自定义 CSS 变量</span><span class="sxs-lookup"><span data-stu-id="39d1a-151">Custom CSS variables</span></span>

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

## <a name="events"></a><span data-ttu-id="39d1a-152">事件</span><span class="sxs-lookup"><span data-stu-id="39d1a-152">Events</span></span>
| <span data-ttu-id="39d1a-153">事件</span><span class="sxs-lookup"><span data-stu-id="39d1a-153">Event</span></span> | <span data-ttu-id="39d1a-154">详情</span><span class="sxs-lookup"><span data-stu-id="39d1a-154">Detail</span></span> | <span data-ttu-id="39d1a-155">说明</span><span class="sxs-lookup"><span data-stu-id="39d1a-155">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="39d1a-156">taskAdded</span><span class="sxs-lookup"><span data-stu-id="39d1a-156">taskAdded</span></span> | <span data-ttu-id="39d1a-157">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="39d1a-157">The detail contains the respective `task` object</span></span> | <span data-ttu-id="39d1a-158">新建任务后触发。</span><span class="sxs-lookup"><span data-stu-id="39d1a-158">Fires when a new task has been created.</span></span> |
| <span data-ttu-id="39d1a-159">taskChanged</span><span class="sxs-lookup"><span data-stu-id="39d1a-159">taskChanged</span></span> | <span data-ttu-id="39d1a-160">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="39d1a-160">The detail contains the respective `task` object</span></span> | <span data-ttu-id="39d1a-161">更改任务元数据（如标记已完成）时触发。</span><span class="sxs-lookup"><span data-stu-id="39d1a-161">Fires when task metadata has been changed, such as marking completed.</span></span> |
| <span data-ttu-id="39d1a-162">taskClick</span><span class="sxs-lookup"><span data-stu-id="39d1a-162">taskClick</span></span> | <span data-ttu-id="39d1a-163">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="39d1a-163">The detail contains the respective `task` object</span></span> | <span data-ttu-id="39d1a-164">当用户单击或点击任务时触发。</span><span class="sxs-lookup"><span data-stu-id="39d1a-164">Fires when the user clicks or taps on a task.</span></span> |
| <span data-ttu-id="39d1a-165">taskRemoved</span><span class="sxs-lookup"><span data-stu-id="39d1a-165">taskRemoved</span></span> | <span data-ttu-id="39d1a-166">详细信息包含各自的 `task` 对象</span><span class="sxs-lookup"><span data-stu-id="39d1a-166">The detail contains the respective `task` object</span></span> | <span data-ttu-id="39d1a-167">删除现有任务后触发。</span><span class="sxs-lookup"><span data-stu-id="39d1a-167">Fires when an existing task has been deleted.</span></span> |

## <a name="templates"></a><span data-ttu-id="39d1a-168">模板</span><span class="sxs-lookup"><span data-stu-id="39d1a-168">Templates</span></span>

<span data-ttu-id="39d1a-169">组件 `tasks` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。</span><span class="sxs-lookup"><span data-stu-id="39d1a-169">The `tasks` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="39d1a-170">若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="39d1a-170">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="39d1a-171">数据类型</span><span class="sxs-lookup"><span data-stu-id="39d1a-171">Data type</span></span>     | <span data-ttu-id="39d1a-172">数据上下文</span><span class="sxs-lookup"><span data-stu-id="39d1a-172">Data context</span></span>              | <span data-ttu-id="39d1a-173">说明</span><span class="sxs-lookup"><span data-stu-id="39d1a-173">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="39d1a-174">task</span><span class="sxs-lookup"><span data-stu-id="39d1a-174">task</span></span>     | <span data-ttu-id="39d1a-175">任务：计划工具任务对象</span><span class="sxs-lookup"><span data-stu-id="39d1a-175">task: a planner task object</span></span> | <span data-ttu-id="39d1a-176">替换整个默认任务。</span><span class="sxs-lookup"><span data-stu-id="39d1a-176">replaces the whole default task.</span></span> |
| <span data-ttu-id="39d1a-177">task-details</span><span class="sxs-lookup"><span data-stu-id="39d1a-177">task-details</span></span> | <span data-ttu-id="39d1a-178">任务：计划工具任务对象</span><span class="sxs-lookup"><span data-stu-id="39d1a-178">task: a planner task object</span></span> | <span data-ttu-id="39d1a-179">template 将替换任务的详细信息部分。</span><span class="sxs-lookup"><span data-stu-id="39d1a-179">template replaces the details section of the task.</span></span> |

<span data-ttu-id="39d1a-180">下面的示例定义任务组件的模板。</span><span class="sxs-lookup"><span data-stu-id="39d1a-180">The following example defines a template for the tasks component.</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="39d1a-181">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="39d1a-181">Microsoft Graph permissions</span></span>

<span data-ttu-id="39d1a-182">此控件使用下列 Microsoft Graph API 和权限。</span><span class="sxs-lookup"><span data-stu-id="39d1a-182">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="39d1a-183">Resource</span><span class="sxs-lookup"><span data-stu-id="39d1a-183">Resource</span></span> | <span data-ttu-id="39d1a-184">权限</span><span class="sxs-lookup"><span data-stu-id="39d1a-184">Permission</span></span> |
| - | - |
| <span data-ttu-id="39d1a-185">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="39d1a-185">/me/planner/plans</span></span> | <span data-ttu-id="39d1a-186">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="39d1a-186">Group.Read.All</span></span> |
| <span data-ttu-id="39d1a-187">/planner/plans/${id}</span><span class="sxs-lookup"><span data-stu-id="39d1a-187">/planner/plans/${id}</span></span> | <span data-ttu-id="39d1a-188">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d1a-188">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="39d1a-189">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="39d1a-189">/planner/tasks</span></span> | <span data-ttu-id="39d1a-190">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d1a-190">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="39d1a-191">/groups/${group-id}/planner/plans</span><span class="sxs-lookup"><span data-stu-id="39d1a-191">/groups/${group-id}/planner/plans</span></span> | <span data-ttu-id="39d1a-192">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d1a-192">Group.Read.All, Group.ReadWrite.All</span></span> |

<span data-ttu-id="39d1a-193">对于 Microsoft Planner 数据源，提取和读取任务需要 Groups.Read.All 权限。</span><span class="sxs-lookup"><span data-stu-id="39d1a-193">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="39d1a-194">添加、更新或删除任务需要 Groups.ReadWrite.All 权限。</span><span class="sxs-lookup"><span data-stu-id="39d1a-194">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="39d1a-195">身份验证</span><span class="sxs-lookup"><span data-stu-id="39d1a-195">Authentication</span></span>

<span data-ttu-id="39d1a-196">任务组件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。</span><span class="sxs-lookup"><span data-stu-id="39d1a-196">The tasks component uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="39d1a-197">缓存</span><span class="sxs-lookup"><span data-stu-id="39d1a-197">Cache</span></span>

<span data-ttu-id="39d1a-198">`mgt-tasks`组件不缓存任何数据。</span><span class="sxs-lookup"><span data-stu-id="39d1a-198">The `mgt-tasks` component doesn't cache any data.</span></span>
