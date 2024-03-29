---
title: 微软待办 Microsoft Graph Toolkit 中的组件
description: 利用微软待办组件，用户可以查看、添加、删除、完成或编辑 todo 任务。 它适用于 Microsoft 微软待办 中微软待办。
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 6a77d75609cbff22fbaccefe45cd1f8b9e5355ca
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589245"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a>微软待办 Microsoft Graph Toolkit 中的组件

微软待办 组件用于使登录用户可以使用 Microsoft Graph 中的 微软待办 API 查看、添加、删除、完成和/或编辑 微软待办 中的任务。

## <a name="example"></a>示例

以下示例显示登录用户使用组件微软待办任务`mgt-todo`。 可以使用代码编辑器查看属性 [如何](#properties) 更改组件的行为。

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[在 mgt.dev 中打开此示例](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a>属性

可以使用下列属性和属性自定义组件。

| 属性 | 属性 | 说明 |
| -- | -- | -- |
| 只读 | readOnly | 一个布尔值，用于将任务界面设置为只读， (添加或删除任务) 。 默认值为“`false`”。 |
| hide-header | hideHeader | 显示或隐藏组件标头的布尔值。 默认值为“`false`”。 |
| hide-options | hideOptions | 用于显示或隐藏任务中的选项的布尔值。 默认值为“`false`”。
| initial-id="folder_id" | initialId | 一个字符串 ID，用于将最初显示的文件夹设置为提供的 ID。 |
| target-id="folder_id"| targetId | 用于将任务接口锁定为所提供的文件夹 ID 的字符串 ID。 |
| 不适用 | isNewTaskVisible  | 确定新任务视图在呈现时是否可见。 |
| 不适用 | taskFilter  | 可选函数，用于筛选向用户显示的任务。 |

以下示例仅显示 ID 为 *12345* 的文件夹中的任务，并且不允许用户创建新任务。

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

若要了解更多信息，请参阅 [设置组件样式](/graph/toolkit/style.md)。

## <a name="events"></a>事件

从组件中触发以下事件。

事件 | 何时发出 | 自定义数据 | Cancelable | 气泡 | 使用自定义模板
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`taskClick` | 当用户单击或点击任务时触发 | 选定的 [任务](https://github.com/microsoftgraph/microsoft-graph-toolkit/blob/66a5bbb6591e6260e95dbc00c0d06bcbe8dcef38/packages/mgt-components/src/components/mgt-todo/graph.todo.ts#L41) | 否 | 否 | 否

有关处理事件的信息，请参阅 [事件](../customize-components/events.md)。

## <a name="templates"></a>模板

组件 `tasks` 支持 [多个模板](../customize-components/templates.md) ，允许您替换组件的某些部分。 若要指定模板，请包含 `<template>` 组件中的元素，将 `data-type` 值设置为以下值之一。

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
| `targetId` set | Tasks.Read | [/me/todo/lists/${listId}](/graph/api/todotasklist-get?tabs=http)、 [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) |
| `targetId` 未设置 | Tasks.Read | [/me/todo/lists](/graph/api/todo-list-lists?tabs=http)、 [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) |
| 创建、更新或删除任务 | Tasks.ReadWrite | [/me/todo/lists/{todoTaskListId}/tasks/{taskId}](/graph/api/todotask-get) |

## <a name="authentication"></a>身份验证

任务组件使用身份验证文档中介绍的全局 [身份验证提供程序](../providers/providers.md)。

## <a name="cache"></a>缓存

组件 `mgt-todo` 不缓存任何数据。