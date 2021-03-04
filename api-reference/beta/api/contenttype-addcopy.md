---
author: swapnil1993
title: contentType：addCopy
description: 将网站内容类型的副本添加到列表中。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 955afab160cb5c927771db4132ec208b85e80b2a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446137"
---
# <a name="contenttype-addcopy"></a>contentType：addCopy
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
将网站内容[类型][site][的副本添加到][contentType][列表中][list]。
 
  

## <a name="permissions"></a>Permissions  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
```http

POST /sites/{site-id}/lists/{list-id}/contentTypes/addCopy
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|-|-|-|
|contentType| string | 将复制到列表的网站内容类型的规范 URL。 必需。|

## <a name="response"></a>响应

如果成功，此调用将返回 `204 No Content` 响应。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopy"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/lists/{list-id}/contentTypes/addCopy
Content-Type: application/json

{
  "contentType": "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
}
```



### <a name="response"></a>响应


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
