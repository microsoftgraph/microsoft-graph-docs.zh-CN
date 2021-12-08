---
title: userExperienceAnalyticsOverview 资源类型
description: 用户体验分析概述实体包含所有类别的总体分数以及每个指标的分数和见解。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7726b36b31be70bcfb8ed36fcd8aaa67f32924e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337194"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a>userExperienceAnalyticsOverview 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析概述实体包含所有类别的总体分数以及每个指标的分数和见解。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|读取 [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) 对象的属性和关系。|
|[更新 userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md)|更新 [userExperienceAnalyticsOverview 对象](../resources/intune-devices-userexperienceanalyticsoverview.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析概述的唯一标识符。|
|overallScore|Int32|用户体验分析总体分数。|
|deviceBootPerformanceOverallScore|Int32|用户体验分析设备启动性能总体分数。|
|bestPracticesOverallScore|Int32|用户体验分析最佳实践总体分数。|
|workFromAnywhereOverallScore|Int32|用户体验分析从任意位置工作总体分数。|
|appHealthOverallScore|Int32|用户体验分析应用运行状况总体分数。|
|resourcePerformanceOverallScore|Int32|用户体验分析资源性能总体分数。|
|batteryHealthOverallScore|Int32|用户体验分析电池运行状况总体分数。|
|insights|[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合|用户体验分析见解。|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析概述的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|deviceBootPerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"BootPerformance"类别的当前运行状况。 可能的值是：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|bestPracticesHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"BestPractices"类别的当前运行状况。 可能的值是：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|workFromAnywhereHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"WorkFromAnywhere"类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|appHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"BestPractices"类别的当前运行状况。 可能的值是：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|resourcePerformanceHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"ResourcePerformance"类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|
|batteryHealthHealthState|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析"BatteryHealth"类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": 1024,
  "deviceBootPerformanceOverallScore": 1024,
  "bestPracticesOverallScore": 1024,
  "workFromAnywhereOverallScore": 1024,
  "appHealthOverallScore": 1024,
  "resourcePerformanceOverallScore": 1024,
  "batteryHealthOverallScore": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "4.2"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String",
  "workFromAnywhereHealthState": "String",
  "appHealthState": "String",
  "resourcePerformanceHealthState": "String",
  "batteryHealthHealthState": "String"
}
```




