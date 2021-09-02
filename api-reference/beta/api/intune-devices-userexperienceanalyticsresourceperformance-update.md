---
title: 更新 userExperienceAnalyticsResourcePerformance
description: 更新 userExperienceAnalyticsResourcePerformance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac54b87e36d0d39f0f744c85ef5102e561161511
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784595"
---
# <a name="update-userexperienceanalyticsresourceperformance"></a>更新 userExperienceAnalyticsResourcePerformance

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 [userExperienceAnalyticsResourcePerformance 对象](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 的属性。

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
PATCH /deviceManagement/userExperienceAnalyticsResourcePerformance/{userExperienceAnalyticsResourcePerformanceId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象的 JSON 表示形式。

下表显示创建 [userExperienceAnalyticsResourcePerformance 时所需的属性](../resources/intune-devices-userexperienceanalyticsresourceperformance.md)。

|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析资源性能实体的唯一标识符。|
|deviceId|String|设备的 ID。|
|deviceName|String|设备的名称。|
|model|String|用户体验分析设备模型。|
|deviceCount|Int64|用户体验分析汇总了设备计数。|
|manufacturer|String|用户体验分析设备制造商。|
|cpuSpikeTimePercentage|双精度|CPU 峰值时间（以百分比表示）。 有效值为 0 至 100|
|ramSpikeTimePercentage|双精度|以百分比表示的 RAM 峰值时间。 有效值为 0 至 100|
|cpuSpikeTimeScore|Int32|用户体验分析设备 CPU 峰值时间分数。 有效值为 0 至 100|
|cpuSpikeTimePercentageThreshold|双精度|cpuSpikeTimeScore 的阈值。 有效值为 0 至 100|
|ramSpikeTimeScore|Int32|用户体验分析设备 RAM 峰值时间分数。 有效值为 0 至 100|
|ramSpikeTimePercentageThreshold|双精度|ramSpikeTimeScore 的阈值。 有效值为 0 至 100|
|deviceResourcePerformanceScore|Int32|特定设备的资源性能分数。 有效值为 0 至 100|
|averageSpikeTimeScore|Int32|设备或型号类型的 AverageSpikeTimeScore。 有效值为 0 至 100|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance/{userExperienceAnalyticsResourcePerformanceId}
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14,
  "averageSpikeTimeScore": 5
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 633

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
  "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "model": "Model value",
  "deviceCount": 11,
  "manufacturer": "Manufacturer value",
  "cpuSpikeTimePercentage": 7.333333333333333,
  "ramSpikeTimePercentage": 7.333333333333333,
  "cpuSpikeTimeScore": 1,
  "cpuSpikeTimePercentageThreshold": 10.333333333333334,
  "ramSpikeTimeScore": 1,
  "ramSpikeTimePercentageThreshold": 10.333333333333334,
  "deviceResourcePerformanceScore": 14,
  "averageSpikeTimeScore": 5
}
```



