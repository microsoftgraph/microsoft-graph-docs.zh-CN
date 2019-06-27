---
title: Microsoft Graph 工具包中的任务组件
description: 通过 "任务" 组件, 用户可以查看、添加、删除、完成或编辑任务。 它适用于 Microsoft Planner 或 Microsoft 中的任何任务。
localization_priority: Normal
author: benotter
ms.openlocfilehash: 3c2017acd7fe054c71a609c8d908e119e12a590b
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35242968"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="47b95-104">Microsoft Graph 工具包中的任务组件</span><span class="sxs-lookup"><span data-stu-id="47b95-104">Tasks component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="47b95-105">通过 "任务" 组件, 用户可以查看、添加、删除、完成或编辑任务。</span><span class="sxs-lookup"><span data-stu-id="47b95-105">The Tasks component enables the user to view, add, remove, complete, or edit tasks.</span></span> <span data-ttu-id="47b95-106">它与 Microsoft Planner 或 Microsoft To Do 中的任务一起使用。</span><span class="sxs-lookup"><span data-stu-id="47b95-106">It works with tasks in Microsoft Planner or Microsoft To-Do.</span></span>

## <a name="example"></a><span data-ttu-id="47b95-107">示例</span><span class="sxs-lookup"><span data-stu-id="47b95-107">Example</span></span>

[<span data-ttu-id="47b95-108">jsfiddle 示例</span><span class="sxs-lookup"><span data-stu-id="47b95-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a><span data-ttu-id="47b95-109">属性</span><span class="sxs-lookup"><span data-stu-id="47b95-109">Properties</span></span>

| <span data-ttu-id="47b95-110">属性</span><span class="sxs-lookup"><span data-stu-id="47b95-110">Property</span></span> | <span data-ttu-id="47b95-111">属性</span><span class="sxs-lookup"><span data-stu-id="47b95-111">Attribute</span></span> | <span data-ttu-id="47b95-112">说明</span><span class="sxs-lookup"><span data-stu-id="47b95-112">Description</span></span> |
| -- | -- | -- |
| `dataSource` | `data-source="todo/planner"` | <span data-ttu-id="47b95-113">设置任务的数据源-是 Microsoft To Do, 或 Microsoft Planner。</span><span class="sxs-lookup"><span data-stu-id="47b95-113">Sets the data source for tasks - either Microsoft To-Do, or Microsoft Planner.</span></span> <span data-ttu-id="47b95-114">默认值为 `planner`。</span><span class="sxs-lookup"><span data-stu-id="47b95-114">Default is `planner`.</span></span> |
| `readOnly` | `read-only` | <span data-ttu-id="47b95-115">将任务接口设置为只读 (不添加或删除任务)。</span><span class="sxs-lookup"><span data-stu-id="47b95-115">Sets the task interface to be read only (no adding or removing tasks).</span></span> <span data-ttu-id="47b95-116">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="47b95-116">Default is `false`.</span></span> |
| `initialId` | `initial-id="planner_id/folder_id"` | <span data-ttu-id="47b95-117">将最初显示的 planner 或文件夹设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="47b95-117">Sets the initially displayed planner or folder to the provided ID.</span></span> |
| `initialBucketId` | `initial-bucket-id="bucket_id"` | <span data-ttu-id="47b95-118">将最初显示的存储桶 (仅 Planner 数据源) 设置为提供的 ID。</span><span class="sxs-lookup"><span data-stu-id="47b95-118">Sets the initially displayed bucket (Planner Data-Source Only) to the provided ID.</span></span> |
| `targetId` | `target-id="planner_id/folder_id"` | <span data-ttu-id="47b95-119">将任务界面锁定为提供的 planner 或文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="47b95-119">Locks the tasks interface to the provided planner or folder ID.</span></span> |
| `targetBucketId` | `target-bucket-id="bucket_id"` | <span data-ttu-id="47b95-120">将 tasks 接口锁定为提供的存储桶 ID (仅 Planner 数据源)。</span><span class="sxs-lookup"><span data-stu-id="47b95-120">Locks the tasks interface to the provided bucket ID (Planner Data-Source Only).</span></span> |

<span data-ttu-id="47b95-121">示例如下。</span><span class="sxs-lookup"><span data-stu-id="47b95-121">The following is an example.</span></span>

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a><span data-ttu-id="47b95-122">自定义 CSS 变量</span><span class="sxs-lookup"><span data-stu-id="47b95-122">Custom CSS variables</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="47b95-123">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="47b95-123">Microsoft Graph permissions</span></span>

<span data-ttu-id="47b95-124">此控件使用以下 Microsoft Graph Api 和权限。</span><span class="sxs-lookup"><span data-stu-id="47b95-124">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="47b95-125">资源</span><span class="sxs-lookup"><span data-stu-id="47b95-125">Resource</span></span> | <span data-ttu-id="47b95-126">权限/范围</span><span class="sxs-lookup"><span data-stu-id="47b95-126">Permission/scope</span></span> |
| - | - |
| <span data-ttu-id="47b95-127">/me/planner/plans</span><span class="sxs-lookup"><span data-stu-id="47b95-127">/me/planner/plans</span></span> | `Group.Read.All` |
| <span data-ttu-id="47b95-128">/planner/plans/$ {id}</span><span class="sxs-lookup"><span data-stu-id="47b95-128">/planner/plans/${id}</span></span> | <span data-ttu-id="47b95-129">`Group.Read.All`, `Group.ReadWrite.All`</span><span class="sxs-lookup"><span data-stu-id="47b95-129"></span></span> |
| <span data-ttu-id="47b95-130">/planner/tasks</span><span class="sxs-lookup"><span data-stu-id="47b95-130">/planner/tasks</span></span> | `Group.ReadWrite.All` |
| <span data-ttu-id="47b95-131">/me/outlook/taskGroups</span><span class="sxs-lookup"><span data-stu-id="47b95-131">/me/outlook/taskGroups</span></span> | `Tasks.Read` |
| <span data-ttu-id="47b95-132">/me/outlook/taskFolders</span><span class="sxs-lookup"><span data-stu-id="47b95-132">/me/outlook/taskFolders</span></span> | <span data-ttu-id="47b95-133">`Tasks.Read`, `Tasks.ReadWrite`</span><span class="sxs-lookup"><span data-stu-id="47b95-133"></span></span> |
| <span data-ttu-id="47b95-134">/me/outlook/tasks</span><span class="sxs-lookup"><span data-stu-id="47b95-134">/me/outlook/tasks</span></span> | `Tasks.ReadWrite` |

<span data-ttu-id="47b95-135">对于 Microsoft Planner 数据源, 提取和读取任务需要组。读取。所有权限。</span><span class="sxs-lookup"><span data-stu-id="47b95-135">For the Microsoft Planner data source, fetching and reading tasks requires the Groups.Read.All permission.</span></span> <span data-ttu-id="47b95-136">添加、更新或删除任务需要组的 ReadWrite。所有权限。</span><span class="sxs-lookup"><span data-stu-id="47b95-136">Adding, updating, or removing tasks requires the Groups.ReadWrite.All permission.</span></span>

<span data-ttu-id="47b95-137">对于 Microsoft Todo 数据源, 需要执行任务。读取和读取任务需要读取权限。</span><span class="sxs-lookup"><span data-stu-id="47b95-137">For the Microsoft Todo data source, the Tasks.Read permission is required for fetching and reading tasks.</span></span> <span data-ttu-id="47b95-138">添加、更新或删除任务需要任务的 ReadWrite 权限。</span><span class="sxs-lookup"><span data-stu-id="47b95-138">Adding, updating, or removing tasks requires the Tasks.ReadWrite permission.</span></span>

## <a name="authentication"></a><span data-ttu-id="47b95-139">身份验证</span><span class="sxs-lookup"><span data-stu-id="47b95-139">Authentication</span></span>

<span data-ttu-id="47b95-140">"任务" 组件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。</span><span class="sxs-lookup"><span data-stu-id="47b95-140">The tasks component uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>
