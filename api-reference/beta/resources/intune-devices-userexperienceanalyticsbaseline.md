---
title: userExperienceAnalyticsBaseline 资源类型
description: 用户体验分析基线实体包含比较用户体验分析分数的基线值。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3426303818afc77dd167a041a3f1af0100a86c4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141198"
---
# <a name="userexperienceanalyticsbaseline-resource-type"></a>userExperienceAnalyticsBaseline 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析基线实体包含比较用户体验分析分数的基线值。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsBaselines](../api/intune-devices-userexperienceanalyticsbaseline-list.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 集合|列出 [userExperienceAnalyticsBaseline 对象的属性和](../resources/intune-devices-userexperienceanalyticsbaseline.md) 关系。|
|[获取 userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|读取 [userExperienceAnalyticsBaseline 对象的属性和](../resources/intune-devices-userexperienceanalyticsbaseline.md) 关系。|
|[创建 userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-create.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|创建新的 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md) 对象。|
|[删除 userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-delete.md)|无|删除 [userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)。|
|[更新 userExperienceAnalyticsBaseline](../api/intune-devices-userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/intune-devices-userexperienceanalyticsbaseline.md)|更新 [userExperienceAnalyticsBaseline 对象](../resources/intune-devices-userexperienceanalyticsbaseline.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析基线的唯一标识符。|
|displayName|String|用户体验分析基线的名称。|
|overallScore|Int32|用户体验分析基线的整体分数。|
|isBuiltIn|Boolean|表示当前比较基准是商业中值基线还是自定义比较基准。|
|createdDateTime|DateTimeOffset|创建自定义比较基准的日期。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|用户体验分析设备启动性能指标。|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|用户体验分析最佳做法指标。|
|rebootAnalyticsMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|用户体验分析重新启动分析指标。|
|resourcePerformanceMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|用户体验分析资源性能指标。|
|appHealthMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|用户体验分析应用运行状况指标。|
|workFromAnywhereMetrics|[userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md)|用户体验分析从任何指标开始工作。|

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



