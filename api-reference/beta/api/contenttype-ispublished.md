---
author: swapnil1993
title: contentType： isPublished
description: 检查内容类型中心网站中内容类型的发布状态。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: d6f5700015dcb69ce3440be187654941816e0a9d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446123"
---
# <a name="contenttype-ispublished"></a>contentType： isPublished
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
检查内容类型中心网站 [中 contentType][] 的发布状态。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.FullControl.All    |
|委派（个人 Microsoft 帐户） | 不支持   |
|Application | Sites.FullControl.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
>**注意：** siteId 表示内容类型中心网站。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="response"></a>响应
如果成功，此调用将返回一个响应和一个指定内容类型的发布状态 `200 OK` 布尔值。

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```http
GET https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true 
}
```

[contentType]: ../resources/contentType.md
