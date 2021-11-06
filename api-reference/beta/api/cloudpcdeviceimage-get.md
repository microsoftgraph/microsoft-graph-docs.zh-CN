---
title: 获取 cloudPcDeviceImage
description: 读取 cloudPcDeviceImage 对象的属性和关系。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: fbf1ddda44812bd75b481fe86e62d9ad23d8ddf1
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805412"
---
# <a name="get-cloudpcdeviceimage"></a>获取 cloudPcDeviceImage

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取特定 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。

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
GET /deviceManagement/virtualEndpoint/deviceImages/{id}
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

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdeviceimage"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcdeviceimage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcdeviceimage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcdeviceimage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcdeviceimage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcDeviceImage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
    "id": "eda7ed64-7705-4079-9d08-c2bd883f4fff",
    "displayName": "Display Name value",
    "osBuildNumber": "OS Build Number value",
    "operatingSystem": "Operating System value",
    "version": "Version value",
    "sourceImageResourceId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage",
    "lastModifiedDateTime": "2020-11-03T07:03:44.97Z",
    "status": "pending",
    "statusDetails": null
}
```
