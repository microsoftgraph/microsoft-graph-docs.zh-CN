---
title: 删除 conversationMember
description: 从频道中删除 conversationMember。
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fb06950403e6f49421fdc600fd5b3d47023b00f12145bf77fab78b08b3ae3691
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54172608"
---
# <a name="delete-conversationmember"></a>删除 conversationMember

命名空间：microsoft.graph

从频道[中删除 conversationMember。](../resources/conversationmember.md) [](../resources/channel.md)


## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|---------|-------------|
|委派（工作或学校帐户）| ChannelMember.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| ChannelMember.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a>请求标头

| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[C#](#tab/csharp)

# <a name="javascript"></a>[JavaScript](#tab/javascript)

# <a name="objective-c"></a>[Objective-C](#tab/objc)

---

### <a name="response"></a>响应

下面是一个响应示例。

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
