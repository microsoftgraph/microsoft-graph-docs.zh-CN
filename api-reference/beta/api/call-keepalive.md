---
title: call： keepAlive
description: 每隔 15 到 45 分钟对此 API 提出请求，以确保正在进行的调用保持活动状态。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 596a1d6abd9eb4986aa97cb31f8d956bbc2822c4
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607944"
---
# <a name="call-keepalive"></a>call： keepAlive

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

每隔 15 到 45 分钟对此 API 提出请求，以确保正在进行的调用保持活动状态。 在 45 分钟内未收到此请求的呼叫被视为非活动状态，随后将结束。

必须在上一个请求或调用开始后 45 分钟内至少提出一个成功请求。

我们建议您以较短的时间间隔发送请求， (每隔 15 分钟) 。 确保这些请求成功防止呼叫超时和结束。

尝试向已结束的呼叫发送请求将导致错误 `404 Not-Found` 。 与调用相关的资源应在应用程序端清理。

## <a name="permissions"></a>Permissions
调用此 API 可能需要以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
| :-------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | 不支持        |
| 委派（个人 Microsoft 帐户） | 不支持        |
| Application     | Calls.Initiate.All、Calls.AccessMedia.All |

> **注意：** 创建调用时检查权限;调用此 API 时，不会进行其他权限检查。 Calls.AccessMedia.All 仅对于使用应用托管媒体的呼叫是必需的。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/keepAlive
```


## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
此方法返回 HTTP `200 OK` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "keep-alive"
}-->

```http
POST https://graph.microsoft.com/beta/communications/calls/2e1a0b00-2db4-4022-9570-243709c565ab/keepAlive
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/keep-alive-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/keep-alive-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/keep-alive-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/keep-alive-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/keep-alive-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/keep-alive-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
以下示例显示了相应的响应。
<!-- {
  "blockType": "response",
  "name": "keep-alive"
} -->
```http
HTTP/1.1 200 OK
```


<!--
{
  "type": "#page.annotation",
  "description": "call: keepAlive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


