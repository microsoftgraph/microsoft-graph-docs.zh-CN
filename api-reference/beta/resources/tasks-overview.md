---
title: 使用微软待办任务 API
description: 可以使用 Microsoft Graph API 创建一个与微软待办中的任务和任务列表连接的应用。
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 1275e9de566bad3797255d232d2edf5892ac4b6d
ms.sourcegitcommit: c99d3feb3ab5cae506c1f758bc277a637adc9111
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61432641"
---
# <a name="use-the-microsoft-to-do-api"></a>使用微软待办 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft Graph 待办事项任务 API 创建与其邮箱中用户的任务连接的应用。 使用任务构建各种体验，如下所示：

* 从应用的工作流（例如，从电子邮件或通知）创建任务，并将其保存到微软待办中。 使用 [linkedResource](linkedresource.md) 实体将链接存储回你的应用。
* 将应用的现有任务与微软待办进行同步，并创建单个任务视图，以便更好地确定优先顺序和实施管理。
* 在自定义业务应用程序中管理微软待办任务。
* 在任务上创建 [checklistItems](checklistitem.md) ，以在较小的步骤中分解复杂任务。

目前，API 仅支持由已登录用户委派的权限。

开始使用微软待办任务 API 之前，请查看资源以及它们之间的关系。

![突出显示任务待办事项任务 API 实体的屏幕截图。 屏幕截图显示了左侧的任务列表、中心内特定任务列表中的任务，以及右侧的清单项和链接资源以及其他任务属性。](/graph/images/tasks-api-entities.png)

## <a name="task-list"></a>任务列表

[TaskList](./basetasklist.md) 代表 [Task](./basetask.md) 资源的逻辑容器。 目前只能在任务列表中创建任务。 在默认任务列表中创建未指定列表的情况下创建的任务。 若要[获取所有任务列表](../api/basetasklist-get.md)，请执行以下 HTTP 请求：

``` http
GET /me/tasks/lists
```

## <a name="task"></a>任务

[Task](./basetask.md) 表示任务，即可跟踪和完成的一件工作或个人项目。 若要从任务列表中获取任务，请执行以下 HTTP 请求：
``` http
GET /me/tasks/lists/{taskListId}/tasks
```

## <a name="checklist-item"></a>清单项 

[ChecklistItem](linkedresource_v2.md)表示一个项，它有助于以更小的步骤分解复杂任务。 如果要从任务获取 checklistItems，请提出以下 HTTP 请求：
``` http
GET /me/tasks/lists/{taskListId}/tasks/{taskId}/checklistItems/{checklistItems}
```

## <a name="linked-resource"></a>链接的资源

[linkedResource](linkedresource_v2.md) 表示与任务相关的合作伙伴应用程序中的任何项目，例如从中创建任务的项目（如电子邮件）。 可以使用它来将信息和链接存储回你的应用中的相关项。 若要从任务获取链接的资源，请执行以下 HTTP 请求：
``` http
GET /me/tasks/lists/{taskListId}/tasks/{taskId}/linkedresources/{linkedResourceId}
```

## <a name="track-changes-using-delta-query"></a>使用 delta 查询跟踪更改

出于性能原因，可能需要维护对象的本地缓存，并使用 [delta 查询](/graph/delta-query-overview)定期将本地缓存与服务器同步。

以下微软待办 API 资源支持 delta 查询：
* 任务列表中的 [Task](./basetask.md) 集合
* [TaskList](./basetasklist.md)

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。
