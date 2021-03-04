---
author: swapnil1993
title: 删除 columnDefinition
description: 从内容类型中删除列。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: fb5df6389c4723cf48185a74f72c1009a3ac031b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446130"
---
# <a name="delete-columndefinition"></a>删除 columnDefinition
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
从[列表][columndefinition]或[网站][]内容类型[中删除][][列][contentType]。


## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
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
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
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
