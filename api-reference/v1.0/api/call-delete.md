---
title: 删除呼叫
description: 删除或挂断活动呼叫。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5c110e83cfe5bb0fdd7e9c93377d5b8c901b330d
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630798"
---
# <a name="delete-call"></a>删除呼叫

命名空间：microsoft.graph

删除或挂断活动呼叫。 对于组呼叫，这只会删除你的通话记录，基础组呼叫将继续。

## <a name="permissions"></a>权限

| 权限类型 | 权限（从最低特权到最高特权）                  |
| :-------------- | :----------------------------------------------------------- |
| 委派（工作或学校帐户）     | 不支持。                         |
| 委派（个人 Microsoft 帐户） | 不支持。                         |
| 应用程序                            | Calls.Initiate.All、Calls.AccessMedia.All |

> **注意：** 创建调用时检查权限;调用此 API 时，不会进行其他权限检查。 Calls.AccessMedia.All 仅对于使用应用托管媒体的呼叫是必需的。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}
```

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面为请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call-1"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-call-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-call-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="notification---terminating"></a>通知 - 终止

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

### <a name="notification---terminated"></a>Notification - 已终止

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": "200",
          "subcode": "5001",
          "message": "The conversation has ended."
        }
      }
    }
  ]
}
```

#### <a name="call-end-reason-codes"></a>呼叫结束原因代码

这些是呼叫终止时通过通知收到的一些常见错误代码。

| 代码 | 子代码 | 终止原因                                                                                 |
| :--- | :------  | :------------------------------------------------------------------------------------------------  |
| 200  | 4097     | 呼叫由呼叫中的另一个参与者结束。                                                   |
| 200  | 4521     | 对等呼叫中其他参与者结束的呼叫。                                          |
| 200  | 5000     | 由另一个参与者从对话中删除。                                              |
| 200  | 5001     | 对话已结束。                                                                        |
| 200  | 5002     | 对话已结束，因为所有其他参与者已离开呼叫。                           |
| 200  | 5003     | 对话已结束。                                                                        |
| 200  | 5007     | 对话已作为组呼叫发起人离开对话结束。               |
| 200  | 5010     | 对话已结束，因为只有一个参与者留在对话中。                   |
| 200  | 5012     | 对话已结束，因为传入名单中没有参与者。                    |
| 200  | 5013     | 对话已结束，因为其他人都未加入组呼叫。                               |
| 200  | 5014     | 对话已结束，因为我们无法确定组呼叫的潜在主机。 |
| 200  | 5020     | 对话已结束，因为传入名单中没有非隐藏参与者。         |
| 200  | 5030     | 对话已结束，因为聊天室持续时间已过。                              |
| 200  | 5300     | 参与者已被另一个参与者从对话中删除。                              |
| 200  | 5855     | 大厅不活动超时后，在大厅中等待的参与者已从对话中删除。     |
| 200  | 7000     | 对话已由机器人结束。                                                                 |
| 200  | 7015     | 呼叫在转接成功完成时结束。                                                 |
| 200  | 10550    | 对话已由机器人结束。                                                                 |
| 200  | 18503    | 对等呼叫中的另一个参与者离开对话。                              |
| 200  | 540000/560000   | 呼叫由 PSTN 用户结束。                                                                |
| 408  | 8537     | 保持活动状态超时，清理非活动呼叫。                                                      |
| 408  | 1106     | 在分配的时间内未收到呼叫接受的确认。                  |
| 408  | 10057    | 由于被叫方终结点没有信号，呼叫被叫方被叫出。                                          |
| 410  | 301005   | 媒体连接失败。                                                                        |
| 480  | 10037    | 未找到被叫方终结点。                                                                    |
| 480  | 10076    | 无法联系被叫方。                                                                       |
| 480  | 10134    | 由于无法路由呼叫，呼叫被拒绝。                                                  |
| 480  | 10199    | 用户已禁用作为私人呼叫拒绝的呼叫。                                         |
| 500  | 1005     | 服务器遇到自动程序媒体连接错误。 请检查 Bot 和 Microsoft 之间的媒体连接。 |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

