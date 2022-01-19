---
title: team：sendActivityNotification
description: 在团队范围内发送活动源通知。
author: eddie-lee-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bf872f5609b7af3d0a47bdf4a88022d47438d948
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072353"
---
# <a name="team-sendactivitynotification"></a>team：sendActivityNotification
命名空间：microsoft.graph

在团队范围内发送活动源通知。 有关发送通知的更多详细信息以及发送通知的要求，请参阅[发送Teams活动通知](/graph/teams-send-activityfeednotifications)。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|TeamsActivity.Send|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|TeamsActivity.Send.Group*，TeamsActivity.Send|

>**注意：** 标记为 * 的权限使用 [特定于资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

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
|activityType|String|活动类型。 这必须在应用清单[Teams声明](/microsoftteams/platform/overview)。|
|chainId|Int64|可选。 用于替代上一个通知。 在后续 `chainId` 请求中使用相同的方法替代上一个通知。|
|previewText|[itemBody](../resources/itembody.md)|预览通知文本。 Microsoft Teams显示前 150 个字符。|
|templateParameters|[keyValuePair](../resources/keyvaluepair.md) 集合|活动源条目中定义的模板变量的值与应用程序Teams `activityType` [相对应](/microsoftteams/platform/overview)。|
|recipient|[teamworkNotificationRecipient](../resources/teamworknotificationrecipient.md)|通知的收件人。 仅Azure AD用户。 另请参阅 [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md)。 |

将 topic 属性的值设置为 时 `source` ，支持 **以下** 资源 `entityUrl` ：

- [团队](../resources/team.md)
- [频道](../resources/channel.md)
- [chatMesage](../resources/chatmessage.md)
- [teamsTab](../resources/teamstab.md)

> **注意：** 实体 URL 必须相同或 URL 中团队的子资源。 此外[，Teams](/microsoftteams/platform/overview)应用必须安装在团队中。

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a>示例 1：通知用户有关待处理的财务审批请求

此示例演示如何发送团队的活动源通知。 此示例通知团队所有者有关待处理的财务审批请求。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}"
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/team-sendactivitynotification-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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

### <a name="example-2-notify-a-user-about-a-channel-tab"></a>示例 2：通知用户有关频道选项卡的信息

与上一示例类似，此示例对 `entityUrl` 使用 `topic` 。 但是，此示例[链接到频道中的](../resources/teamstab.md)[选项卡](../resources/channel.md)。 选项卡承载一个页面，向用户显示其酒店预订的状态。 选择通知后，用户即可访问选项卡，可在其中查看预订。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
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

### <a name="example-3-notify-a-user-about-a-channel-tab-using-user-principal-name"></a>示例 3：使用用户主体名称通知用户有关频道选项卡的信息

与上一示例类似，此示例对 `entityUrl` 使用 `topic` 。 但是，此示例[链接到频道中的](../resources/teamstab.md)[选项卡](../resources/channel.md)。 选项卡承载一个页面，向用户显示其酒店预订的状态。 选择通知后，用户即可访问选项卡，可在其中查看预订。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_upn"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    },
    "activityType": "reservationUpdated",
    "previewText": {
        "content": "You have moved up the queue"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "jacob@contoso.com"
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-upn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-upn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-upn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-upn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/team-sendactivitynotification-upn-go-snippets.md)]
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

### <a name="example-4-notify-a-user-about-an-event-using-custom-topic"></a>示例 4：使用自定义主题通知用户事件

如前面的示例中所示，你可以链接到团队的不同方面。 但是，如果要链接到不是团队的一部分或不是由 Microsoft Graph 表示的方面，或者希望自定义名称，可以将 的源设置为 并传递其自定义 `topic` `text` 值。 `webUrl` 将 source 设置为 时 `topic` 是必需的 `text` 。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
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