---
title: userExperienceAnalyticsBaseline 资源类型
description: User experience analytics 基线实体包含比较用户体验分析得分所依据的基线值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2103470ec8321ca1750e7dac47b3d885f8939aba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080941"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>userExperienceAnalyticsBaseline 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics 基线实体包含比较用户体验分析得分所依据的基线值。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBaselines](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 集合|列出 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|读取 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|创建新的 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象。|
|[删除 userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|无|删除 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)。|
|[更新 userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|更新 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|User experience analytics 比较基准的唯一标识符。|
|displayName|字符串|User experience analytics 基线的名称。|
|overallScore|Int32|用户体验分析基准的总体分数。|
|isBuiltIn|Boolean|指示当前基线是商业中间基线还是自定义基线。|
|createdDateTime|DateTimeOffset|自定义基线的创建日期。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|User experience analytics 设备启动性能指标。|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|用户体验分析最佳实践指标。|
|rebootAnalyticsMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|用户体验分析重新启动分析指标。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
  "isBuiltIn": true,
  "createdDateTime": "String (timestamp)"
}
```






