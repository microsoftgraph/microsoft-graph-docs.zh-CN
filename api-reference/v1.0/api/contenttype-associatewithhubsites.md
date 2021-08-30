---
author: swapnil1993
title: contentType：associateWithHubSites
description: 将内容类型与中心网站列表关联。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ae0cfe842b77b58134b127202e559711220f5aa3
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696517"
---
# <a name="contenttype-associatewithhubsites"></a>contentType：associateWithHubSites

命名空间：microsoft.graph


将内容 [类型中心][contentType] 中的已发布内容类型与中心网站列表关联。

>**注意：** 此功能仅限于拥有许可证的SharePoint Syntex租户。
  

## <a name="permissions"></a>权限  

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。

  

|权限类型 | 权限（从最低特权到最高特权） |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Sites.Manage.All、Sites.FullControl.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序 | Sites.Manage.All、Sites.FullControl.All |

  

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/associateWithHubSites
```
>**注意：**_siteId_ 表示内容类型中心网站。

## <a name="request-headers"></a>请求头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|-|-|-|
|hubSiteUrls| 集合 (字符串)  |需要强制执行内容类型的中心网站的规范 URL 列表。 此为必需属性。|
|propagateToExistingLists| 布尔值 |如果 `true` 为 ，内容类型将强制应用于中心网站中的现有列表;否则，将仅应用于新创建的列表。|

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
POST https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/{contentTypeId}/associateWithHubSites
Content-Type: application/json

{
   "hubSiteUrls":[
      "https://graph.microsoft.com/v1.0/sites/{site-id}"
   ],
   "propagateToExistingLists":false
}
```
---




### <a name="response"></a>响应


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
