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
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的任务组件

通过 "任务" 组件, 用户可以查看、添加、删除、完成或编辑任务。 它与 Microsoft Planner 或 Microsoft To Do 中的任务一起使用。

## <a name="example"></a>示例

[jsfiddle 示例](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a>属性

| 属性 | 属性 | 说明 |
| -- | -- | -- |
| `dataSource` | `data-source="todo/planner"` | 设置任务的数据源-是 Microsoft To Do, 或 Microsoft Planner。 默认值为 `planner`。 |
| `readOnly` | `read-only` | 将任务接口设置为只读 (不添加或删除任务)。 默认值为 `false`。 |
| `initialId` | `initial-id="planner_id/folder_id"` | 将最初显示的 planner 或文件夹设置为提供的 ID。 |
| `initialBucketId` | `initial-bucket-id="bucket_id"` | 将最初显示的存储桶 (仅 Planner 数据源) 设置为提供的 ID。 |
| `targetId` | `target-id="planner_id/folder_id"` | 将任务界面锁定为提供的 planner 或文件夹 ID。 |
| `targetBucketId` | `target-bucket-id="bucket_id"` | 将 tasks 接口锁定为提供的存储桶 ID (仅 Planner 数据源)。 |

示例如下。

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a>自定义 CSS 变量

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

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用以下 Microsoft Graph Api 和权限。

| 资源 | 权限/范围 |
| - | - |
| /me/planner/plans | `Group.Read.All` |
| /planner/plans/$ {id} | `Group.Read.All`, `Group.ReadWrite.All` |
| /planner/tasks | `Group.ReadWrite.All` |
| /me/outlook/taskGroups | `Tasks.Read` |
| /me/outlook/taskFolders | `Tasks.Read`, `Tasks.ReadWrite` |
| /me/outlook/tasks | `Tasks.ReadWrite` |

对于 Microsoft Planner 数据源, 提取和读取任务需要组。读取。所有权限。 添加、更新或删除任务需要组的 ReadWrite。所有权限。

对于 Microsoft Todo 数据源, 需要执行任务。读取和读取任务需要读取权限。 添加、更新或删除任务需要任务的 ReadWrite 权限。

## <a name="authentication"></a>身份验证

"任务" 组件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。
