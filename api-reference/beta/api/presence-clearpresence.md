---
title: presence： clearPresence
description: 清除用户的应用程序状态会话状态信息。
author: jsandoval-msft
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: af98bf701603acac022a0944c01937c2f0979641
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60997357"
---
# <a name="presence-clearpresence"></a>presence： clearPresence

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

清除用户的应用程序状态会话。 如果它是用户的唯一状态会话，则用户状态将更改为 `Offline/Offline` 。

有关状态会话的详细信息，请参阅 [状态：setPresence](presence-setpresence.md#presence-sessions)。

## <a name="permissions"></a>Permissions
调用 API 需要以下权限。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | 不支持。                              |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearPresence
```

## <a name="request-headers"></a>请求标头
| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数 | 类型   | 说明                                   |
| :-------- | :----- | :-------------------------------------------- |
| sessionId | string | 应用程序状态会话的 ID。 |


> [!IMPORTANT]
> 
> 提供请求中应用程序 `sessionId` ID。

## <a name="response"></a>响应
如果成功，此方法返回 `200 OK` 响应代码。

如果状态会话不存在，此方法将返回 响应 `404 NotFound` 代码。

## <a name="examples"></a>示例
以下请求显示 ID 为 `22553876-f5ab-4529-bffb-cfe50aa89f87` 用户清除其状态会话的应用程序 `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` 。

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clear--presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clear--presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clear--presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clear--presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clear--presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/clear--presence-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
