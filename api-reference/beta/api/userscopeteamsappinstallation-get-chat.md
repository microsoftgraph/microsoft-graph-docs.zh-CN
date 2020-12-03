---
title: 在用户和 teamsApp 之间获取聊天
description: 检索指定用户与团队应用程序之间的一对一聊天。
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0e9776b48fcfc64d3a3b1a1f9c5eb49f704adfc2
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564159"
---
# <a name="get-chat-between-user-and-teamsapp"></a>在用户和 teamsApp 之间获取聊天

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索指定[用户](../resources/user.md)和[团队应用程序](../resources/teamsapp.md)的[聊天](../resources/chat.md)。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}/chat
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [chat](../resources/chat.md) 对象的实例。

## <a name="examples"></a>示例

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a>示例1：在指定的用户与团队应用程序之间列出一对一聊天

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}/chat
```

#### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "name": "user_chat_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
   "id": "19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
 }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User chat teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
