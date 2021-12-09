---
title: presence： setPresence
description: 设置用户的应用程序状态会话状态信息。
author: mkhribech
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: f3a62e802d8ade524669aa68a0d6fb13ea717cc7
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391072"
---
# <a name="presence-setpresence"></a>presence： setPresence

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为用户设置应用程序状态会话中的可用性和活动状态。

### <a name="presence-sessions"></a>状态会话
用户可以具有多个状态会话，因为用户可以在桌面、移动和 web Teams多个 (客户端) 。 每个Teams客户端都有一个独立的状态会话，并且用户的状态是来自所有隐藏会话的聚合状态。

同样，应用程序可以具有其自己的用户状态会话，并能够更新状态。

以下是会话状态聚合方式的优先级，"A > B"表示 A 优先于 B：
* 用户首选状态>会话级别状态 (用户首选状态覆盖会话级别状态) 
* 在会话级别状态中：当前不支持 **setPresence** (Busy) > Available > DoNotDisturb >离开

### <a name="timeout-expiration-and-keep-alive"></a>超时、到期并保持活动状态
状态会话 **可能会超时并** 过期，因此应用程序需要在超时之前调用此 API，以维护会话的状态;或过期 **之前，** 使会话保持活动状态。

如果状态会话可用且超时为 5 分钟， `Available` 则状态会话可能会超时。 当状态淡出时，状态将逐渐淡出。 例如，如果应用程序将状态会话设置为 ，状态将在 5 分钟内更改为第一个超时，然后在另外 5 分钟（第二个超时） `Available/Available` `Available/AvailableInactive` `Away/Away` 中更改。

状态会话的过期时间可用 参数 `expirationDuration` 进行配置。 当会话过期时，它将变为 `Offline` 。

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
POST /users/{userId}/presence/setPresence
```
## <a name="request-headers"></a>请求标头
| 名称          | 说明                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数          | 类型     | 说明                                                                                            |
| :----------------- | :------- | :----------------------------------------------------------------------------------------------------- |
| sessionId          | string   | 应用程序状态会话的 ID。                                                          |
| availability       | string   | 基本状态信息。                                                                         |
| 活动           | string   | 可用性的补充信息。                                                          |
| expirationDuration | duration | 应用状态会话的过期时间。 该值以 ISO 8601 格式表示，持续时间为。</p>如果未提供，将应用 5 分钟的默认过期时间。 |

> [!IMPORTANT]
>
> 提供请求中应用程序 `sessionId` ID。

支持的 和 `availability` `activity` 的组合包括：

| availability | 活动          | 说明                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| 可用    | 可用         | 将状态会话更新为"可用"。               |
| 忙碌         | InACall           | 将状态会话更新为 Busy、InACall。           |
| 忙碌         | InAConferenceCall | 将状态会话更新为 Busy、InAConferenceCall。 |
| 离开         | 离开              | 将状态会话更新为离开。                    |

## <a name="response"></a>响应
如果成功，此方法返回 `200 OK` 响应代码。

## <a name="examples"></a>示例
以下请求显示 ID 为 `22553876-f5ab-4529-bffb-cfe50aa89f87` 用户设置其状态会话的应用程序 `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` 。

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "set-presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87",
  "availability": "Available",
  "activity": "Available",
  "expirationDuration": "PT1H"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/set-presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/set-presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/set-presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/set-presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/set-presence-go-snippets.md)]
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
