---
title: 更新 userExperienceAnalyticsBatteryHealthDevicePerformance
description: 更新 userExperienceAnalyticsBatteryHealthDevicePerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cebca01e4512eeed9759f73b602dcdc894b62644
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689235"
---
# <a name="update-userexperienceanalyticsbatteryhealthdeviceperformance"></a>更新 userExperienceAnalyticsBatteryHealthDevicePerformance

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsBatteryHealthDevicePerformance 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) 的属性。

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
PATCH /deviceManagement/userExperienceAnalyticsBatteryHealthDevicePerformance/{userExperienceAnalyticsBatteryHealthDevicePerformanceId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsBatteryHealthDevicePerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|用户体验分析电池运行状况设备性能对象的唯一标识符。|
|deviceId|String|设备的唯一标识符 Intune DeviceID。|
|deviceName|String|设备友好名称。|
|model|String|设备的型号名称。|
|maxCapacityPercentage|Int32|具有最低容量的电池的当前容量和设计容量的比率。 百分比单位，值范围为 0-100。 有效值 -2147483648 2147483647|
|estimatedRuntimeInMinutes|Int32|电池完全充电时设备的预计运行时。 单位（以分钟表示）。 有效值 -2147483648 2147483647|
|batteryAgeInDays|Int32|估计电池使用时间。 单位（以天表示）。 有效值 -2147483648 2147483647|
|deviceBatteryHealthScore|Int32|设备最大容量分数和运行时估计分数的加权平均值。 值范围为 0-100。 有效值 -2147483648 2147483647|
|healthStatus|字符串|设备的整体电池运行状况状态。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthDevicePerformance/{userExperienceAnalyticsBatteryHealthDevicePerformanceId}
Content-type: application/json
Content-length: 362

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "maxCapacityPercentage": 5,
  "estimatedRuntimeInMinutes": 9,
  "batteryAgeInDays": 0,
  "deviceBatteryHealthScore": 8,
  "healthStatus": "Health Status value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 411

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "id": "c8b9e0fd-e0fd-c8b9-fde0-b9c8fde0b9c8",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "maxCapacityPercentage": 5,
  "estimatedRuntimeInMinutes": 9,
  "batteryAgeInDays": 0,
  "deviceBatteryHealthScore": 8,
  "healthStatus": "Health Status value"
}
```



