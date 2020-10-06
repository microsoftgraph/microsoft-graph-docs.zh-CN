---
title: 创建频道
description: 在请求正文中指定的 Microsoft 团队中创建新通道。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3f9c5ace14274d4761b90bc56d9c4bfce03f2d3e
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364234"
---
# <a name="create-channel"></a>创建频道

命名空间：microsoft.graph

在团队中创建一个新的 [频道](../resources/channel.md) ，如请求正文中所指定。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | "创建"、"组"、"全部"、"全部"、"全部"    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 |"创建"、"组"、"全部"、"全部"、"全部迁移"、"全部迁移"。|

> **注意**：此 API 支持管理员权限。 全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.  |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-create-a-standard-channel"></a>示例1：创建标准通道
#### <a name="request"></a>请求

下面的示例展示了创建标准频道的请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="c"></a>[C#](#tab/csharp) 
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript) 
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]
---
#### <a name="response"></a>响应

以下示例显示了相应的响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a>示例2：代表用户创建专用通道

#### <a name="request"></a>请求

下面的示例演示了创建专用通道并将用户添加为团队所有者的请求。

<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{group_id}/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Graph.channel",
  "membershipType": "private",
  "displayName": "My First Private Channel",
  "description": "This is my first private channels",
  "members":
     [
        {
           "@odata.type":"#microsoft.graph.aadUserConversationMember",
           "user@odata.bind":"https://graph.microsoft.com/v1.0/users('{user_id}')",
           "roles":["owner"]
        }
     ]
}
```

#### <a name="response"></a>响应

以下示例显示了相应的响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('{group_id}')/channels/$entity",
    "id": "{channel_id}",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/{channel_id}/My%20First%20Private%20Channel?groupId={group_id}&tenantId={tenant_id}",
    "membershipType": "private"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
