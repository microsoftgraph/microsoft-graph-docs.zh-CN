---
title: 更新 userExperienceAnalyticsAppHealthDeviceModelPerformance
description: 更新 userExperienceAnalyticsAppHealthDeviceModelPerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 43c1cca17b1718debae367a950a3e90102b355c1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202897"
---
# <a name="update-userexperienceanalyticsapphealthdevicemodelperformance"></a>更新 userExperienceAnalyticsAppHealthDeviceModelPerformance

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的属性。

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
PATCH /deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md)时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 设备模型性能对象的唯一标识符。|
|deviceModel|String|设备的模型名称。|
|deviceManufacturer|String|设备的制造商名称。|
|activeDeviceCount|Int32|模型的活动设备数。 有效值-2147483648 到2147483647|
|meanTimeToFailureInMinutes|Int32|以分钟为单位的模型设备发生故障的平均时间。 有效值-2147483648 到2147483647|
|modelAppHealthScore|双精度|设备模型的应用运行状况得分。 有效值-1.79769313486232 E + 308 到 1.79769313486232 E + 308|
|modelAppHealthStatus|String|设备模型的整体应用运行状况状态。|



## <a name="response"></a>响应
如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [userExperienceAnalyticsAppHealthDeviceModelPerformance](../resources/intune-devices-userexperienceanalyticsapphealthdevicemodelperformance.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDeviceModelPerformance/{userExperienceAnalyticsAppHealthDeviceModelPerformanceId}
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "modelAppHealthScore": 6.333333333333333,
  "modelAppHealthStatus": "Model App Health Status value"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 408

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDeviceModelPerformance",
  "id": "4daddc60-dc60-4dad-60dc-ad4d60dcad4d",
  "deviceModel": "Device Model value",
  "deviceManufacturer": "Device Manufacturer value",
  "activeDeviceCount": 1,
  "meanTimeToFailureInMinutes": 10,
  "modelAppHealthScore": 6.333333333333333,
  "modelAppHealthStatus": "Model App Health Status value"
}
```




