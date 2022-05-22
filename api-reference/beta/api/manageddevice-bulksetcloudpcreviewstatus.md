---
title: managedDevice：bulkSetCloudPcReviewStatus
description: 使用包含Intune托管设备 ID 的单个请求设置多个云电脑设备的审阅状态。
author: yayang3
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: bd1d5d27581f1752ef0d2064810514d98be53420
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629495"
---
# <a name="manageddevice-bulksetcloudpcreviewstatus"></a>managedDevice：bulkSetCloudPcReviewStatus

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用包含Intune托管设备 ID 的单个请求设置多个云电脑设备的审阅状态。

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
POST /deviceManagement/managedDevices/bulkSetCloudPcReviewStatus
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|Description|
|:---|:---|:---|
|managedDeviceIds|字符串集合|云电脑设备的托管设备 ID。|
|reviewStatus|[cloudPcReviewStatus](../resources/cloudpcreviewstatus.md)|云电脑设备的新审阅状态。 |


## <a name="response"></a>响应

如果成功，此操作在响应正文中返回 `200 OK` 响应代码和 [cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "manageddevicethis.bulksetcloudpcreviewstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/bulkSetCloudPcReviewStatus
Content-Type: application/json

{
  "managedDeviceIds": [
    "30d0e128-de93-41dc-89ec-33d84bb662a0",
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
  ],
  "reviewStatus": {
    "inReview": true,
    "userAccessLevel": "restricted",
    "azureStorageAccountId": "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
  }
}
```


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult",
  "name": "manageddevicethis.bulksetcloudpcreviewstatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult",
  "successfulDeviceIds": [
    "30d0e128-de93-41dc-89ec-33d84bb662a0"
  ],
  "failedDeviceIds": [
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
  ],
  "notFoundDeviceIds": [],
  "notSupportedDeviceIds": []
}
```

