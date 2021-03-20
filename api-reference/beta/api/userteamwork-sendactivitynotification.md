---
title: userTeamwork： sendActivityNotification
description: 向用户发送活动源通知。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 73acd02d0189a4eb1c26f533e13b31b101a1fa7e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941935"
---
# <a name="userteamwork-sendactivitynotification"></a>userTeamwork： sendActivityNotification
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

向用户发送活动源通知。 有关发送通知的更多详细信息以及发送通知的要求，请参阅 [发送 Teams 活动通知](/graph/teams-send-activityfeednotifications)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
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
POST /users/{userId}/teamwork/sendActivityNotification
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
|activityType|String|活动类型。 这必须在 Teams 应用清单 [中声明](/microsoftteams/platform/overview)。|
|chainId|Int64|可选。 用于替代上一个通知。 在后续 `chainId` 请求中使用相同的方法替代上一个通知。|
|previewText|[itemBody](../resources/itembody.md)|预览通知文本。 Microsoft Teams 将只显示前 150 个字符。|
|templateParameters|[keyValuePair](../resources/keyvaluepair.md) 集合|在 Teams 应用清单 中对应的活动源条目中定义的 `activityType` 模板 [变量的值](/microsoftteams/platform/overview)。|

将 topic 属性的值设置为 时 `source` ，支持 **以下** 资源 `entityUrl` ：

- [teamsAppInstallation](../resources/teamsappinstallation.md)
- [teamsCatalogApp](../resources/teamscatalogapp.md)

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a>示例 1：向用户发送已创建任务的通知

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userteamwork_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
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
[!INCLUDE [sample-code](../includes/snippets/csharp/userteamwork-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userteamwork-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userteamwork-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userteamwork-sendactivitynotification-java-snippets.md)]
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

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a>示例 2：使用自定义主题通知用户事件

如果要链接未由 Microsoft Graph 表示的方面，或者希望自定义名称，可以将 的源设置为 并传递其 `topic` `text` 自定义值。 `webUrl` 将 source 用作 时 `topic` 是必需的 `text` 。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_4"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
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
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-4-java-snippets.md)]
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
