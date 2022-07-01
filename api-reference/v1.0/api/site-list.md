---
title: 列出网站
description: 列出组织中的所有可用网站，或列出与提供的筛选条件和查询选项匹配的站点。
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: f78db6d9ad4d4b2f772ed79451ff16853a514d4e
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578100"
---
# <a name="list-sites"></a>列出网站

命名空间：microsoft.graph

列出组织中所有可用 [的站点][] 。

还支持特定的筛选条件和查询选项，如下所述：

| Filter 语句             | Select 语句        | 说明
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | 列出组织中的所有根级网站集。 可用于发现每个地理位置的主站点。

此外，还可以对集合使用 **[$search][]** 查询 `/sites` 来查找与给定关键字匹配的网站。

[$search]: site-search.md
[sites]: ../resources/site.md

有关生成使用站点发现进行扫描的应用程序的更多指南，请参阅 [有关发现文件和大规模检测更改的最佳做法](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="list-all-site-collections"></a>列出所有网站集

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。                              |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | Sites.Read.All、Sites.ReadWrite.All         |

### <a name="discover-the-home-site-for-each-geography"></a>发现每个地理位置的主站点

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Sites.Read.All、Sites.ReadWrite.All         |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | Sites.Read.All、Sites.ReadWrite.All         |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /sites
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a>示例

### <a name="request"></a>请求


<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```

### <a name="request"></a>请求

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/sites
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,bf6fb551-d508-4946-a439-b2a6154fc1d9,65a04b8b-1f44-442b-a1fc-9e5852fb946c",
      "name": "Root Site",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso.sharepoint.com,d9ecf079-9b13-4376-ac5d-f242dda55626,746dbcc1-fa2b-4120-b657-2670bae5bb6f",
      "name": "Site A",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com"
      },
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,fd1a778f-263e-4c43-acdf-d5c2519d80eb,c06016db-dfec-4f79-83a1-09c6dbfd7022",
      "name": "Site B",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com"
      },
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->


