---
title: userExperienceAnalyticsDevicePerformance 资源类型
description: 用户体验分析设备性能实体包含设备启动性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 763e123689a0ea7149f164dd8a79341664bb20a3
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264820"
---
# <a name="userexperienceanalyticsdeviceperformance-resource-type"></a>userExperienceAnalyticsDevicePerformance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析设备性能实体包含设备启动性能详细信息。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDevicePerformances](../api/intune-devices-userexperienceanalyticsdeviceperformance-list.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 集合|列出 [userExperienceAnalyticsDevicePerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 关系。|
|[获取 userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-get.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|读取 [userExperienceAnalyticsDevicePerformance 对象的属性和](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 关系。|
|[创建 userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-create.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|创建新的 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象。|
|[删除 userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-delete.md)|无|删除 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)。|
|[更新 userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-update.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|更新 [userExperienceAnalyticsDevicePerformance 对象](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 的属性。|
|[summarizeDevicePerformanceDevices 函数](../api/intune-devices-userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析设备启动性能设备的唯一标识符。|
|deviceName|String|用户体验分析设备名称。|
|model|String|用户体验分析设备模型。|
|manufacturer|String|用户体验分析设备制造商。|
|diskType|[diskType](../resources/intune-devices-disktype.md)|用户体验分析设备磁盘类型。 可取值为：`unkown`、`hdd`、`ssd`。|
|operatingSystemVersion|String|用户体验分析设备操作系统版本。|
|bootScore|Int32|用户体验分析设备启动分数。|
|coreBootTimeInMs|Int32|用户体验分析设备核心启动时间（以毫秒为单位）。|
|groupPolicyBootTimeInMs|Int32|用户体验分析设备组策略启动时间（以毫秒为单位）。|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析设备的运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|loginScore|Int32|用户体验分析设备登录分数。|
|coreLoginTimeInMs|Int32|用户体验分析设备核心登录时间（以毫秒为单位）。|
|groupPolicyLoginTimeInMs|Int32|用户体验分析设备组策略登录时间（以毫秒为单位）。|
|deviceCount|Int64|用户体验分析汇总了设备计数。|
|responsiveDesktopTimeInMs|Int32|用户体验分析响应式桌面时间（以毫秒为单位）。|
|blueScreenCount|Int32|最近 14 天内的蓝屏数。 有效值为 0 到 9999999|
|restartCount|Int32|最近 14 天内的重启次数。 有效值为 0 到 9999999|
|averageBlueScreens|双精度|平均 (平均) 14 天内每个设备的蓝屏数量。 有效值为 0 到 9999999|
|averageRestarts|双精度|平均 (，) 最近 14 天内每个设备重新启动次数的平均值。 有效值为 0 到 9999999|
|startupPerformanceScore|双精度|用户体验分析设备启动性能分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDevicePerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "String (identifier)",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "diskType": "String",
  "operatingSystemVersion": "String",
  "bootScore": 1024,
  "coreBootTimeInMs": 1024,
  "groupPolicyBootTimeInMs": 1024,
  "healthStatus": "String",
  "loginScore": 1024,
  "coreLoginTimeInMs": 1024,
  "groupPolicyLoginTimeInMs": 1024,
  "deviceCount": 1024,
  "responsiveDesktopTimeInMs": 1024,
  "blueScreenCount": 1024,
  "restartCount": 1024,
  "averageBlueScreens": "4.2",
  "averageRestarts": "4.2",
  "startupPerformanceScore": "4.2"
}
```




