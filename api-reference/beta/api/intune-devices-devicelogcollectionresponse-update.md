---
title: 更新 deviceLogCollectionResponse
description: 更新 deviceLogCollectionResponse 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e162b964f4b80ac554cc8bb283f345db6400fc2f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49219284"
---
# <a name="update-devicelogcollectionresponse"></a>更新 deviceLogCollectionResponse

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
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
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象的 JSON 表示形式。

下表显示创建 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|TenantId_deviceId_requestId 形式的唯一标识符|
|status|字符串|日志集合请求的状态|
|managedDeviceId|Guid|设备 Id|
|errorCode|Int64|错误代码（如果有）。 有效值-9.22337203685478 E + 18 to 9.22337203685478 E + 18|
|requestedDateTimeUTC|DateTimeOffset|请求的日期时间|
|receivedDateTimeUTC|DateTimeOffset|收到请求的日期/时间|
|initiatedByUserPrincipalName|字符串|为其启动请求的 UPN|
|expirationDateTimeUTC|DateTimeOffset|日志过期日期的日期/时间|
|大小|双精度|日志的大小。 有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308|



## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/logCollectionRequests/{deviceLogCollectionResponseId}
Content-type: application/json
Content-length: 479

{
  "@odata.type": "#microsoft.graph.deviceLogCollectionResponse",
  "status": "Status value",
  "managedDeviceId": "3b336f00-6f00-3b33-006f-333b006f333b",
  "errorCode": 9,
  "requestedDateTimeUTC": "2016-12-31T23:57:40.7845755-08:00",
  "receivedDateTimeUTC": "2016-12-31T23:59:48.6545758-08:00",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "expirationDateTimeUTC": "2017-01-01T00:02:49.2157996-08:00",
  "size": 1.3333333333333333
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 528

{
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
```




