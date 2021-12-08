---
title: userExperienceAnalyticsAppHealthDevicePerformance 资源类型
description: 用户体验分析设备性能实体包含设备性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97cf26e0c9885745be63a3221bb7b9fd9508c6db
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347331"
---
# <a name="userexperienceanalyticsapphealthdeviceperformance-resource-type"></a>userExperienceAnalyticsAppHealthDevicePerformance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备性能实体包含设备性能详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsAppHealthDevicePerformances](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-list.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 集合|列出 [userExperienceAnalyticsAppHealthDevicePerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 关系。|
|[获取 userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-get.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|读取 [userExperienceAnalyticsAppHealthDevicePerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 关系。|
|[创建 userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-create.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|创建新的 [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 对象。|
|[删除 userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-delete.md)|无|删除 [userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)。|
|[更新 userExperienceAnalyticsAppHealthDevicePerformance](../api/intune-devices-userexperienceanalyticsapphealthdeviceperformance-update.md)|[userExperienceAnalyticsAppHealthDevicePerformance](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md)|更新 [userExperienceAnalyticsAppHealthDevicePerformance 对象](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformance.md) 的属性。|

## <a name="properties"></a>属性
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

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformance",
  "id": "String (identifier)",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "appCrashCount": 1024,
  "crashedAppCount": 1024,
  "appHangCount": 1024,
  "processedDateTime": "String (timestamp)",
  "meanTimeToFailureInMinutes": 1024,
  "deviceAppHealthScore": "4.2",
  "deviceAppHealthStatus": "String",
  "healthStatus": "String",
  "deviceId": "String",
  "deviceDisplayName": "String"
}
```




