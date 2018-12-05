---
title: 共享或委派的日历中获取 Outlook 事件
description: 在 Outlook 中，客户可以与其他用户共享日历并让他人查看或修改该日历中的事件。 客户还可以授予其代表，以接收或响应会议请求，或者创建或更改日历中的项目的代理人。
ms.openlocfilehash: e05352e164b127adca1305dded5cbb00840eed52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091821"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>共享或委派的日历中获取 Outlook 事件

在 Outlook 中，客户可以与其他用户共享日历并让他人查看或修改该日历中的事件。 客户还可以授予其代表，以接收或响应会议请求，或者创建或更改日历中的项目的代理人。

以编程方式，Microsoft Graph 支持获取已由其他用户共享的日历中的事件，以及获取共享日历本身。 支持也适用于已委派的日历。

例如，Garth 具有与 John 共享其默认日历和授予 John 读取访问权限。 如果 John 已登录到您的应用程序，并提供委派的权限 （Calendars.Read.Shared 或 Calendars.ReadWrite.Shared），您的应用程序都将能够访问 Garth 的默认日历和事件，如下所述的日历中。

## <a name="get-an-event-in-the-shared-calendar"></a>共享日历中获取事件

您可以获取 Garth 的共享的默认日历中的特定事件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

在操作成功完成，您将获取 HTTP 200 确定和[事件](/graph/api/resources/event?view=graph-rest-1.0)实例由标识`{id}`Garth 的默认日历。

## <a name="get-all-the-events-in-the-shared-calendar"></a>共享日历中获取所有事件

获取与 John 共享 Garth 默认日历中的所有事件：

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

在操作成功完成，您将获取 HTTP 200 确定和 Garth 的默认日历中的[事件](/graph/api/resources/event?view=graph-rest-1.0)实例的集合。

## <a name="get-the-shared-calendar"></a>获取共享的日历

获取与 John 共享 Garth 的默认日历。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

在操作成功完成，您将获取 HTTP 200 确定和代表 Garth 的默认文件夹的[日历](/graph/api/resources/calendar?view=graph-rest-1.0)实例。

如果 Garth 具有委派 John 进一步访问 Garth 的默认日历，或者 Garth 具有委派 John 其整个邮箱将应用相同的 GET 功能。

如果 Garth 不具有与 John、 共享其默认日历也有他代理其邮箱到 John，这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [为什么与 Outlook 日历集成](outlook-calendar-concept-overview.md)
- Microsoft Graph v1.0 中的[日历 API](/graph/api/resources/calendar?view=graph-rest-1.0) 。