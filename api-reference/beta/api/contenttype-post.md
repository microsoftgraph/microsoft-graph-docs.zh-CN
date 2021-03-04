---
author: swapnil1993
title: 创建 contentType
description: 在网站中创建内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: f84ec9db88917b55f518bbdbd4660bf91e9321ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446115"
---
# <a name="create-contenttype"></a>创建 contentType
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在网站[中创建新的 contentType。][] [][]

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All    |
|委派（个人 Microsoft 帐户） |不支持    |
|Application | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |


## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/contentTypes

```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供要创建的 [contentType][] 资源的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应 `201 Created` 代码和 [contentType][] 对象。


## <a name="example"></a>示例

以下示例演示如何创建新的通用内容类型。

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_contenttype"
}
-->

```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes
Content-Type: application/json

{
    "name": "docSet",
    "description": "custom docset",
    "parentReference": {
        name: "Document Set",
        id: "0x0120D520"
    },
    "group": "Document Set Content Types" 
}
```

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "0x01002A2479FF33DD4BC3B1533A012B653717",
  "name": "docSet",
  "group":"Document Set Content Types",
  "description" : "custom docset",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```


[contentType]: ../resources/contentType.md
[网站]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a Content type in a site",
  "keywords": "content type",
  "section": "documentation",
  "tocPath": "sites/Create ContentType",
  "suppressions": [
  ]
}
-->
