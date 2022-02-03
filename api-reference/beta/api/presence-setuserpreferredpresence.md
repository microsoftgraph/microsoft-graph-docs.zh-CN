---
title: presence： setUserPreferredPresence
description: 为用户设置用户首选状态
author: mkhribech
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 37fd49ea1f45ae8c1bb06e609d6fbc91d465a521
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344936"
---
# <a name="presence-setuserpreferredpresence"></a>presence： setUserPreferredPresence

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

设置用户的首选可用性和活动状态。 如果设置了用户的首选状态，则用户状态为首选状态。

首选状态仅在用户至少有一个状态 [会话时](presence-setpresence.md#presence-sessions) 生效。 否则，用户状态将保持脱机状态。

状态会话可以是 [setPresence](presence-setpresence.md) 操作成功的结果，或者如果用户登录到 Teams 客户端。 

阅读有关[状态会话](presence-setpresence.md#presence-sessions)及其[退出和过期时间等内容。](presence-setpresence.md#timeout-expiration-and-keep-alive) 

## <a name="permissions"></a>权限
调用 API 需要以下权限。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | Presence.ReadWrite                          |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | Presence.ReadWrite.All                      |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/setUserPreferredPresence
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数          | 类型     | 说明                                                                                                                                                                                                                                    |
| :----------------- | :------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| availability       | string   | 基本状态信息。                                                                                                                                                                                                                 |
| 活动           | string   | 可用性的补充信息。                                                                                                                                                                                                  |
| expirationDuration | duration | 应用状态会话的过期时间。 该值以 ISO 8601 格式表示，持续时间为。<br/>如果未提供，将应用默认过期：<br/>DoNotDisturb 或 Busy：在 1 天到期<br/>所有其他：在 7 天后过期 |

支持的可用性 **和活动****组合** 包括：

| availability | 活动     | 说明                                         |
| :----------- | :----------- | :-------------------------------------------------- |
| 可用    | 可用    | 将用户首选状态设置为"可用"。       |
| 忙碌         | 忙碌         | 将用户首选状态设置为忙碌。            |
| DoNotDisturb | DoNotDisturb | 将用户首选状态设置为 DoNotDisturb。    |
| BeRightBack  | BeRightBack  | 将用户首选状态设置为 BeRightBack。     |
| 离开         | 离开         | 将用户首选状态设置为离开。            |
| Offline      | OffWork      | 将用户首选状态设置为"脱机"。 |

## <a name="response"></a>响应
如果成功，此方法返回 `200 OK` 响应代码。

## <a name="examples"></a>示例

以下请求将用户首选状态设置为用户的 `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`DoNotDisturb，过期时间为 8 小时。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "setUserPreferredPresence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setUserPreferredPresence
Content-Type: application/json

{
  "availability": "DoNotDisturb",
  "activity": "DoNotDisturb",
  "expirationDuration": "PT8H"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/setuserpreferredpresence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/setuserpreferredpresence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/setuserpreferredpresence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/setuserpreferredpresence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/setuserpreferredpresence-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/setuserpreferredpresence-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
