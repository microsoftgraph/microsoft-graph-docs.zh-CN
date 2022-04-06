---
title: participant： stopHoldMusic
description: 重新合并之前置于呼叫保留状态的参与者。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7665fc34203bf6b25f8e23cc93bca2d6f6593f2a
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64607937"
---
# <a name="participant-stopholdmusic"></a>participant： stopHoldMusic

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

重新合并之前置于呼叫保留状态的参与者。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。                               |
| 委派（个人 Microsoft 帐户） | 不支持。                               |
| Application                            | Calls.JoinGroupCallsasGuest.All 或 Calls.JoinGroupCalls.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /communications/calls/{id}/participants/{id}/stopHoldMusic
```

## <a name="request-headers"></a>请求标头
| 名称          | 说明               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}。必需。 |
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数      | 类型    |说明|
|:---------------|:--------|:----------|
|clientContext|String|可选。 唯一的客户端上下文字符串。 最多可包含 256 个字符。|

## <a name="response"></a>响应
如果成功，此方法在响应 `202 Accepted` 正文中返回 响应代码和 [stopHoldMusicOperation](../resources/stopHoldmusicoperation.md) 对象。

## <a name="example"></a>示例
以下示例演示如何调用此 API。

### <a name="request"></a>请求
请求示例如下所示。



# <a name="http"></a>[HTTP](#tab/http)
<!-- { 
  "blockType": "request", 
  "name": "participant-stopHoldMusic" 
}-->
```http
POST https://graph.microsoft.com/beta/communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/participants/fa1e9582-7145-4ca3-bcd8-577f561fcb6e/stopHoldMusic
Content-type: application/json

{
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/participant-stopholdmusic-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/participant-stopholdmusic-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/participant-stopholdmusic-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/participant-stopholdmusic-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/participant-stopholdmusic-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/participant-stopholdmusic-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 
 
<!-- { 
  "blockType": "response", 
  "truncated": true, 
  "@odata.type": "microsoft.graph.stopHoldMusicOperation" 
} --> 
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5

{
  "@odata.type": "#microsoft.graph.stopHoldMusicOperation",
  "id": "0fe0623f-d628-42ed-b4bd-8ac290072cc5",
  "status": "completed",
  "clientContext": "d45324c1-fcb5-430a-902c-f20af696537c",
  "resultInfo": null
}
```
