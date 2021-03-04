---
author: swapnil1993
title: contentType：取消发布
description: 从内容类型中心网站取消发布内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ca432973337ac81f3ee8e632bb0705f26c7575ea
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446113"
---
# <a name="contenttype-unpublish"></a>contentType：取消发布
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
从内容类型中心网站取消发布[contentType。][]

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.FullControl.All    |
|委派（个人 Microsoft 帐户） | Sites.FullControl.All    |
|Application | Sites.FullControl.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

>**注意：** siteId 表示内容类型中心网站。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将返回 `204 No Content` 响应。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "contenttype_unpublish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

### <a name="response"></a>响应

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
