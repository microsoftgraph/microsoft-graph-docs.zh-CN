---
author: swapnil1993
title: contentType：associateWithHubSites
description: 将内容类型与中心网站列表关联。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8049eb6db5975c2e5c8600a654b6cc533124217f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446135"
---
# <a name="contenttype-associatewithhubsites"></a>contentType：associateWithHubSites

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
将 [内容类型][contentType] 与中心网站列表关联。

>**注意：** 此功能仅限于拥有 SharePoint Syntex 许可证的租户。
  

## <a name="permissions"></a>Permissions  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------
|委派（工作或学校帐户） | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/id/contentTypes/id/associateWithHubSites
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
|hubSiteUrls| 集合 (字符串)  |需要强制执行内容类型的中心网站的主要 URL 列表。 必需。|
|propagateToExistingLists| 布尔 |如果 ，内容类型将在中心网站中的现有列表上强制执行;否则，它将仅应用于 `true` 新创建的列表。 

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="example"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "contenttype_associatewithhubsites"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/id/contentTypes/id/associateWithHubSites
Content-Type: application/json

{
  "hubSiteUrls":
    [
      "https://graph.microsoft.com/beta/sites/id"
      
    ],
    "propagateToExistingLists": false
}
```



### <a name="response"></a>响应


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content

```

  

[contentType]: ../resources/contentType.md
