---
title: userExperienceAnalyticsBatteryHealthOsPerformance 资源类型
description: 用户体验分析电池运行状况操作系统性能实体包含组织中所有操作系统版本的电池相关信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f0cbc451fb10d12672b60555a08a56803f010a5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697244"
---
# <a name="userexperienceanalyticsbatteryhealthosperformance-resource-type"></a>userExperienceAnalyticsBatteryHealthOsPerformance 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析电池运行状况操作系统性能实体包含组织中所有操作系统版本的电池相关信息。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBatteryHealthOsPerformances](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-list.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) 集合|列出 [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-get.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|读取 [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-create.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|创建新的 [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) 对象。|
|[删除 userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-delete.md)|无|删除 [userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)。|
|[更新 userExperienceAnalyticsBatteryHealthOsPerformance](../api/intune-devices-userexperienceanalyticsbatteryhealthosperformance-update.md)|[userExperienceAnalyticsBatteryHealthOsPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md)|更新 [userExperienceAnalyticsBatteryHealthOsPerformance 对象](../resources/intune-devices-userexperienceanalyticsbatteryhealthosperformance.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析电池运行状况操作系统性能对象的唯一标识符。|
|activeDevices|Int32|该操作系统版本的活动设备数。 有效值 -2147483648 2147483647|
|osVersion|String|操作系统的版本。|
|osBuildNumber|String|操作系统的生成号。|
|averageMaxCapacityPercentage|Int32|运行特定操作系统版本的所有设备的最大容量的平均值。 最大容量用于测量设备电池的完全充电容量与设计容量。 有效值 -2147483648 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|对于运行特定操作系统版本的所有设备，估计运行时的全费平均值。 单位（以分钟表示）。 有效值 -2147483648 2147483647|
|averageBatteryAgeInDays|Int32|在租户中运行特定操作系统版本的所有设备的电池使用时间平均值。 单位（以天表示）。 有效值 -2147483648 2147483647|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthOsPerformance",
  "id": "String (identifier)",
  "activeDevices": 1024,
  "osVersion": "String",
  "osBuildNumber": "String",
  "averageMaxCapacityPercentage": 1024,
  "averageEstimatedRuntimeInMinutes": 1024,
  "averageBatteryAgeInDays": 1024
}
```



