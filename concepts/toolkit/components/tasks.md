---
title: Microsoft Graph 工具包中的任务组件
description: 通过 "任务" 组件，用户可以查看、添加、删除、完成或编辑任务。 它适用于 Microsoft Planner 或 Microsoft 中的任何任务。
localization_priority: Normal
author: benotter
ms.openlocfilehash: cfd248ca7cb240cd724b8df863383b308121db4b
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144273"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具包中的任务组件

通过 "任务" 组件，用户可以查看、添加、删除、完成或编辑任务。 它与 Microsoft Planner 或 Microsoft To Do 中的任务一起使用。  

此外，用户还可以将一个或多个 Microsoft Graph 用户分配给一个任务。 有关 Microsoft Graph 分配的更多详细信息，请参阅[plannerAssignments](https://docs.microsoft.com/graph/api/resources/plannerassignments?view=graph-rest-1.0)。

## <a name="example"></a>示例

下面的示例使用`mgt-tasks`组件显示已登录用户的 Microsoft Planner 任务。 您可以使用代码编辑器来查看[属性](#properties)如何更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[在 "dev" 中打开此示例](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a>属性

| 属性 | 属性 | 说明 |
| -- | -- | -- |
| 数据源 = "todo/planner" | dataSource | 用于配置任务的数据源的枚举-Microsoft To Do 或 Microsoft Planner。 默认值为 `planner`。 |
| 只读 | 只读 | 一个布尔值，用于将任务接口设置为只读（不添加或删除任务）。 默认值为 `false`。 |
| 隐藏-页眉 | hideHeader | 一个 Boolean 类型的值，用于显示或隐藏组件的标题。 默认值为 `false`。 |
| 隐藏-选项 | hideOptions | 一个 Boolean 类型的值，用于显示或隐藏任务中的选项。 默认值为 `false`。
| 初始 id = "planner_id/folder_id" | initialId | 一个字符串 ID，用于将最初显示的 planner 或文件夹设置为所提供的 ID。 |
| 初始存储桶-id = "bucket_id" | initialBucketId | 一个字符串 ID，用于将最初显示的存储桶（仅 Planner 数据源）设置为提供的 ID。 |
| 目标-id = "planner_id/folder_id"| targetId | 一个字符串 ID，用于将任务界面锁定为提供的 planner 或文件夹 ID。 |
| 目标存储段-id = "bucket_id" |targetBucketId  | 一个字符串 ID，用于将任务接口锁定为提供的存储桶 ID （仅 Planner 数据源）。 |
| 组 id | groupId  | 一个字符串 ID，用于将任务接口锁定到组 ID （仅限 Planner 数据源）。 |
| 不适用 | isNewTaskVisible  | 确定新任务视图在呈现时是否可见。 |
| 不适用 | taskFilter  | 一个可选函数，用于筛选向用户显示的任务。 |

下面的示例仅演示来自 ID 为*12345*的 Planner 的任务，并且不允许用户创建新任务。

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

下面的示例演示如何筛选仅具有*category3*集的任务。

```js
let taskView = document.querySelector('mgt-tasks');
taskView.taskFilter = task => task.appliedCategories.category3 === true;
```

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

## <a name="events"></a>事件
| 事件 | 详细信息 | 说明 |
| --- | --- | --- |
| taskClick | 详细信息包含各自`task`的对象 | 当用户单击或点击某项任务时激发。 |

## <a name="templates"></a>模板

组件支持多个[模板](../templates.md)，这些模板允许您替换组件的某些部分。 `tasks` 若要指定模板，请在`<template>`组件内添加一个元素，并`data-type`将值设置为下列值之一：

| 数据类型     | 数据上下文              | 说明                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | 任务： planner 或待办事项任务对象 | 替换整个默认任务。 |
| 任务-详细信息 | 任务： planner 或待办事项任务对象 | 模板将替换该任务的 "详细信息" 部分。 |

下面的示例定义了 tasks 组件的模板。

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

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用以下 Microsoft Graph Api 和权限。

| 资源 | 权限 |
| - | - |
| /me/planner/plans | Group.Read.All |
| /planner/plans/$ {id} | Group.Read.All、Group.ReadWrite.All |
| /planner/tasks | Group.ReadWrite.All |
| /me/outlook/taskGroups | Tasks.Read |
| /me/outlook/taskFolders | Read、Task、ReadWrite |
| /me/outlook/tasks | Tasks.ReadWrite |
| /groups/$ {group-id}/planner/plans | Group.Read.All、Group.ReadWrite.All |

对于 Microsoft Planner 数据源，提取和读取任务需要组。读取。所有权限。 添加、更新或删除任务需要组的 ReadWrite。所有权限。

对于 Microsoft Todo 数据源，需要执行任务。读取和读取任务需要读取权限。 添加、更新或删除任务需要任务的 ReadWrite 权限。

## <a name="authentication"></a>身份验证

"任务" 组件使用[身份验证文档](./../providers.md)中介绍的全局身份验证提供程序。
