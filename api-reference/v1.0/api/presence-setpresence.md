---
title: presence： setPresence
description: 设置用户应用程序状态会话的状态信息。
author: jsandoval-msft
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: c65754ffa61f62577ce4023d9a4a6e48ce0d533e
ms.sourcegitcommit: a11c874a7806fb5825752c8348e12079d23323e4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2022
ms.locfileid: "65293954"
---
# <a name="presence-setpresence"></a>presence： setPresence

命名空间：microsoft.graph

将用户的状态会话设置为应用程序。

### <a name="presence-sessions"></a>状态会话
用户可以有多个状态会话，因为用户可以在桌面、移动和 Web)  (多个Teams客户端上。 每个Teams客户端都有一个独立的状态会话，并且用户的状态是后面所有会话的聚合状态。

同样，应用程序可以为用户拥有自己的状态会话，并能够更新状态。

以下是聚合会话状态的优先级：
* 用户配置的>应用配置的 (用户配置状态替代其他) 
* 在配置的应用中：DoNotDisturb (当前不支持设置状态) >忙>可用>离开

### <a name="timeout-expiration-and-keep-alive"></a>超时、过期和保持活动状态
状态会话可能会 **超时** 和 **过期**，因此应用程序需要在 **超时** 前调用此 API 来维护会话的状态;或在 **过期** 之前，为了使会话保持活动状态。

如果可用性为 `Available` 且超时为 5 分钟，则状态会话可能会超时。 超时时时，状态将分阶段淡出。 例如，如果应用程序将状态会话设置为 `Available/Available`，状态将在第一次超时后更改为 `Available/AvailableInactive` 5 分钟，然后 `Away/Away` 在 5 分钟内再进行第二次超时。

状态会话的过期可使用 `expirationDuration` 参数进行配置。 当会话过期时，它将变为 `Offline`。

## <a name="permissions"></a>权限
调用 API 需要以下权限。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | Presence.ReadWrite                              |
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
| sessionId          | string   | 应用程序的状态会话的 ID。                                                          |
| availability       | string   | 基本状态信息。                                                                         |
| 活动           | string   | 可用性的补充信息。                                                          |
| expirationDuration | duration | 应用状态会话过期。 该值在持续时间内以 ISO 8601 格式表示。</p>如果未提供，将应用默认过期 5 分钟。 有效持续时间范围为 5-240 分钟 (PT5M 到 PT4H) |

> [!IMPORTANT]
>
> 提供应用程序的 ID，如请求中所示 `sessionId` 。

支持的组合包括`availability``activity`：

| availability | 活动          | 说明                                              |
| :----------- | :---------------- | :------------------------------------------------------- |
| 可用    | 可用         | 将状态会话更新为可用。               |
| 忙碌         | InACall           | 将状态会话更新为 Busy、InACall。           |
| 忙碌         | InAConferenceCall | 将状态会话更新为 Busy、InAConferenceCall。 |
| 离开         | 离开              | 将状态会话更新为“离开”。                    |

## <a name="response"></a>响应
如果成功，此方法返回 `200 OK` 响应代码。

## <a name="examples"></a>示例
以下请求显示 ID `22553876-f5ab-4529-bffb-cfe50aa89f87` 为用户设置其状态会话的应用程序 `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`。

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

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/set-presence-powershell-snippets.md)]
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
