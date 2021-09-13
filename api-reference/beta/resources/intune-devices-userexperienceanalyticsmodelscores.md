---
title: userExperienceAnalyticsModelScores 资源类型
description: 用户体验分析模型分数实体合并了各种终结点分析分数。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a29726d69cca6330de93af4793862a76e6fc9ce2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064061"
---
# <a name="userexperienceanalyticsmodelscores-resource-type"></a>userExperienceAnalyticsModelScores 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析模型分数实体合并了各种终结点分析分数。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsModelScoreses](../api/intune-devices-userexperienceanalyticsmodelscores-list.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 集合|列出 [userExperienceAnalyticsModelScores 对象的属性和](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 关系。|
|[获取 userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-get.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|读取 [userExperienceAnalyticsModelScores 对象的属性和](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 关系。|
|[创建 userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-create.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|创建新的 [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 对象。|
|[删除 userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-delete.md)|无|删除 [userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)。|
|[更新 userExperienceAnalyticsModelScores](../api/intune-devices-userexperienceanalyticsmodelscores-update.md)|[userExperienceAnalyticsModelScores](../resources/intune-devices-userexperienceanalyticsmodelscores.md)|更新 [userExperienceAnalyticsModelScores 对象](../resources/intune-devices-userexperienceanalyticsmodelscores.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析模型评分对象的唯一标识符。|
|model|String|用户体验分析模型分数的唯一标识符：设备模型。|
|manufacturer|String|用户体验分析模型分数的唯一标识符：设备制造商。|
|modelDeviceCount|Int64|用户体验分析模型设备计数。 有效值 -9.22337203685478E+18 到 9.22337203685478E+18|
|endpointAnalyticsScore|双精度|用户体验分析模型分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|startupPerformanceScore|双精度|用户体验分析模型启动性能分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|appReliabilityScore|双精度|用户体验分析模型应用可靠性分数。 有效值 -1.79769313486232E+308 到 1.79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|用户体验分析模型的运行状况。 可取值为：`unknown`、`insufficientData`、`needsAttention`、`meetingGoals`。|

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
  "healthStatus": "String"
}
```



