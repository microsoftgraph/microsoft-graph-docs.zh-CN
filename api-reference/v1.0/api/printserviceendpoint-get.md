---
title: 获取 printServiceEndpoint
description: 检索打印服务终结点的属性和关系。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 4668399829c08771db185727e4c791c611013a26
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992541"
---
# <a name="get-printserviceendpoint"></a>获取 printServiceEndpoint
命名空间：microsoft.graph

检索打印服务终结点的属性和关系。

## <a name="permissions"></a>权限
调用 **此** API 需要委派 [的通用打印权限](/graph/permissions-reference#universal-print-permissions) 之一。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services/{printServiceId}/endpoints/{printServiceEndpointId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [printServiceEndpoint](../resources/printserviceendpoint.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printserviceendpoint"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services/{printServiceId}/endpoints/{printServiceEndpointId}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printserviceendpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printserviceendpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printserviceendpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printserviceendpoint-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-printserviceendpoint-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printServiceEndpoint"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.printServiceEndpoint)",
  "id": "mpsdiscovery",
  "displayName": "Microsoft Universal Print Discovery Service",
  "uri": "https://discovery.print.microsoft.com"
}
```

