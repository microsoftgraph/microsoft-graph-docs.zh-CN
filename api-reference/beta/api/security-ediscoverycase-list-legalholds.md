---
title: 列出 ediscoveryHoldPolicies
description: 获取 ediscoveryHoldPolicy 对象及其属性的列表。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 748b3de6efce13e7b07af6e10b2a98275d8eaac0
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838029"
---
# <a name="list-ediscoveryholdpolicies"></a>列出 ediscoveryHoldPolicies
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象及其属性的列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|eDiscovery.Read.All、eDiscovery.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/legalHolds
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_ediscoveryholdpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/legalHolds
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-ediscoveryholdpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-ediscoveryholdpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-ediscoveryholdpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-ediscoveryholdpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-ediscoveryholdpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryHoldPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/legalHolds",
    "@odata.count": 2,
    "value": [
        {
            "isEnabled": false,
            "errors": [],
            "contentQuery": "",
            "description": null,
            "createdDateTime": "2022-05-23T01:09:53Z",
            "lastModifiedDateTime": "2022-05-23T02:36:26Z",
            "status": "pending",
            "id": "783c3ea4-d474-4051-9c13-08707ce8c8b6",
            "displayName": "CustodianHold-b0073e4e-4184-41c6-9eb7-8c8cc3e2288b",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "MOD Administrator",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "user": {
                    "id": "MOD Administrator",
                    "displayName": null
                }
            }
        },
        {
            "isEnabled": false,
            "errors": [],
            "contentQuery": "",
            "description": null,
            "createdDateTime": "2022-05-23T02:09:27Z",
            "lastModifiedDateTime": "2022-05-23T02:41:26Z",
            "status": "pending",
            "id": "ff7e8841-b1ac-41f0-87c5-fa00da045ae0",
            "displayName": "NCDSHold-b0073e4e-4184-41c6-9eb7-8c8cc3e2288b",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "MOD Administrator",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "user": {
                    "id": "MOD Administrator",
                    "displayName": null
                }
            }
        }
    ]
}
```

