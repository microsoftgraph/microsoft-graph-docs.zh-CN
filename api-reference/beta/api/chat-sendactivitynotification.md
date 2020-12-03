---
title: 聊天： sendActivityNotification
description: 在聊天范围内发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 76598572ebca1421770de5a298f46fdedc30a0c9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521997"
---
# <a name="chat-sendactivitynotification"></a>聊天： sendActivityNotification
命名空间：microsoft.graph

在聊天范围内发送活动源通知。 有关发送通知和执行此操作的要求的详细信息，请参阅 [发送团队活动通知](/graph/teams-send-activityfeednotifications)。

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
POST /chats/{chatId}/sendActivityNotification
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

将主题属性的值设置为以下资源时，支持以下资源 `source` **topic** `entityURL` ：

- [聊天](../resources/chat.md)
- [chatMessage](../resources/chatmessage.md)

> **注意：** 实体 URL 必须与 URL 中的聊天或子资源相同。 此外，还必须在聊天中安装 [团队应用程序](/microsoftteams/platform/overview) 。

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>示例1：通知用户在聊天中创建的任务

本示例演示如何为在聊天中创建的新任务发送活动源通知。 有关更多详细信息，请参阅 [发送团队活动通知](/graph/teams-send-activityfeednotifications)。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-java-snippets.md)]
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

### <a name="example-2-notify-a-user-about-a-approval-needed-in-a-chat-message"></a>示例2：在聊天消息中通知用户所需的审批

与上一个示例类似，此示例使用 `entityUrl` `topic` 。 但是，在这种情况下，它链接到聊天中的邮件。 邮件可以包含卡片上有审批按钮的卡片。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "Deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "approvalTaskId",
            "value": "2020AAGGTAPP"
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

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a>示例3：通知用户与聊天相关的事件

如前面的示例中所示，您可以链接到聊天的不同方面。 但是，如果您想要链接到不属于聊天的方位，或者不是由 Microsoft Graph 表示的，则可以将的来源设置 `topic` 为， `text` 并为其传入自定义值。 此外，将 " `webUrl` 源" 设置为时也是必需的 `topic` `text` 。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
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
