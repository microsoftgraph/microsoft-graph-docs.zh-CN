---
title: userExperienceAnalyticsDevicePerformance 资源类型
description: User experience analytics device performance entity 包含设备启动性能详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 817fb08cf3efeb107741c8428d721ab10e28c75c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208427"
---
# <a name="userexperienceanalyticsdeviceperformance-resource-type"></a>userExperienceAnalyticsDevicePerformance 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics device performance entity 包含设备启动性能详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsDevicePerformances](../api/intune-devices-userexperienceanalyticsdeviceperformance-list.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 集合|列出 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-get.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|读取 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-create.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|创建新的 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象。|
|[删除 userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-delete.md)|无|删除 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)。|
|[更新 userExperienceAnalyticsDevicePerformance](../api/intune-devices-userexperienceanalyticsdeviceperformance-update.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md)|更新 [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 对象的属性。|
|[summarizeDevicePerformanceDevices 函数](../api/intune-devices-userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices.md)|[userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) 集合|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 设备启动性能设备的唯一标识符。|
|deviceName|String|User experience analytics 设备名称。|
|model|String|User experience analytics 设备模型。|
|manufacturer|String|User experience analytics 设备制造商。|
|diskType|[diskType](../resources/intune-devices-disktype.md)|User experience analytics 设备磁盘类型。 可取值为：`unkown`、`hdd`、`ssd`。|
|operatingSystemVersion|String|User experience analytics 设备操作系统版本。|
|bootScore|Int32|用户体验分析设备启动得分。|
|coreBootTimeInMs|Int32|User experience analytics device core boot time （以毫秒为单位）。|
|groupPolicyBootTimeInMs|Int32|User experience analytics device group policy boot time （以毫秒为单位）。|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|User experience analytics 设备的运行状况状态。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|loginScore|Int32|用户体验分析设备登录分数。|
|coreLoginTimeInMs|Int32|User experience analytics device core login time （以毫秒为单位）。|
|groupPolicyLoginTimeInMs|Int32|User experience analytics 设备组策略登录时间（以毫秒为单位）。|
|deviceCount|Int64|用户体验分析汇总了设备计数。|
|responsiveDesktopTimeInMs|Int32|用户体验分析响应桌面时间（以毫秒为单位）。|
|blueScreenCount|Int32|过去14天中的蓝色屏幕数。 有效值为0至9999999|
|restartCount|Int32|最近14天内的重新启动次数。 有效值为0至9999999|
|averageBlueScreens|双精度|平均 (表示过去14天中每台设备的) 的蓝色屏幕数。 有效值为0至9999999|
|averageRestarts|双精度|Average (平均平均) 在最近14天内每个设备的重新启动次数。 有效值为0至9999999|

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
  "averageRestarts": "4.2"
}
```




