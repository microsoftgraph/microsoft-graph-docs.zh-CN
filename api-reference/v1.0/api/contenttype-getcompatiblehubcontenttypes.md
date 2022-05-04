---
title: contentType： getCompatibleHubContentTypes
description: 从内容类型中心获取可添加到目标网站或列表的兼容内容类型的列表。
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: 1d0f5d421e1f1f68298c555c8e7dad9dd81f294f
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191840"
---
# <a name="contenttype-getcompatiblehubcontenttypes"></a>contentType： getCompatibleHubContentTypes
命名空间：microsoft.graph

从内容类型中心获取可添加到目标 [网站](../resources/site.md) 或列表的兼容内容类型的 [列表](../resources/list.md)。

此方法是内容类型发布更改的一部分，旨在优化已发布内容类型与网站和列表的同步，从而有效地从“随处推送”切换为“根据需要拉取”。 该方法允许用户直接从内容类型中心将内容类型拉取到网站或列表。 有关详细信息，请参阅 [contentType：addCopyFromContentTypeHub](contenttype-addcopyfromcontenttypehub.md) 和博客文章 [Syntex Product Updates – 2021 年 8 月](https://techcommunity.microsoft.com/t5/sharepoint-syntex-blog/syntex-product-updates-august-2021/ba-p/2606438)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|Application | Sites.Manage.All、Sites.FullControl.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{siteId}/lists/{listId}/contentTypes/getCompatibleHubContentTypes
GET /sites/{siteId}/contentTypes/getCompatibleHubContentTypes
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 `200 OK` 响应代码和 [contentType](../resources/contenttype.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "contenttype_getcompatiblehubcontenttypes"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/sites/root/lists/Documents/contentTypes/getCompatibleHubContentTypes
```

### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contentType",
      "id": "0x0101",
      "description": "Document content type",
      "group": "Document Content Types",
      "hidden": false,
      "isBuiltIn": true,
      "name": "Document"
    }
  ]
}
```

