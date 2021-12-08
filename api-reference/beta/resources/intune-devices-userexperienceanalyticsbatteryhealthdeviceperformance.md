---
title: userExperienceAnalyticsBatteryHealthDevicePerformance 资源类型
description: 用户体验分析电池运行状况设备性能实体包含设备级别的电池信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c30e0a20e0e37d45932733b7416ba83c288f4fbc
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336879"
---
# <a name="userexperienceanalyticsbatteryhealthdeviceperformance-resource-type"></a>userExperienceAnalyticsBatteryHealthDevicePerformance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况设备性能实体包含设备级别的电池信息。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBatteryHealthDevicePerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-list.md)|[userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) 集合|列出 [userExperienceAnalyticsBatteryHealthDevicePerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) 关系。|
|[获取 userExperienceAnalyticsBatteryHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-get.md)|[userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)|读取 [userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsBatteryHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-create.md)|[userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)|创建新的 [userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) 对象。|
|[删除 userExperienceAnalyticsBatteryHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-delete.md)|无|删除 [userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)。|
|[更新 userExperienceAnalyticsBatteryHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance-update.md)|[userExperienceAnalyticsBatteryHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md)|更新 [userExperienceAnalyticsBatteryHealthDevicePerformance 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthdeviceperformance.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况设备性能对象的唯一标识符。|
|deviceId|String|设备的唯一标识符 Intune DeviceID。|
|deviceName|String|设备友好名称。|
|model|String|设备的型号名称。|
|maxCapacityPercentage|Int32|具有最低容量的电池的当前容量和设计容量的比率。 百分比单位，值范围为 0-100。 有效值 -2147483648 to 2147483647|
|estimatedRuntimeInMinutes|Int32|电池完全充电时设备的预计运行时。 单位（以分钟表示）。 有效值 -2147483648 to 2147483647|
|batteryAgeInDays|Int32|估计电池使用时间。 单位（以天表示）。 有效值 -2147483648 to 2147483647|
|deviceBatteryHealthScore|Int32|设备最大容量分数和运行时估计分数的加权平均值。 值范围为 0-100。 有效值 -2147483648 to 2147483647|
|healthStatus|String|设备的整体电池运行状况状态。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthDevicePerformance",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "model": "String",
  "maxCapacityPercentage": 1024,
  "estimatedRuntimeInMinutes": 1024,
  "batteryAgeInDays": 1024,
  "deviceBatteryHealthScore": 1024,
  "healthStatus": "String"
}
```




