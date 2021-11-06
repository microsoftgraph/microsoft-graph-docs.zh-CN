---
title: 获取 cloudPcGalleryImage
description: 读取 cloudPcGalleryImage 对象的属性和关系。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c1aafdfca8ecfbc9b067a63c16324f6eb791b708
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805555"
---
# <a name="get-cloudpcgalleryimage"></a>获取 cloudPcGalleryImage

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取特定 [cloudPcGalleryImage 对象的属性和](../resources/cloudpcgalleryimage.md) 关系。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.Read.All、CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CloudPC.Read.All、CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/galleryImages/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$select` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_cloudpcgalleryimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/galleryImages/{id}
```

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcGalleryImage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#cloudPcGalleryImage",
  "id":"MicrosoftWindowsDesktop_windows-ent-cpc_19h2-ent-cpc-os",
  "displayName":"Windows 10 Enterprise + OS Optimizations 1909",
  "offerDisplayName":"Windows 10 Enterprise + OS Optimizations",
  "skuDisplayName":"1909",
  "publisher":"MicrosoftWindowsDesktop",
  "offer":"windows-ent-cpc",
  "sku":"19h2-ent-cpc-os",
  "recommendedSku":"light",
  "status":"supported",
  "sizeInGB":64,
  "startDate":"2019-11-12",
  "endDate":"2022-05-10",
  "expiredDate":"2022-11-10"
}

```
