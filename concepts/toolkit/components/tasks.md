---
title: Microsoft Graph 工具中的任务Toolkit
description: 任务组件使用户能够查看、添加、删除、完成或编辑任务。 它适用于 Microsoft Planner 中的任何任务。
localization_priority: Normal
author: benotter
ms.openlocfilehash: 5364491caae4edc9cd3f022937bcd6d809aa924f
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659212"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph 工具中的任务Toolkit

任务组件使用户能够查看、添加、删除、完成或编辑 Microsoft Planner 中的任务。  

此外，用户能够将一个或多个 Microsoft Graph 用户分配给任务。 有关 Microsoft Graph 分配的详细信息，请参阅[plannerAssignments。](/graph/api/resources/plannerassignments)

## <a name="example"></a>示例

以下示例使用组件显示登录用户的 Microsoft Planner `mgt-tasks` 任务。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a>属性

| 属性 | 属性 | 说明 |
| -- | -- | -- |
| 只读 | readOnly | 一个布尔值，用于将任务界面设置为只读， (添加或删除任务) 。 默认值为“`false`”。 |
| hide-header | hideHeader | 显示或隐藏组件标头的布尔值。 默认值为“`false`”。 |
| hide-options | hideOptions | 用于显示或隐藏任务中的选项的布尔值。 默认值为“`false`”。
| initial-id="planner_id/folder_id" | initialId | 一个字符串 ID，用于将最初显示的规划器或文件夹设置为提供的 ID。 |
| initial-bucket-id="bucket_id" | initialBucketId | 一个字符串 ID，用于将最初显示的存储桶 (Planner Data-Source设置为) ID。 |
| target-id="planner_id/folder_id"| targetId | 一个字符串 ID，用于将任务接口锁定到所提供的计划工具或文件夹 ID。 |
| target-bucket-id="bucket_id" |targetBucketId  | 一个字符串 ID，用于将任务接口锁定到 Planner (仅Data-Source提供的) 。 |
| group-id | groupId  | 用于将任务接口锁定到组 ID 的字符串 ID。 |
| 不适用 | isNewTaskVisible  | 确定新任务视图在呈现时是否可见。 |
| 不适用 | taskFilter  | 可选函数，用于筛选向用户显示的任务。 |

以下示例仅显示来自 ID *为 12345* 的 Planner 中的任务，并且不允许用户创建新任务。

```html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
```

以下示例演示如何筛选仅设置了 *category3* 的任务。

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

## <a name="events"></a>活动
| 事件 | 详情 | 说明 |
| --- | --- | --- |
| taskAdded | 详细信息包含各自的 `task` 对象 | 在新建任务后触发。 |
| taskChanged | 详细信息包含各自的 `task` 对象 | 更改任务元数据（如标记已完成）时触发。 |
| taskClick | 详细信息包含各自的 `task` 对象 | 当用户单击或点击任务时触发。 |
| taskRemoved | 详细信息包含各自的 `task` 对象 | 删除现有任务后触发。 |

## <a name="templates"></a>模板

该 `tasks` 组件支持 [多个](../customize-components/templates.md) 模板，允许您替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件中的元素，将值设置为下列 `data-type` 值之一：

| 数据类型     | 数据上下文              | 说明                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | task： a planner task object | 替换整个默认任务。 |
| task-details | task： a planner task object | 模板替换任务的详细信息部分。 |

下面的示例定义任务组件的模板。

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

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用以下 Microsoft Graph API 和权限。

| 资源 | 权限 |
| - | - |
| /me/planner/plans | Group.Read.All |
| /planner/plans/${id} | Group.Read.All、Group.ReadWrite.All |
| /planner/tasks | Group.ReadWrite.All |
| /groups/${group-id}/planner/plans | Group.Read.All、Group.ReadWrite.All |

对于 Microsoft Planner 数据源，提取和读取任务需要 Groups.Read.All 权限。 添加、更新或删除任务需要 Groups.ReadWrite.All 权限。

## <a name="authentication"></a>身份验证

任务组件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。