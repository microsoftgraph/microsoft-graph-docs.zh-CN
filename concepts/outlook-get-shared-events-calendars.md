---
title: 获取共享日历或委托日历中的 Outlook 事件
description: 在 Outlook 中，客户可以与其他用户共享日历，并允许其他用户查看或修改此日历中的事件。 客户还可以授权代理代表自己执行操作、接收或答复会议请求，或在日历中创建或更改项。
author: angelgolfer-ms
ms.openlocfilehash: ef4de6cedeeb9a5688f250652eef0cd6cd5f5183
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2018
ms.locfileid: "27413146"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>获取共享日历或委托日历中的 Outlook 事件

在 Outlook 中，客户可以与其他用户共享日历，并允许其他用户查看或修改此日历中的事件。 客户还可以授权代理代表自己执行操作、接收或答复会议请求，或在日历中创建或更改项。

Microsoft Graph 支持以编程方式获取其他用户已共享日历中的事件，以及共享日历本身。 此支持还适用于已委托的日历。

例如，Garth 已与 John 共享自己的默认日历，并向 John 授予读取访问权限。 如果 John 已登录应用并授予委托的权限（Calendars.Read.Shared 或 Calendars.ReadWrite.Shared），应用便能访问 Garth 的默认日历及其中的事件，如下所述。

> **注意**通过共享权限（Calendars.Read.Shared 或 Calendars.ReadWrite.Shared），你可以在共享或委托日历中读取或写入事件。 它们不支持[订阅此类文件夹中的项的更改通知](webhooks.md)。 若要对租户中共享、委托或任何其他用户或资源日历中的事件设置更改通知订阅，请使用应用程序权限 Calendars.Read。

## <a name="get-an-event-in-the-shared-calendar"></a>获取共享日历中的事件

可以获取 Garth 共享的默认日历中的特定事件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

成功完成后，便会收到“HTTP 200 正常”消息，以及 Garth 默认日历中由 `{id}` 标识的 [event](/graph/api/resources/event?view=graph-rest-1.0) 实例。

## <a name="get-all-the-events-in-the-shared-calendar"></a>获取共享日历中的所有事件

获取 Garth 已与 John 共享的默认日历中的所有事件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

成功完成后，便会收到“HTTP 200 正常”消息，以及 Garth 默认日历中的 [event](/graph/api/resources/event?view=graph-rest-1.0) 实例集合。

## <a name="get-the-shared-calendar"></a>获取共享日历

获取 Garth 已与 John 共享的默认日历。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

成功完成后，便会收到“HTTP 200 正常”消息，以及表示 Garth 默认文件夹的 [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) 实例。

如果 Garth 已委托 John 进一步访问自己的默认日历，或如果 Garth 已将自己的整个邮箱委托给 John，那么相同的 GET 功能适用。

如果 Garth 既未与 John 共享自己的默认日历，也未将自己的邮箱委托给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称便会返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解：

- [为什么要与 Outlook 日历集成](outlook-calendar-concept-overview.md)
- Microsoft Graph v1.0 中的[日历 API](/graph/api/resources/calendar?view=graph-rest-1.0)。