---
title: 列出 ediscoveryNoncustodialDataSources
description: 获取 ediscoveryNoncustodialDataSource 对象的列表。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e1a49e58687c5cafb16eb7e11ebd495a395b60da
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838344"
---
# <a name="list-ediscoverynoncustodialdatasources"></a>列出 ediscoveryNoncustodialDataSources
命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [非托管数据源](../resources/security-ediscoverynoncustodialdatasource.md) 及其属性的列表。

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求
请求示例如下所示。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_ediscoverynoncustodialdatasource_from_"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources?$expand=dataSource
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-ediscoverynoncustodialdatasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-ediscoverynoncustodialdatasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-ediscoverynoncustodialdatasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-ediscoverynoncustodialdatasource-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryNoncustodialDataSource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources(dataSource())",
    "@odata.count": 3,
    "value": [
        {
            "status": "active",
            "holdStatus": "applied",
            "createdDateTime": "2022-05-23T02:09:11.1395287Z",
            "lastModifiedDateTime": "2022-05-23T02:09:11.1395287Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "35393639323133394345384344303043",
            "displayName": "U.S. Sales",
            "dataSource@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources('35393639323133394345384344303043')/dataSource/$entity",
            "dataSource": {
                "@odata.type": "#microsoft.graph.security.siteSource",
                "@odata.id": "https://graph.microsoft.com/v1.0/sites/169718e3-a8df-449d-bef4-ee09fe1ddc5d",
                "displayName": "U.S. Sales",
                "createdDateTime": "2022-05-23T02:09:11.1395535Z",
                "holdStatus": "0",
                "id": "169718e3-a8df-449d-bef4-ee09fe1ddc5d",
                "createdBy": {
                    "application": null,
                    "user": {
                        "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                        "displayName": null
                    }
                },
                "site": {
                    "webUrl": "https://m365x809305.sharepoint.com/sites/USSales",
                    "id": "169718e3-a8df-449d-bef4-ee09fe1ddc5d",
                    "createdDateTime": "2022-05-23T02:09:11.1395535Z"
                }
            }
        },
        {
            "status": "active",
            "holdStatus": "applied",
            "createdDateTime": "2022-05-23T02:09:11.1395287Z",
            "lastModifiedDateTime": "2022-05-23T02:09:11.1395287Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "31453237353743363432414242344641",
            "displayName": "Sales and Marketing",
            "dataSource@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources('31453237353743363432414242344641')/dataSource/$entity",
            "dataSource": {
                "@odata.type": "#microsoft.graph.security.siteSource",
                "@odata.id": "https://graph.microsoft.com/v1.0/sites/74f6c798-fc32-4dbe-9e5b-8e11459b9f44",
                "displayName": "Sales and Marketing",
                "createdDateTime": "2022-05-23T02:09:11.1397925Z",
                "holdStatus": "0",
                "id": "74f6c798-fc32-4dbe-9e5b-8e11459b9f44",
                "createdBy": {
                    "application": null,
                    "user": {
                        "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                        "displayName": null
                    }
                },
                "site": {
                    "webUrl": "https://m365x809305.sharepoint.com/sites/SalesAndMarketing",
                    "id": "74f6c798-fc32-4dbe-9e5b-8e11459b9f44",
                    "createdDateTime": "2022-05-23T02:09:11.1397925Z"
                }
            }
        },
        {
            "status": "active",
            "holdStatus": "applied",
            "createdDateTime": "2022-05-23T02:09:11.1395287Z",
            "lastModifiedDateTime": "2022-05-23T02:09:11.1395287Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "46333131344239353834433430454335",
            "displayName": "Retail",
            "dataSource@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources('46333131344239353834433430454335')/dataSource/$entity",
            "dataSource": {
                "@odata.type": "#microsoft.graph.security.siteSource",
                "@odata.id": "https://graph.microsoft.com/v1.0/sites/dbe4b18e-2765-4989-8647-48139180c45f",
                "displayName": "Retail",
                "createdDateTime": "2022-05-23T02:09:11.1399861Z",
                "holdStatus": "0",
                "id": "dbe4b18e-2765-4989-8647-48139180c45f",
                "createdBy": {
                    "application": null,
                    "user": {
                        "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                        "displayName": null
                    }
                },
                "site": {
                    "webUrl": "https://m365x809305.sharepoint.com/sites/Retail",
                    "id": "dbe4b18e-2765-4989-8647-48139180c45f",
                    "createdDateTime": "2022-05-23T02:09:11.1399861Z"
                }
            }
        }
    ]
}
```

