---
title: managedDevice：bulkReprovisionCloudPc
description: 使用Intune托管设备 ID 批量重新预配一组云电脑设备。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: c7ba4082db38a8f2ac4f1c72f0acbc84fa6c95fa
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628872"
---
# <a name="manageddevice-bulkreprovisioncloudpc"></a>managedDevice：bulkReprovisionCloudPc

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用Intune托[管设备](../resources/cloudpc.md) ID 批量重新预配一组云电脑设备。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/managedDevices/bulkReprovisionCloudPc
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供Intune托管设备的 ID 的 JSON 表示形式。

下表显示了批量重新预配一组云电脑设备时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|managedDeviceIds|集合（字符串）|云电脑设备的 ID。|

## <a name="response"></a>响应

如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managedDevice_bulkReprovisionCloudPc"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/bulkReprovisionCloudPc
Content-Type: application/json

{
  managedDeviceIds: ["30d0e128-de93-41dc-89ec-33d84bb662a0", "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"] 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/manageddevice-bulkreprovisioncloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/manageddevice-bulkreprovisioncloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/manageddevice-bulkreprovisioncloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/manageddevice-bulkreprovisioncloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/manageddevice-bulkreprovisioncloudpc-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult",
    "successfulDeviceIds": [
        "30d0e128-de93-41dc-89ec-33d84bb662a0"
    ],
    "failedDeviceIds": [
        "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
    ],
    "notFoundDeviceIds": [
    ],
    "notSupportedDeviceIds": [
    ]
  }
}
```
