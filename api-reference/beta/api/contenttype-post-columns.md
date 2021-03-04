---
author: swapnil1993
ms.date: 08/30/2020
title: 创建 columnDefinition
description: 向内容类型添加列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 071a855c79c055179022157b991b4a9f2789cad1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446117"
---
# <a name="create-columndefinition"></a>创建 columnDefinition
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
将现有网站或列表 [列][columnDefinition] 添加到 [内容类型][contentType 中]。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/concepts/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/contentTypes/{contentType-id}/columns
POST /sites/{site-id}/lists/{list-id}//contentTypes/{contentType-id}/columns
```

## <a name="request-body"></a>请求正文

在请求正文中，提供要添加的 [columnDefinition 资源的][] JSON 表示形式。  

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [contentType][] 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns
Content-Type: application/json

{
    "sourceColumn@odata.bind": "https://graph.microsoft.com/beta/sites/root/columns/99ddcf45-e2f7-4f17-82b0-6fba34445103",
}
```

### <a name="response"></a>响应

该响应返回添加到内容类型的所有列的列表。

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true, "scopes": "sites.readwrite.all" } -->

  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "",
  "displayName": "Title",
  "enforceUniqueValues": false,
  "hidden": false,
  "id": "99ddcf45-e2f7-4f17-82b0-6fba34445103",
  "indexed": false,
  "name": "Title",
  "text": {
    "allowMultipleLines": false,
    "appendChangesToExistingText": false,
    "linesForEditing": 0,
    "maxLength": 255
  }
}

```

  

[columnDefinition]: ../resources/columnDefinition.md
[contentType]: ../resources/contentType.md
  

