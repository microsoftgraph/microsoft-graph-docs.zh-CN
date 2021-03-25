---
title: createDeviceLogCollectionRequest 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb303df2b0590d1986b7853992a2c2aa2c741573
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150113"
---
# <a name="createdevicelogcollectionrequest-action"></a>createDeviceLogCollectionRequest 操作

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/comanagedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|属性|类型|说明|
|:---|:---|:---|
|templateType|[deviceLogCollectionRequest](../resources/intune-devices-devicelogcollectionrequest.md)|尚未记录|



## <a name="response"></a>响应
如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [deviceLogCollectionResponse。](../resources/intune-devices-devicelogcollectionresponse.md)

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/createDeviceLogCollectionRequest

Content-type: application/json
Content-length: 153

{
  "templateType": {
    "@odata.type": "microsoft.graph.deviceLogCollectionRequest",
    "id": "Id value",
    "templateType": "predefined"
  }
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
    "id": "05fb97dc-97dc-05fb-dc97-fb05dc97fb05",
    "status": "Status value",
    "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
    "errorCode": 9,
    "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
    "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
    "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
    "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
    "size": 1.3333333333333333
  }
}
```




