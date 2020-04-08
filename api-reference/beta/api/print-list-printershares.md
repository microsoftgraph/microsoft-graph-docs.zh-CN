---
title: 获取 printerShares
description: 检索打印机共享的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 02fc83e45a19165a23600c9c03bc94e74ff9f493
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42948286"
---
# <a name="list-printershares"></a>列出 printerShares

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索**printerShares**的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| 已阅读的用户。所有 |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /print/printerShares
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。

### <a name="exceptions"></a>异常

* `$count`运算符不受支持。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法在响应`200 OK`正文中返回响应代码和[printerShare](../resources/printershare.md)对象集合。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershares"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printerShares
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershares-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershares-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershares-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 269

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "name": "PrinterShareName",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List printerShares",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
