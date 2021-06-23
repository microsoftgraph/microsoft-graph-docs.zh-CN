---
title: Microsoft 服务中的任务Graph Toolkit
description: 任务组件使用户能够查看、添加、删除、完成或编辑任务。 它适用于 Microsoft Planner 中的任何任务。
localization_priority: Normal
author: benotter
ms.openlocfilehash: 3b3476751798dd5569218ec6acc6d09a91112fe6
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082032"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Microsoft 服务中的任务Graph Toolkit

任务组件使用户能够查看、添加、删除、完成或编辑 Microsoft Planner 中的任务。  

此外，用户能够将单个或多个 Microsoft Graph分配给任务。 有关 Microsoft 工作分配Graph的详细信息，请参阅[plannerAssignments](/graph/api/resources/plannerassignments)。

## <a name="example"></a>示例

以下示例使用 组件显示已登录用户的 Microsoft Planner `mgt-tasks` 任务。 可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-tasks--tasks&source=docs" height="500"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-tasks--tasks&source=docs)

## <a name="properties"></a>属性

| 属性 | 属性 | 说明 |
| -- | -- | -- |
| 只读 | readOnly | 一个布尔值，用于将任务界面设置为只读， (添加或删除任务) 。 默认值为“`false`”。 |
| hide-header | hideHeader | 显示或隐藏组件标头的布尔值。 默认值为“`false`”。 |
| hide-options | hideOptions | 用于显示或隐藏任务中的选项的布尔值。 默认值为“`false`”。
| initial-id="planner_id/folder_id" | initialId | 一个字符串 ID，用于将最初显示的规划器或文件夹设置为提供的 ID。 |
| initial-bucket-id="bucket_id" | initialBucketId | 一个字符串 ID，用于将最初显示的存储桶 (Planner Data-Source仅) 设置为提供的 ID。 |
| target-id="planner_id/folder_id"| targetId | 一个字符串 ID，用于将任务接口锁定为提供的规划器或文件夹 ID。 |
| target-bucket-id="bucket_id" |targetBucketId  | 一个字符串 ID，用于将任务接口锁定为 Planner (提供的Data-Source ID) 。 |
| group-id | groupId  | 用于将任务接口锁定为组 ID 的字符串 ID。 |
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
| `taskAdded` | 详细信息包含各自的 `task` 对象 | 新建任务后触发。 |
| `taskChanged` | 详细信息包含各自的 `task` 对象 | 更改任务元数据（如标记已完成）时触发。 |
| `taskClick` | 详细信息包含各自的 `task` 对象 | 当用户单击或点击任务时触发。 |
| `taskRemoved` | 详细信息包含各自的 `task` 对象 | 删除现有任务后触发。 |

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

## <a name="templates"></a>模板

组件 `tasks` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为下列值之一：

| 数据类型     | 数据上下文              | 说明                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | 任务：计划工具任务对象 | 替换整个默认任务。 |
| task-details | 任务：计划工具任务对象 | template 将替换任务的详细信息部分。 |

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

此控件使用下列 Microsoft Graph API 和权限。

| 配置 | 权限 | API |
| ------------- | ---------- | --- |
| `groupId` set and `dataSource` set to `TasksSource.planner` | Group.Read.All | [/groups/${group-id}/planner/plans](/graph/api/plannergroup-list-plans?view=graph-rest-1.0&tabs=http)、 [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http)、 [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http) |
| `targetId` set and `dataSource` set to `TasksSource.todo` | Tasks.Read | [/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0) [、/me/outlook/taskGroups/${groupId}/taskFolders、/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http) [](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http) |
| `targetId` set and `dataSource` set to something else than `TasksSource.todo` | Group.Read.All | [/planner/plans/${planId}](/graph/api/plannerplan-get?view=graph-rest-1.0&tabs=http)、 [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http)、 [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http) |
| `dataSource` 设置为 `TasksSource.planner` | Group.Read.All | [/me/planner/plans](/graph/api/planneruser-list-plans?view=graph-rest-1.0&tabs=http)、 [/planner/plans/${planId}/buckets](/graph/api/plannerplan-list-buckets?view=graph-rest-1.0&tabs=http)、 [/planner/buckets/${bucketId}/tasks](/graph/api/plannerplan-list-tasks?view=graph-rest-1.0&tabs=http) |
| `dataSource` 设置为 `TasksSource.todo` | Tasks.Read | [/me/outlook/taskGroups](/graph/api/outlookuser-list-taskgroups?view=graph-rest-beta&tabs=http&viewFallbackFrom=graph-rest-1.0) [、/me/outlook/taskGroups/${groupId}/taskFolders、/me/outlook/taskFolders/${folderId}/tasks](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http) [](/graph/api/outlooktaskfolder-list-tasks?view=graph-rest-beta&tabs=http) |
| `addTask` 设置为 `true` ， `dataSource` 设置为 `TasksSource.planner` | Group.ReadWrite.All | [/planner/tasks](/graph/api/planner-post-tasks?view=graph-rest-1.0&tabs=http) |
| `addTask` 设置为 `true` ， `dataSource` 设置为 `TasksSource.todo` | Tasks.ReadWrite | [/me/outlook/taskFolders/${parentFolderId}/tasks](/graph/api/outlookuser-post-tasks?view=graph-rest-beta&tabs=csharp) |

对于 Microsoft Planner 数据源，提取和读取任务需要 Groups.Read.All 权限。 添加、更新或删除任务需要 Groups.ReadWrite.All 权限。

## <a name="authentication"></a>身份验证

任务组件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="cache"></a>缓存

`mgt-tasks`组件不缓存任何数据。
