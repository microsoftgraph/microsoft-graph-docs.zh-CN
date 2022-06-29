---
title: 列出 documentSetVersions
description: 获取列表中文档集项的版本列表。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: d72e340a9804ecd5e71f86767066154613ab48fa
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447365"
---
# <a name="list-documentsetversions"></a>列出 documentSetVersions
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取列表中[文档集项的版本](../resources/documentsetversion.md)[列表](../resources/list.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）| Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All|
|委派（个人 Microsoft 帐户）| 不支持。 |
|应用程序| Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All、Sites.Selected|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{siteId}/lists/{listId}/items/{itemId}/documentSetVersions
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

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [documentSetVersion](../resources/documentsetversion.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_documentsetversion"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/root/lists/Documents/items/1/documentSetVersions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-documentsetversion-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-documentsetversion-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-documentsetversion-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-documentsetversion-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-documentsetversion-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-documentsetversion-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "name": "list_documentsetversion",
  "truncated": true,
  "@odata.type": "microsoft.graph.documentSetVersion",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "value": [
        {
            "id": "2",
            "lastModifiedDateTime": "2022-04-05T04:55:29Z",
            "comment": "v2",
            "createdDateTime": "2022-04-05T04:55:29Z",
            "shouldCaptureMinorVersion": false,
            "lastModifiedBy": {
                "user": {
                    "displayName": "Tenant Admin User",
                    "email": "admin@contoso.sharepoint.com"
                }
            },
            "items": [
                {
                    "itemId": "a5d83ae7-8c3e-4a2c-bc3e-8f276db857bf",
                    "versionId": "1.0"
                },
                {
                    "itemId": "62d40672-befe-4017-934b-06372fd96022",
                    "versionId": "1.0"
                }
            ],
            "createdBy": {
                "user": {
                    "displayName": "Tenant Admin User",
                    "email": "admin@contoso.sharepoint.com"
                }
            }
        },
        {
            "id": "1",
            "lastModifiedDateTime": "2022-04-05T04:53:42Z",
            "comment": "v1",
            "createdDateTime": "2022-04-05T04:53:42Z",
            "shouldCaptureMinorVersion": false,
            "lastModifiedBy": {
                "user": {
                    "displayName": "Tenant Admin User",
                    "email": "admin@contoso.sharepoint.com"
                }
            },
            "items": [
                {
                    "itemId": "a5d83ae7-8c3e-4a2c-bc3e-8f276db857bf",
                    "versionId": "1.0"
                }
            ],
            "createdBy": {
                "user": {
                    "displayName": "Tenant Admin User",
                    "email": "admin@contoso.sharepoint.com"
                }
            }
        }
    ]
}
```

