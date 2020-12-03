---
title: 团队： sendActivityNotification
description: 在团队范围内发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6db256a71c17e4c940669aaf96f61f70285c8f3e
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523385"
---
# <a name="team-sendactivitynotification"></a>团队： sendActivityNotification
命名空间：microsoft.graph

在团队范围内发送活动源通知。 有关发送通知和执行此操作的要求的详细信息，请参阅 [发送团队活动通知](/graph/teams-send-activityfeednotifications)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|TeamsActivity.Send|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|TeamsActivity.Send|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|topic|[teamworkActivityTopic](../resources/teamworkactivitytopic.md)|通知的主题。 指定要讨论的资源。|
|activityType|String|活动类型。 必须在 [团队应用程序清单](/microsoftteams/platform/overview)中声明。|
|chainId|Int64|可选。 用于替代以前的通知。 `chainId`在后续请求中使用相同的重写以前的通知。|
|previewText|[itemBody](../resources/itembody.md)|预览通知文本。 Microsoft 团队将仅显示前150个字符。|
|templateParameters|[keyValuePair](../resources/keyvaluepair.md) 集合|在与 `activityType` [团队应用程序清单](/microsoftteams/platform/overview)对应的活动源条目中定义的模板变量的值。|
|recipient|[teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md)|通知的收件人。 仅支持 Azure AD 用户。 另请参阅 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md)。 |

将主题属性的值设置为以下资源时，支持以下资源 `source` **topic** `entityUrl` ：

- [team](../resources/team.md)
- [频道](../resources/channel.md)
- [chatMesage](../resources/chatmessage.md)
- [teamsTab](../resources/teamstab.md)

> **注意：** 实体 url 必须是 url 中的团队的相同或子资源。 此外，团队 [应用程序](/microsoftteams/platform/overview) 必须安装在团队中。

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a>示例1：通知用户有关待定的财务审批请求

本示例演示如何向团队发送活动源通知。 本示例将关于待处理的财务审批请求通知工作组所有者。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a>示例2：通知用户有关频道选项卡的信息

与上一个示例类似，此示例使用 `entityUrl` `topic` 。 但是，此示例链接到[频道](../resources/channel.md)中的一个[选项卡](../resources/teamstab.md)。 该选项卡承载一个页面，向用户显示其酒店预订的状态。 选择通知将使用户进入该选项卡，在其中可以检查其保留。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    },
    "activityType": "reservationUpdated",
    "previewText": {
        "content": "You have moved up the queue"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "reservationId",
            "value": "TREEE433"
        },
        {
            "name": "currentSlot",
            "value": "23"
        }
    ]
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a>示例3：使用自定义主题通知用户有关事件

如前面的示例中所示，您可以链接到团队的不同方面。 但是，如果要链接到不属于团队的方位或者不是由 Microsoft Graph 表示的方位，或者您想要自定义该名称，则可以设置 to 的来源 `topic` `text` 并为其传入自定义值。 `webUrl` 将 "源" 设置为时是必需的 `topic` `text` 。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "deploymentApprovalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
