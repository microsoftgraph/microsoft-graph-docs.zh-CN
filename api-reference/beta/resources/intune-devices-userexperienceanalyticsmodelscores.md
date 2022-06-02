---
title: userExperienceAnalyticsModelScores 资源类型
description: 用户体验分析模型评分实体合并了各种终结点分析分数。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbf00cd94e9667ac556535b5d8dca75e2a76800a
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857867"
---
# <a name="userexperienceanalyticsmodelscores-resource-type"></a>userExperienceAnalyticsModelScores 资源类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析模型评分实体合并了各种终结点分析分数。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsModelScoreses](../api/intune-devices-userexperienceanalyticsmodelscores-list.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 集合|列出 [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-get.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|读取 [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-create.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|创建新的 [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 对象。|
|[删除 userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-delete.md)|None|删除 [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)。|
|[更新 userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-update.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|更新 [userExperienceAnalyticsModelScores 对象的](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析模型评分对象的唯一标识符。|
|model|String|用户体验分析模型评分的唯一标识符：设备模型。|
|manufacturer|String|用户体验分析模型评分的唯一标识符：设备制造商。|
|modelDeviceCount|Int64|用户体验分析模型设备计数。 有效值 -9.22337203685478E+18 到 9.22337203685478E+18|
|endpointAnalyticsScore|双精度|用户体验分析模型分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|startupPerformanceScore|双精度|用户体验分析模型启动性能分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|appReliabilityScore|双精度|用户体验分析模型应用可靠性分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|workFromAnywhereScore|双精度|用户体验分析模型可从任何位置进行评分。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|batteryHealthScore|双精度|用户体验分析模型电池运行状况分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析模型的运行状况状态。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsModelScores"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsModelScores",
  "id": "String (identifier)",
  "model": "String",
  "manufacturer": "String",
  "modelDeviceCount": 1024,
  "endpointAnalyticsScore": "4.2",
  "startupPerformanceScore": "4.2",
  "appReliabilityScore": "4.2",
  "workFromAnywhereScore": "4.2",
  "batteryHealthScore": "4.2",
  "healthStatus": "String"
}
```




