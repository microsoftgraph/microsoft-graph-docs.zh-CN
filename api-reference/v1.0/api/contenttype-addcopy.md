---
author: swapnil1993
title: contentType：addCopy
description: 将网站内容类型的副本添加到列表中。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 819e0c3bcf5455153d53eb8b84f423f99afebe67
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696524"
---
# <a name="contenttype-addcopy"></a>contentType：addCopy
命名空间：microsoft.graph


将内容类型[contentType] [的副本从][网站添加到][site][列表][list]。
 
  

## <a name="permissions"></a>权限  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |Sites.Manage.All、Sites.FullControl.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Sites.Manage.All、Sites.FullControl.All |

  

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

如果成功，此调用在响应 `201 Created` 正文中返回 响应代码和 [contentType][] 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "contenttype_addcopy"
}
-->
```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/contentTypes/addCopy
Content-Type: application/json

{
  "contentType": "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101"
}
```


### <a name="response"></a>响应


<!-- { "blockType": "response", "@type": "microsoft.graph.contentType", "truncated": true} -->

```http
HTTP/1.1 201 Created

{
    "id": "0x0101",
    "description": "Create a new custom CSR JavaScript Display Template.",
    "group": "Display Template Content Types",
    "hidden": false,
    "name": "JavaScript Display Template",
    "parentId": "0x01",
    "readOnly": false,
    "sealed": false,
    "base": {
        "id": "0x01",
        "description": "Create a new custom CSR JavaScript Display Template.",
        "group": "Display Template Content Types",
        "hidden": false,
        "name": "JavaScript Display Template",
        "readOnly": false,
        "sealed": false
    }
}
```

[site]: ../resources/site.md
[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
