---
title: 使用微软待办 API
description: 可以使用 todoTask 上构建的 Microsoft Graph API 创建与 Microsoft To Do 中的任务连接的应用。
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: e20b6102eb94e05b62b701026fa6958b895739d3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820383"
---
# <a name="use-the-microsoft-to-do-api"></a>使用微软待办 API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用在 [todoTask](todotask.md) 上构建的 Microsoft Graph 待办事项 API 创建一个可跨 Microsoft To Do 客户端任务连接的应用。 使用任务构建各种体验，如下所示：

* 从应用的工作流（例如，从电子邮件或通知）创建任务，并将其保存到微软待办中。 使用 [linkedResource](linkedresource.md) 实体将链接存储回你的应用。
* 将应用的现有任务与微软待办进行同步，并创建单个任务视图，以便更好地确定优先顺序和实施管理。
* 在自定义业务应用程序中管理微软待办任务。

目前，API 仅支持由已登录用户委派的权限。

在开始使用微软待办 API 之前，请查看资源以及它们之间的关系。

![突出显示待办事项 API 实体的屏幕截图。屏幕截图显示了左侧的任务列表、中心内特定任务列表中的任务，以及右侧的清单项和链接资源以及其他任务属性。](/graph/images/tasks-api-entities.png)

## <a name="task-list"></a>任务列表

在此 API 集中，任务列表由 [todoTaskList](./todotasklist.md) 表示，它是 [todoTask](./todotask.md) 资源的逻辑容器。 目前只能在任务列表中创建任务。 若要[获取所有任务列表](../api/todotasklist-get.md)，请执行以下 HTTP 请求：

``` http
GET /me/todo/lists
```

## <a name="task"></a>任务

在此 API 集中，任务由 [todoTask](./todotask.md) 资源表示，该资源是可跟踪和完成的工作项或个人项目。 若要从任务列表中获取任务，请执行以下 HTTP 请求：
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
```

## <a name="checklist-item"></a>清单项 

[checklistItem](checklistitem.md) 表示较大的 [todoTask](./todotask.md) 中的子任务。 通过 **ChecklistItem**，可将复杂任务分解为更具可操作性、更小的任务。 若要从任务获取 **checklistItem**，请发出以下 HTTP 请求：
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItems}
```

## <a name="linked-resource"></a>链接的资源

[linkedResource](linkedresource.md) 表示与任务相关的合作伙伴应用程序中的任何项目，例如从中创建任务的项目（如电子邮件）。 可以使用它来将信息和链接存储回你的应用中的相关项。 若要从任务获取链接的资源，请执行以下 HTTP 请求：
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/linkedresources/{linkedResourceId}
```

## <a name="track-changes-using-delta-query"></a>使用 delta 查询跟踪更改

出于性能原因，可能需要维护对象的本地缓存，并使用 [delta 查询](/graph/delta-query-overview)定期将本地缓存与服务器同步。

以下微软待办 API 资源支持 delta 查询：
* 任务列表中的 [todoTask](./todotask.md) 集合
* [todoTaskList](./todotasklist.md)

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

