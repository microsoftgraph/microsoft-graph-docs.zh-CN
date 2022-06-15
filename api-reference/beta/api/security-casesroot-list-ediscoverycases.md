---
title: 列出 ediscoveryCases
description: 获取电子数据展示案例的列表
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: dd70dbb010fcdfff5aa8e90cc88ff3714a8f75e9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092491"
---
# <a name="list-ediscoverycases"></a>列出 ediscoveryCases
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [ediscoveryCase](../resources/security-ediscoverycase.md) 对象及其属性的列表。

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
GET /security/cases/ediscoveryCases
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [ediscoveryCase](../resources/security-ediscoverycase.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_ediscoverycase"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/ediscoveryCases
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-ediscoverycase-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面是响应的示例
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryCase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases",
    "@odata.count": 22,
    "value": [
        {
            "description": "",
            "lastModifiedDateTime": "2022-05-19T23:30:41.23Z",
            "status": "active",
            "closedDateTime": null,
            "externalId": "",
            "id": "60f86305-ac3e-408b-baa2-ea585dd8b0c0",
            "displayName": "My case 1",
            "createdDateTime": "2022-05-19T23:30:41.23Z",
            "lastModifiedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": "MOD Administrator"
                }
            },
            "closedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": ""
                }
            }
        },
        {
            "description": "",
            "lastModifiedDateTime": "2022-05-18T23:05:07.82Z",
            "status": "active",
            "closedDateTime": null,
            "externalId": "",
            "id": "7acdda75-3559-4f93-9827-cbd4c89db033",
            "displayName": "My case 2",
            "createdDateTime": "2022-05-18T23:05:07.82Z",
            "lastModifiedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": "MOD Administrator"
                }
            },
            "closedBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": ""
                }
            }
        }
    ]
}
```

