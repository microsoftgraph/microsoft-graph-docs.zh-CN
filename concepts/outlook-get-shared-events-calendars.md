---
title: 获取共享或委托的 Outlook 日历及其事件
description: 在 Outlook 中，日历所有者可与其他用户共享日历，并让他们查看或修改该日历中的事件；日历可以是自定义日历或主日历。 所有者还可以授权代理人代表其执行操作，接收或答复会议请求，或在电子邮件帐户的主日历中创建或更改项目。
author: juforan
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 89752e74222dadeb424d5c2a8b865c8b5536b572
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135884"
---
# <a name="get-shared-or-delegated-outlook-calendar-and-its-events"></a>获取共享或委托的 Outlook 日历及其事件

在 Outlook 中，日历所有者可与其他用户共享日历，并让他们查看或修改该日历中的事件；共享日历可以是所有者的主日历或由所有者创建的自定义日历。 所有者还可以向其主日历授权代理人以代表其执行操作，接收或答复会议请求，或在主日历中创建或更改项目。

Microsoft Graph 支持以编程方式读取和写入其他用户已共享的日历中的事件、读取共享日历以及更新共享者的日历名称。 此支持还适用于已委托的日历。 本文的其余部分介绍如何在共享或委托的日历中读取事件。 有关创建事件的信息，请参阅[在共享日历或委托的日历中创建 Outlook 事件](outlook-create-event-in-shared-delegated-calendar.md)。

## <a name="sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox"></a>共享者：直接从日历所有者的邮箱获取共享日历或其事件

以下三个示例假设这样的情景：在 Outlook 中，Alex 向 Megan 共享了他的主日历，并给予 Megan 读取权限。 如果 Megan 登录你的应用，并提供 _委托权限_ (Calendars.Read.Shared or Calendars.ReadWrite.Shared)，代表 Megan，你的应用可以直接从 Alex 的邮箱中访问 Alex 的主日历及其事件。

三个示例指定了所有者的标识（Alex 的用户 ID 或用户主体名称）和 `calendar` 快捷方式。 这些示例仅访问与所有者的邮箱对应的日历和事件 ID。 在共享者的邮箱（Megan 的用户 ID 或用户主体名称）中指定这些日历和事件 ID 将返回错误。 若要使用与共享者的邮箱对应的日历和事件 ID，请参阅[共享者：从共享者的邮箱获取共享的自定义日历或其事件](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox)。 

> **注意**：通过共享权限（Calendars.Read.Shared 或 Calendars.ReadWrite.Shared），你可以在共享或委托的日历中读取或写入事件。 它们不支持[订阅此类文件夹中的项的更改通知](webhooks.md)。 若要对租户中共享、委托或任何其他用户或资源日历中的事件设置更改通知订阅，请使用应用程序权限 Calendars.Read。

### <a name="megan-get-the-shared-primary-calendar-directly-from-alex-mailbox"></a>Megan：直接从 Alex 的邮箱获取共享的主日历

以 Megan 的身份登录，直接从 Alex 的邮箱获取 Alex 向 Megan 共享的主日历：

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar
```

成功完成后，你将收到 HTTP 200 OK 消息和一个[日历](/graph/api/resources/calendar?view=graph-rest-1.0)实例，该实例表示 Alex 在Alex 的邮箱中共享的主日历。

### <a name="megan-get-an-event-in-the-shared-primary-calendar-directly-from-alex-mailbox"></a>Megan：直接从 Alex 的邮箱获取共享主日历中的事件

以 Megan 的身份登录，你的应用可以直接从 Alex 的邮箱获取 Alex 向 Megan 共享的主日历中的特定事件：

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events/{id}
```

成功完成后，你将收到 HTTP 200 OK 消息以及 Alex 的主日历中由 `{id}` 标识的[事件](/graph/api/resources/event?view=graph-rest-1.0)实例（直接从 Alex 的邮箱获取）。

### <a name="megan-get-all-the-events-in-the-shared-primary-calendar-from-alex-mailbox"></a>Megan：从 Alex 的邮箱获取共享主日历中的所有事件

以 Megan 的身份登录，直接从 Alex 的邮箱获取 Alex 向 Megan 共享的主日历中的所有事件：

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events
```

成功完成后，你将收到 HTTP 200 OK 消息以及 Alex 的主日历中的一组[事件](/graph/api/resources/event?view=graph-rest-1.0)实例（直接从 Alex 的邮箱获取）。

如果 Alex 已委托 Megan 访问 Alex 的主日历，或者 Alex 向 Megan 委托了其整个邮箱，则将适用同样的 GET 功能。

如果 Alex 尚未向 Megan 共享也未委托其主日历，则在前面的 GET 操作中指定 Alex 的用户 ID 或用户主体名称将返回错误。 


## <a name="sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox"></a>共享者：从共享者的邮箱获取共享的自定义日历或其事件

如果 Alex 向 Adele 共享了一个 _自定义_ 日历（例如，名为“Kids parties”的日历），并且 Adele 提供了委托权限（Calendars.Read 或 Calendars.ReadWrite），则你的应用可以从 Adele 邮箱中的 Alex 日历本地副本获取事件或日历，如下所述。

1. 以 Adele 的身份登录，使用以下任一请求获取 Adele 有权访问的所有日历，包括共享的自定义日历。

    <!-- {
      "blockType": "request",
      "name": "get_all_Adele_calendars"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars
    ```

    成功后的响应包括响应代码 HTTP 200 以及 Adele 有权访问的一组日历，包括所有者名称为“Alex Wilber”的日历（“Kids parties”），作为响应中的第二个日历。 对于共享者“Adele”，共享日历的 **canShare** 属性始终为 false。

    <!-- {
      "blockType": "response",
      "name": "get_all_Adele_calendars",
      "truncated": true,
      "@odata.type": "microsoft.graph.calendar",
      "isCollection": true
    } -->
    ```http
    HTTP/1.1 200 OK
    Content-type: application/json

    {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars",
        "value": [
            {
                "id": "AQMkADU5NAAAJMjAAAAA==",
                "name": "Calendar",
                "color": "auto",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAAAACXQ==",
                "canShare": true,
                "canViewPrivateItems": true,
                "canEdit": true,
                "owner": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            {
                "id": "AAMkADAABf0JlyAAA=",
                "name": "Kids parties",
                "color": "lightYellow",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAYumJRQ==",
                "canShare": false,
                "canViewPrivateItems": false,
                "canEdit": false,
                "owner": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            }
        ]
    }
    ```

2. 以 Adele 的身份登录，获取共享日历或获取共享日历中的一个或多个事件（使用步骤 1 的响应中的第二个日历 ID）。 共享日历的 ID 及其事件对应于 Adele 邮箱中的 Alex 日历本地副本。

    <!-- { "blockType": "ignored" } -->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events/{id}
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events/{id}

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events
    ```

成功完成后，你将收到 HTTP 200 OK 消息以及所请求的一个或多个事件或 Alex 向 Adele 共享的日历。


## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- [在共享或委托的日历中创建 Outlook 事件](outlook-create-event-in-shared-delegated-calendar.md)
- [在 Outlook 中共享或委托日历（预览版）](outlook-share-or-delegate-calendar.md)
- [为什么要与 Outlook 日历集成](outlook-calendar-concept-overview.md)
- Microsoft Graph v1.0 中的[日历 API](/graph/api/resources/calendar?view=graph-rest-1.0)。
