---
title: 获取 dataPolicyOperation
description: 检索 dataPolicyOperation 对象的属性。
ms.openlocfilehash: f2894b7cc23d6a5d35a03c7626ca9cb4640a9fcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042896"
---
# <a name="get-datapolicyoperation"></a>获取 dataPolicyOperation

检索 dataPolicyOperation 对象的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
|委派（个人 Microsoft 帐户） |  不适用  |
|应用程序 | Directory.Read.All、Directory.ReadWrite.All | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/<id>
```

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | 持有者 {token}|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法返回`200 OK`响应正文中的响应代码和[dataPolicyOperation](../resources/datapolicyoperation.md)对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/<id>
```
##### <a name="response"></a>响应
注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
