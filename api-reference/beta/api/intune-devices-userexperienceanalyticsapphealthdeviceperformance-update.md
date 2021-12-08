---
title: 更新 userExperienceAnalyticsAppHealthDevicePerformance
description: 更新 userExperienceAnalyticsAppHealthDevicePerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b502d1432225b670613aa9b9d2d86dcd36f0a26
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347653"
---
# <a name="update-userexperienceanalyticsapphealthdeviceperformance"></a>更新 userExperienceAnalyticsAppHealthDevicePerformance

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsAppHealthDevicePerformance 对象](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 的属性。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsAppHealthDevicePerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析设备性能对象的唯一标识符。|
|deviceModel|String|设备的型号名称。|
|deviceManufacturer|String|设备的制造商名称。|
|appCrashCount|Int32|设备的应用崩溃数。 有效值 -2147483648 to 2147483647|
|crashedAppCount|Int32|设备不同应用崩溃的数量。 有效值 -2147483648 to 2147483647|
|appHangCount|Int32|设备的应用挂起数。 有效值 -2147483648 to 2147483647|
|processedDateTime|DateTimeOffset|上次计算统计信息的日期和时间。|
|meanTimeToFailureInMinutes|Int32|设备失败平均时间（分钟）。 有效值 -2147483648 to 2147483647|
|deviceAppHealthScore|双精度|设备的应用运行状况分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|deviceAppHealthStatus|String|设备的整体应用运行状况状态。|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析设备的运行状况。 可能的值是：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|deviceId|String|设备的 ID。|
|deviceDisplayName|String|设备的名称。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformance/{userExperienceAnalyticsAppHealthDevicePerformanceId}
Content-type: application/json
Content-length: 590

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "processedDateTime": "2017-01-01T00:03:22.2339319-08:00",
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "healthStatus": "insufficientData",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "2c651499-1499-2c65-9914-652c9914652c",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "appCrashCount": 13,
  "crashedAppCount": 15,
  "appHangCount": 12,
  "processedDateTime": "2017-01-01T00:03:22.2339319-08:00",
  "meanTimeToFailureInMinutes": 10,
  "deviceAppHealthScore": 6.666666666666667,
  "deviceAppHealthStatus": "Device App Health Status value",
  "healthStatus": "insufficientData",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




