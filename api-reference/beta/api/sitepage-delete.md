---
author: rahmit
description: 从网站的 "网站页面" 列表中删除 sitePage。
ms.date: 05/07/2018
title: 从 SharePoint 网站中删除页面
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d573553ee87b70adfd1f2cde575ce6182dedf8b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044485"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a>从网站的 "网站页面" 列表中删除页面

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从[网站][]的 "网站页面"[列表][]中删除[sitePage][] 。

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a>权限

需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。

>**注意：** 若要删除项，用户必须已授予应用程序对要删除的项的写入权限。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a>可选的请求标头

| 名称       | 值 | 说明
|:-----------|:------|:--------------------------------------------------------
| _if-match_ | etag  | 如果包含此请求标头，且提供的 eTag 与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。

## <a name="request-body"></a>请求正文

请勿为此方法提供请求正文。
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a>响应

如果成功，此调用将返回 `204 No Content` 响应，表示资源已被删除，没有任何可返回的内容。

## <a name="example"></a>示例

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a>请求

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a>响应

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": []
}
-->


