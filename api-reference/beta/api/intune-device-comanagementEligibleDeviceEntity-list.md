---
title: 列出 comanagementEligibleDeviceEntity
description: 列出 comanagementEligibleDeviceEntity 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39d7a92c5914107cdd5ecfebb9b4b7948bc8b8b0
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636089"
---
# <a name="list-comanagementeligibledeviceentity"></a>列出 comanagementEligibleDeviceEntity

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 comanagementEligibleDeviceEntity 对象的属性和关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleReports
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应`200 OK`正文中返回响应代码和 comanagementEligibleDeviceEntity 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleReports
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
      "id": "659554f2-54f2-6595-f254-9565f2549565",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "deviceType": "Device Type value",
      "clientRegistrationStatus": "Client Registration Status value",
      "ownerType": "Owner Type value",
      "managementAgents": "Management Agent value",
      "managementState": "Management State value",
      "referenceId": "Reference Id value",
      "mdmStatus": "MDM Status value",
      "osVersion": "OS Version value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacture value",
      "model": "Model value",
      "osDescription": "OS Description value",
      "entitySource": 1024,
      "userId": "User Id value",
      "upn": "UPN value",
      "userEmail": "User Email value",
      "userName": "User name value",
      "coManageEligibleStatus": "CO Manage Eligible Status value"
    }
  ]
}
```



