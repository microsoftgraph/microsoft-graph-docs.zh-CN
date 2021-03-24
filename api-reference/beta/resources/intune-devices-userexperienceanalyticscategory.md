---
title: userExperienceAnalyticsCategory 资源类型
description: 用户体验分析类别实体包含类别的各种指标的分数和见解。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f138b2417bccd6ed089810335e375eb721af80c6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141440"
---
# <a name="userexperienceanalyticscategory-resource-type"></a>userExperienceAnalyticsCategory 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析类别实体包含类别的各种指标的分数和见解。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 userExperienceAnalyticsCategory](../api/intune-devices-userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|读取 [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) 对象的属性和关系。|
|[更新 userExperienceAnalyticsCategory](../api/intune-devices-userexperienceanalyticscategory-update.md)|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|更新 [userExperienceAnalyticsCategory 对象](../resources/intune-devices-userexperienceanalyticscategory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析类别的唯一标识符。|
|overallScore|Int32|用户体验分析类别的整体分数。|
|totalDevices|Int32|用户体验分析类别的设备总数。|
|insights|[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) 集合|用户体验分析类别的见解。|
|state|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析类别的当前运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|metricValues|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 集合|用户体验分析类别的指标值。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "overallScore": 1024,
  "totalDevices": 1024,
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
  "state": "String"
}
```




