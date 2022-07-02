---
title: deletedTeam：getAllMessages
description: 检索已删除团队中跨所有频道的全部消息。
author: agnesliu
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ddb94c35b00a88041004d01567d572d157af84a9
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578121"
---
# <a name="deletedteam-getallmessages"></a>deletedTeam：getAllMessages
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [已删除团队](../resources/deletedteam.md) 中跨所有 [频道](../resources/channel.md) 的全部 [消息](../resources/chatmessage.md)，包括文本、音频和视频对话。

要详细了解如何使用 Microsoft Teams 导出 API 导出内容，请参阅 [使用 Microsoft Teams 导出 API 导出内容](/microsoftteams/export-teams-content)。

[!INCLUDE [teams-model-A-and-B-disclaimer](../../includes/teams-model-A-and-B-disclaimer.md)]

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|不支持。|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|ChannelMessage.Read.All|

> [!NOTE]
> 在使用应用程序权限调用此 API 之前，必须先请求访问权限。 有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="optional-query-parameters"></a>可选的查询参数

根据首选的 [许可和付款模型](/graph/teams-licenses)，可以使用支持值 `A` 和 `B` 的 `model` 查询参数，如以下示例所示。  

```http
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages?model=A
GET /teamwork/deletedTeams/{deletedTeamId}/channels/getAllMessages?model=B
```

如果未指定 `model` 参数，则将使用 [评估模式](/graph/teams-licenses#evaluation-mode-default-requirements)。

此方法支持 [$top](/graph/query-parameters#top-parameter) 查询参数以控制每个响应的项数，并通过 **lastModifiedDateTime** 上的 **dateTime** 范围查询支持 [$filter](/graph/query-parameters#filter-parameter) 查询参数。 当前不支持其他 [OData 查询参数](/graph/query-parameters)。

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数将在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。
<!-- {
  "blockType": "request",
  "name": "deletedteamthis_getallmessages"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/deletedTeams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages
```


### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teamwork/deletedTeams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1616990417393",
            "replyToId": null,
            "etag": "1616990417393",
            "messageType": "message",
            "createdDateTime": "2021-03-29T04:00:17.393Z",
            "lastModifiedDateTime": "2021-03-29T04:00:17.393Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3Ad5d2708d408c41d98424c1c354c19db3%40thread.tacv2/1616990417393?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990417393&parentMessageId=1616990417393",
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": "Robin Kline",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Test message"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:d5d2708d408c41d98424c1c354c19db3@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

