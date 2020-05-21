---
title: 使用的列表
description: '计算并列出用户已查看或修改的文档。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 332d4b7bb9650128b31289b251a30cbb193f75b4
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335137"
---
# <a name="list-used"></a>使用的列表

命名空间：microsoft.graph

计算并列出用户已查看或修改的文档。 

对于登录用户：
- 此方法包括用户已修改的文档;请参阅[示例 1](#example-1-return-documents-that-user-has-modified)。 
- 使用 `$orderby` **lastAccessedDateTime**属性上的查询参数返回用户可能已修改或可能尚未修改的最近查看过的文档; 请参阅[示例 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified)。

对于其他用户，此方法仅包括用户已修改的文档。


## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Read.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

- 获取已登录用户已修改的文档列表：
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used
  ```

- 获取指定用户修改的文档的列表：
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /users/{id | userPrincipalName}/insights/used
  ```
  >**注意**：请求其他用户的已**使用**文档返回按**lastModifiedDateTime**排序的结果。 然后，将**lastAccessedDateTime**设置为**lastModifiedDateTime**。


- 扩展**使用**的洞察力引用的资源：
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/insights/used/{id}/resource
  GET /users/{id | userPrincipalName}/insights/used/{id}/resource
  ```


## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持[OData 查询参数](/graph/query-parameters)来帮助自定义响应：

- 使用 `$filter` 查询参数筛选已使用的项目。 例如，基于**类型**：
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

- 使用 `$filter` 基于**containerType**筛选已使用的项目：
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

  请参阅可在[resourceVisualization](../resources/insights-resourcevisualization.md)中筛选的可用容器类型和类型。

- 使用 `$orderBy` 查询参数对_已登录用户_上次查看或修改的文档进行排序，基于**lastAccessedDateTime**属性：
  <!-- { "blockType": "ignored" } -->
  `https://graph.microsoft.com/v1.0/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc`

  >**注意**：_仅对已登录用户_使用此查询选项。 您不能使用此 API 获取其他用户查看或修改的文档。 请参阅[示例 2](#example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified)。


## <a name="request-headers"></a>请求标头
| 标头       |  值|
|:-------------|:------|
| Authorization  | Bearer {token}。必需。|
| 接受  | application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在 `200 OK` 响应正文中返回响应代码和已[使用](../resources/insights-used.md)项的列表。
## <a name="example"></a>示例

### <a name="example-1-return-documents-that-user-has-modified"></a>示例1：返回用户已修改的文档

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifieddocuments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/insights/used
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifieddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifieddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifieddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifieddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('c74dcd16-d8af-4df8-9621-d123b58de3e6')/insights/used",
    "value": [
        {
            "id": "Abk3ZeZmlghMhUVKP9mygDoPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INA5k5RvS1T4tPmZSWjFY1PFu5N2XmZpYITIVFSj_ZsoA6BQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:12:38Z",
                "lastModifiedDateTime": "2019-05-25T07:12:37Z"
            },
            "resourceVisualization": {
                "title": "Org Chart",
                "type": "Visio",
                "mediaType": "application/vnd.visio",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3/thumbnails/0/small/thumbnailContent",
                "previewText": "Page-1",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/Retail/Shared Documents/NC460 Sales",
                "containerDisplayName": "Retail",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/Retail/_layouts/15/Doc.aspx?sourcedoc=%7BF4463999-4FB5-4F8B-9994-968C56353C5B%7D&file=Org%20Chart.vsdx&action=default&DefaultItemOpen=1",
                "id": "drives/b!uTdl5maWCEyFRUo_2bKAOg8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01JSNPH6EZHFDPJNKPRNHZTFEWRRLDKPC3",
                "type": "microsoft.graph.driveItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IwPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INA5T7emOJwqlCit_j9Q5CpWSlSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:12:26Z",
                "lastModifiedDateTime": "2019-05-25T07:12:26Z"
            },
            "resourceVisualization": {
                "title": "USA Sales",
                "type": "Excel",
                "mediaType": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJM4U7N5GHCOCVFBIVX7D6UHEFJLE/thumbnails/0/small/thumbnailContent",
                "previewText": "Product Category Product  Product Category - Product Target Revenue TY YTD Revenue Variance to Target Revenue COGS List Price % of List Price Actual Margin Target Margin Audio Car Audio Audio - Car Audio 4910000 4664500 245500 3928000 4320800 -736500 Audi",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/Shared Documents/Monthly Reports",
                "containerDisplayName": "Sales and Marketing",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/_layouts/15/Doc.aspx?sourcedoc=%7B637AFB94-C289-42A9-8ADF-E3F50E42A564%7D&file=USA%20Sales.xlsx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJM4U7N5GHCOCVFBIVX7D6UHEFJLE",
                "type": "microsoft.graph.driveItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IwPEPUbLediT7xb7UyGkIkmjsvR4JlgRUGA28jNM6INAy6LlBcXfAJCmOiEWgBJjh-lSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2019-05-25T07:11:49Z",
                "lastModifiedDateTime": "2019-05-25T07:11:48Z"
            },
            "resourceVisualization": {
                "title": "UK Sales",
                "type": "Excel",
                "mediaType": "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJMZOROKBOF34AJBJR2EELIAETDQ7/thumbnails/0/small/thumbnailContent",
                "previewText": "Product Category Product  Product Category - Product Target Revenue TY YTD Revenue Variance to Target Revenue COGS List Price % of List Price Actual Margin Target Margin Electronics Wearable Technology Electronics - Wearable Technology 2226000 2114700 111",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/Shared Documents/Monthly Reports",
                "containerDisplayName": "Sales and Marketing",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/_layouts/15/Doc.aspx?sourcedoc=%7B17948B2E-7C17-4202-98E8-845A00498E1F%7D&file=UK%20Sales.xlsx&action=default&mobileredirect=true&DefaultItemOpen=1",
                "id": "drives/b!pUjqfkqojkWMOo2cH874jA8Q9Rst52JPvFvtTIaQiSaOy9HgmWBFQYDbyM0zog0D/items/01YAUTJMZOROKBOF34AJBJR2EELIAETDQ7",
                "type": "microsoft.graph.driveItem"
            }
        }
    ]
}
```

### <a name="example-2-return-the-most-recently-viewed-documents-that-the-signed-in-user-might-or-might-not-have-modified"></a>示例2：返回已登录用户可能已修改或可能尚未修改的最近查看过的文档 

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mymodifiedandvieweddocuments"
}-->
  
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/insights/used?$orderby=LastUsed/LastAccessedDateTime desc
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mymodifiedandvieweddocuments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mymodifiedandvieweddocuments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mymodifiedandvieweddocuments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mymodifiedandvieweddocuments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('c74dcd16-d8af-4df8-9621-d123b58de3e6')/insights/used",
    "value": [
        {
            "id": "AWTmrUBYzTxMsvtILkUktIaN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABk5q1AWM08TLL7SC5FJLSGBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Executive Corner",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!ZOatQFjNPEyy-0guRSS0ho36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01NTE4NPQAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Executive Corner",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/Exec",
                "id": "sites/m365x887078.sharepoint.com,40ade664-cd58-4c3c-b2fb-482e4524b486,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        },
        {
            "id": "AahdFRA14_FMrGLq9V4WmyiN-sDnMnRRTYqBxeih4bUUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACoXRUQNePxTKxi6vVeFpsoBA",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:55Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Contoso Landings",
                "type": "spsite",
                "mediaType": "application/octet-stream",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!qF0VEDXj8UysYur1XhabKI36wOcydFFNioHF6KHhtRQAAAAAAAAAAAAAAAAAAAAA/items/01UHO6LBAAAAAAAAAAAAAAAAAAAAAAAAAA/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerDisplayName": "Contoso Landings",
                "containerType": "Site"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/ContosoLandings",
                "id": "sites/m365x887078.sharepoint.com,10155da8-e335-4cf1-ac62-eaf55e169b28,e7c0fa8d-7432-4d51-8a81-c5e8a1e1b514",
                "type": "microsoft.graph.siteItem"
            }
        },
        {
            "id": "AaVI6n5KqI5FjDqNnB_O-IztQAKAS6acR7HFoIKDqOPE6bjkeoHWtEu7LoUIsZkHSkzLaA_67htEozMGRwifyaqlSOp-SqiORYw6jZwfzviMBQ",
            "lastUsed": {
                "lastAccessedDateTime": "2020-03-16T13:31:54Z",
                "lastModifiedDateTime": "0001-01-01T00:00:00Z"
            },
            "resourceVisualization": {
                "title": "Media Preview Packages",
                "type": "Web",
                "mediaType": "text/html",
                "previewImageUrl": "https://m365x887078.sharepoint.com/_api/v2.0/drives/b!pUjqfkqojkWMOo2cH874jO1AAoBLppxHscWggoOo48TpuOR6gda0S7suhQixmQdK/items/01RGQ6XKCMZNUA76XODNCKGMYGI4EJ7SNK/thumbnails/0/small/thumbnailContent",
                "previewText": "",
                "containerWebUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/CampaignsEvents/SitePages/Forms/ByAuthor.aspx",
                "containerDisplayName": "Campaigns - Events"
            },
            "resourceReference": {
                "webUrl": "https://m365x887078.sharepoint.com/sites/SalesAndMarketing/CampaignsEvents/SitePages/Media-Preview-Packages.aspx"
            }
        }
    ]
}
```
