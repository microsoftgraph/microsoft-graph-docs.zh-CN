---
title: 获取频道
description: 检索频道的属性和关系。
author: nkramer
doc_type: apiPageType
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: 4426a28cde06f7718bc35f05e6c093f06f8b3e8a
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60925760"
---
# <a name="get-channel"></a>获取频道

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索[频道](../resources/channel.md)的属性和关系。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Channel.ReadBasic.All、ChannelSettings.Read.All、ChannelSettings.ReadWrite.All、Group.Read.All **、Group.ReadWrite.All**、Directory.Read.All **、Directory.ReadWrite.All** |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | ChannelSettings.Read.Group *、ChannelSettings.ReadWrite.Group*、Channel.ReadBasic.All、ChannelSettings.Read.All、ChannelSettings.ReadWrite.All、Group.Read.All **、Group.ReadWrite.All**、Directory.Read.All **、Directory.ReadWrite.All** |

> **注意**：标有 * 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。 标记为 **的权限已弃用，不应使用。

> **注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [channel](../resources/channel.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面是一个响应示例。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2",
    "createdDateTime": "2020-05-27T19:22:25.692Z",
    "displayName": "General",
    "description": "AutoTestTeam_20210311_150740.2550_fim3udfdjen9",
    "membershipType": "standard"
}

```

下面是关闭频道审核的标准频道的响应示例。

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('8bb12236-b929-42e0-94a0-1c417466ebf8')/channels/$entity",
    "id": "19:d468258bc90f4a358361b5d73b89d39b@thread.skype",
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3Ad468258bc90f4a358361b5d73b89d39b%40thread.skype/General?groupId=8bb12236-b929-42e0-94a0-1c417466ebf8&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
    "membershipType": "standard",
    "moderationSettings": {
        "userNewMessageRestriction": "everyone",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```

下面是频道审核打开的标准频道的响应示例。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('8bb12236-b929-42e0-94a0-1c417466ebf8')/channels/$entity",
    "id": "19:d468258bc90f4a358361b5d73b89d39b@thread.skype",
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3Ad468258bc90f4a358361b5d73b89d39b%40thread.skype/General?groupId=8bb12236-b929-42e0-94a0-1c417466ebf8&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
    "membershipType": "standard",
    "moderationSettings": {
        "userNewMessageRestriction": "moderators",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```

下面是私人频道的响应示例。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('8bb12236-b929-42e0-94a0-1c417466ebf8')/channels/$entity",
    "id": "19:d468258bc90f4a358361b5d73b89d39b@thread.skype",
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19%3Ad468258bc90f4a358361b5d73b89d39b%40thread.skype/General?groupId=8bb12236-b929-42e0-94a0-1c417466ebf8&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924",
    "membershipType": "private",
    "moderationSettings": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


