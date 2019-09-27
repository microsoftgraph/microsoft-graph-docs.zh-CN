---
title: Microsoft Graph 工具包中的任务组件
description: 通过 "任务" 组件，用户可以查看、添加、删除、完成或编辑任务。 它适用于 Microsoft Planner 或 Microsoft 中的任何任务。
localization_priority: Normal
author: benotter
ms.openlocfilehash: f8366842be9319e8c89d05fa23bc488cde49359a
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275820"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="c24bc-104">Microsoft Graph 工具包中的任务组件</span><span class="sxs-lookup"><span data-stu-id="c24bc-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="c24bc-105">通过 "任务" 组件，用户可以查看、添加、删除、完成或编辑任务。</span><span class="sxs-lookup"><span data-stu-id="c24bc-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="c24bc-106">它与 Microsoft Planner 或 Microsoft To Do 中的任务一起使用。</span><span class="sxs-lookup"><span data-stu-id="c24bc-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>

## <a name="example"></a><span data-ttu-id="c24bc-107">示例</span><span class="sxs-lookup"><span data-stu-id="c24bc-107">Example</span></span>

[<span data-ttu-id="c24bc-108">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="c24bc-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="c24bc-109">属性</span><span class="sxs-lookup"><span data-stu-id="c24bc-109">Properties</span></span>

| <span data-ttu-id="c24bc-110">属性</span><span class="sxs-lookup"><span data-stu-id="c24bc-110">Property</span></span> | <span data-ttu-id="c24bc-111">属性</span><span class="sxs-lookup"><span data-stu-id="c24bc-111">Attribute</span></span> | <span data-ttu-id="c24bc-112">说明</span><span class="sxs-lookup"><span data-stu-id="c24bc-112">Description</span></span> |
| -- | -- | -- |
| <span data-ttu-id="c24bc-113">dataSource</span><span class="sxs-lookup"><span data-stu-id="c24bc-113">dataSource</span></span> | <span data-ttu-id="c24bc-114">数据源 = "todo/planner"</span><span class="sxs-lookup"><span data-stu-id="c24bc-114">data-source="todo/planner"</span></span> | <span data-ttu-id="c24bc-115">用于配置任务的数据源的枚举-Microsoft To Do 或 Microsoft Planner。</span><span class="sxs-lookup"><span data-stu-id="c24bc-115">An enumeration to configure the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="c24bc-116">默认值为 `planner`。</span><span class="sxs-lookup"><span data-stu-id="c24bc-116">Default is `planner`.</span></span> |
| <span data-ttu-id="c24bc-117">只读</span><span class="sxs-lookup"><span data-stu-id="c24bc-117">readOnly</span></span> | <span data-ttu-id="c24bc-118">只读</span><span class="sxs-lookup"><span data-stu-id="c24bc-118">read-only</span></span> | <span data-ttu-id="c24bc-119">一个布尔值，用于将任务接口设置为只读（不添加或删除任务）。</span><span class="sxs-lookup"><span data-stu-id="c24bc-119">A boolean to set the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="c24bc-120">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="c24bc-120">Default is `false`.</span></span> |
| <span data-ttu-id="c24bc-121">hideHeader</span><span class="sxs-lookup"><span data-stu-id="c24bc-121">hideHeader</span></span> | <span data-ttu-id="c24bc-122">隐藏-页眉</span><span class="sxs-lookup"><span data-stu-id="c24bc-122">hide-header</span></span> | <span data-ttu-id="c24bc-123">一个 boolean 类型的值，用于显示或隐藏组件的标题。</span><span class="sxs-lookup"><span data-stu-id="c24bc-123">A boolean to show or hide the header of the component.</span></span> <span data-ttu-id="c24bc-124">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="c24bc-124">Default is `false`.</span></span> |
| <span data-ttu-id="c24bc-125">initialId</span><span class="sxs-lookup"><span data-stu-id="c24bc-125">initialId</span></span> | <span data-ttu-id="c24bc-126">初始 id = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="c24bc-126">initial-id="planner_id/folder_id"</span></span> | <span data-ttu-id="c24bc-127">一个字符串 id，用于将最初显示的 planner 或文件夹设置为所提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="c24bc-127">A string id to set the initially displayed planner or folder to the provided ID.</span></span> |
| <span data-ttu-id="c24bc-128">initialBucketId</span><span class="sxs-lookup"><span data-stu-id="c24bc-128">initialBucketId</span></span> | <span data-ttu-id="c24bc-129">初始存储桶-id = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="c24bc-129">initial-bucket-id="bucket_id"</span></span> | <span data-ttu-id="c24bc-130">一个字符串 id，用于将最初显示的存储桶（仅 Planner 数据源）设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="c24bc-130">A string id to set the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| <span data-ttu-id="c24bc-131">targetId</span><span class="sxs-lookup"><span data-stu-id="c24bc-131">targetId</span></span> | <span data-ttu-id="c24bc-132">目标-id = "planner_id/folder_id"</span><span class="sxs-lookup"><span data-stu-id="c24bc-132">target-id="planner_id/folder_id"</span></span> | <span data-ttu-id="c24bc-133">一个字符串 id，用于将任务界面锁定为提供的 planner 或文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="c24bc-133">A string id to lock the tasks interface to the provided planner or folder ID.</span></span> |
| <span data-ttu-id="c24bc-134">targetBucketId</span><span class="sxs-lookup"><span data-stu-id="c24bc-134">targetBucketId</span></span> | <span data-ttu-id="c24bc-135">目标存储桶-id = "bucket_id"</span><span class="sxs-lookup"><span data-stu-id="c24bc-135">target-bucket-id="bucket_id"</span></span> | <span data-ttu-id="c24bc-136">一个字符串 ID，用于将任务接口锁定为提供的存储桶 ID （仅 Planner 数据源）。</span><span class="sxs-lookup"><span data-stu-id="c24bc-136">A string ID to lock the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |

<span data-ttu-id="c24bc-137">示例如下。</span><span class="sxs-lookup"><span data-stu-id="c24bc-137">The following is an example.</span></span>

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a><span data-ttu-id="c24bc-138">自定义 CSS 变量</span><span class="sxs-lookup"><span data-stu-id="c24bc-138">Custom CSS variables</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="c24bc-139">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="c24bc-139">Microsoft Graph permissions</span></span>

<span data-ttu-id="c24bc-140">此控件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="c24bc-140">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="c24bc-141">资源</span><span class="sxs-lookup"><span data-stu-id="c24bc-141">Resource</span></span> | <span data-ttu-id="c24bc-142">权限</span><span class="sxs-lookup"><span data-stu-id="c24bc-142">Permission</span></span> |
| - | - |
| <span data-ttu-id="c24bc-143">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="c24bc-143">/me/planner/plans</span></span> | <span data-ttu-id="c24bc-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c24bc-144">Group.Read.All</span></span> |
| <span data-ttu-id="c24bc-145">/planner/plans/$ {id}</span><span class="sxs-lookup"><span data-stu-id="c24bc-145">/planner/plans/${id}</span></span> | <span data-ttu-id="c24bc-146">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c24bc-146">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c24bc-147">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="c24bc-147">/planner/tasks</span></span> | <span data-ttu-id="c24bc-148">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c24bc-148">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c24bc-149">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="c24bc-149">/me/outlook/taskGroups</span></span> | <span data-ttu-id="c24bc-150">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c24bc-150">Tasks.Read</span></span> |
| <span data-ttu-id="c24bc-151">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="c24bc-151">/me/outlook/taskFolders</span></span> | <span data-ttu-id="c24bc-152">Read、Task、ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c24bc-152">Tasks.Read, Tasks.ReadWrite</span></span> |
| <span data-ttu-id="c24bc-153">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="c24bc-153">/me/outlook/tasks</span></span> | <span data-ttu-id="c24bc-154">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c24bc-154">Tasks.ReadWrite</span></span> |

<span data-ttu-id="c24bc-155">对于 Microsoft Planner 数据源，提取和读取任务需要组。读取。所有权限。</span><span class="sxs-lookup"><span data-stu-id="c24bc-155">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="c24bc-156">添加、更新或删除任务需要组的 ReadWrite。所有权限。</span><span class="sxs-lookup"><span data-stu-id="c24bc-156">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="c24bc-157">对于 Microsoft Todo 数据源，需要执行任务。读取和读取任务需要读取权限。</span><span class="sxs-lookup"><span data-stu-id="c24bc-157">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="c24bc-158">添加、更新或删除任务需要任务的 ReadWrite 权限。</span><span class="sxs-lookup"><span data-stu-id="c24bc-158">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="c24bc-159">身份验证</span><span class="sxs-lookup"><span data-stu-id="c24bc-159">Authentication</span></span>

<span data-ttu-id="c24bc-160">"任务" 组件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="c24bc-160">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
