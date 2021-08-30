---
author: swapnil1993
title: 删除 columnDefinition
description: 从网站、列表或内容类型中删除列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: e367741d7225c0cee80626392458158de37cfb88
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696561"
---
# <a name="delete-columndefinition"></a>删除 columnDefinition
命名空间：microsoft.graph


从[网站][columndefinition][、列表][][或内容类型][]中删除[列][contentType]。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Sites.Manage.All、Sites.FullControl.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/columns/{column-id}
DELETE /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```
## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "delete_columns_from_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[columndefinition]: ../resources/columndefinition.md
[contentType]: ../resources/contentType.md
[网站]: ../resources/site.md
