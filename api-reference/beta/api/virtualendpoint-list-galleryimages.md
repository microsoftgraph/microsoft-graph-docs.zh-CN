---
title: List galleryImages
description: 列出组织库图像的属性和关系。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 1d2288844b6823e3690cab3016b760950842c6c4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031316"
---
# <a name="list-galleryimages"></a>List galleryImages

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

列出 [cloudPcGalleryImage 对象的属性和](../resources/cloudpcgalleryimage.md) 关系。

## <a name="permissions"></a>Permissions

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
GET /deviceManagement/virtualEndpoint/galleryImages
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$select` `$filter` 和 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcGalleryImage](../resources/cloudpcgalleryimage.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcgalleryimage"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/galleryImages
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcgalleryimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcgalleryimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcgalleryimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcgalleryimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-cloudpcgalleryimage-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcGalleryImage",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cloudPcGalleryImage",
    "value": [
        {
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
        },
        {
            "id":"MicrosoftWindowsDesktop_windows-ent-cpc_20h1-ent-cpc-os",
            "displayName":"Windows 10 Enterprise + OS Optimizations 2004",
            "offerDisplayName":"Windows 10 Enterprise + OS Optimizations",
            "skuDisplayName":"2004",
            "publisher":"MicrosoftWindowsDesktop",
            "offer":"windows-ent-cpc",
            "sku":"20h1-ent-cpc-os",
            "recommendedSku":"light",
            "status":"supported",
            "sizeInGB":64,
            "startDate":"2020-05-27",
            "endDate":"2021-12-14",
            "expiredDate":"2022-06-14"
        }
   ]
}
```
