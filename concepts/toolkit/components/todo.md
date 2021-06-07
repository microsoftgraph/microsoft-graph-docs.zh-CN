---
title: 微软待办 Microsoft Graph Toolkit
description: 利用微软待办组件，用户可以查看、添加、删除、完成或编辑任务。 它适用于 Microsoft 微软待办 中微软待办。
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 3eb91bc23f1159e08749b6e6b073939bacca0c5c
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781000"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a>微软待办 Microsoft Graph Toolkit

微软待办 组件用于允许登录用户在 Microsoft Graph 中通过 微软待办 API 查看、添加、删除、完成和/或编辑 微软待办 中的任务。

## <a name="example"></a>示例

以下示例显示登录用户使用组件微软待办任务 `mgt-todo` 。 可以使用代码编辑器查看 [属性如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[在"打开"mgt.dev](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a>属性

可以使用下列属性和属性自定义组件。

| 属性 | 属性 | 说明 |
| -- | -- | -- |
| 只读 | readOnly | 一个布尔值，用于将任务界面设置为只读， (添加或删除任务) 。 默认值为“`false`”。 |
| hide-header | hideHeader | 显示或隐藏组件标头的布尔值。 默认值为“`false`”。 |
| hide-options | hideOptions | 用于显示或隐藏任务中的选项的布尔值。 默认值为“`false`”。
| initial-id="folder_id" | initialId | 一个字符串 ID，用于将最初显示的文件夹设置为提供的 ID。 |
| target-id="folder_id"| targetId | 一个字符串 ID，用于将任务接口锁定为所提供的文件夹 ID。 |
| 不适用 | isNewTaskVisible  | 确定新任务视图在呈现时是否可见。 |
| 不适用 | taskFilter  | 可选函数，用于筛选向用户显示的任务。 |

以下示例只显示 ID 为 *12345* 的文件夹中的任务，并且不允许用户创建新任务。

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a>自定义 CSS 变量

组件 `mgt-todo` 定义以下 CSS 自定义属性。

````css
mgt-todo {
  --tasks-background-color
  --tasks-header-padding
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

  --task-margin
  --task-background
  --task-border
  --task-header-color
  --task-header-margin

  --task-new-margin
  --task-new-border
  --task-new-input-margin
  --task-new-input-padding
  --task-new-input-font-size
  --task-new-select-border

  --task-new-add-button-background
  --task-new-add-button-disabled-background
  --task-new-cancel-button-color

  --task-complete-background
  --task-complete-border

  --task-icon-alignment: flex-start (default) | center | flex-end
  --task-icon-background
  --task-icon-background-completed
  --task-icon-border
  --task-icon-border-completed
  --task-icon-border-radius
  --task-icon-color
  --task-icon-color-completed
}
````

若要了解更多信息，请参阅 [设置组件样式](https://docs.microsoft.com/graph/toolkit/style.md)。

## <a name="events"></a>活动

从组件中触发以下事件。

| 事件 | 详情 | 说明 |
| --- | --- | --- |
| taskAdded | 详细信息包含各自的 `task` 对象 | 新建任务后触发。 |
| taskChanged | 详细信息包含各自的 `task` 对象 | 更改任务元数据（如标记已完成）时触发。 |
| taskClick | 详细信息包含各自的 `task` 对象 | 当用户单击或点击任务时触发。 |
| taskRemoved | 详细信息包含各自的 `task` 对象 | 删除现有任务后触发。 |

## <a name="templates"></a>模板

组件 `tasks` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含组件 `<template>` 中的元素，将值 `data-type` 设置为以下值之一。

| 数据类型     | 数据上下文              | 说明                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| task     | task： a to-do task object | 替换整个默认任务。 |
| task-details | task： a to-do task object | 模板将替换任务的详细信息部分。 |

下面的示例定义任务组件的模板。

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a>Microsoft Graph 权限

此控件使用下列 Microsoft Graph API 和权限。

| 配置 | 权限 | API |
| ------------- | ---------- | --- |
| `targetId` set | Tasks.Read | [/me/todo/lists/${listId}](/graph/api/todotasklist-get?view=graph-rest-1.0&tabs=http)、 [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) |
| `targetId` 未设置 | Tasks.Read | [/me/todo/lists](/graph/api/todo-list-lists?view=graph-rest-1.0&tabs=http) [、/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) |
| 创建、更新或删除任务 | Tasks.ReadWrite | [/me/todo/lists/{todoTaskListId}/tasks/{taskId}](/graph/api/todotask-get) |

## <a name="authentication"></a>身份验证

任务组件使用身份验证文档 中所述的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="cache"></a>缓存

`mgt-todo`组件不缓存任何数据。
