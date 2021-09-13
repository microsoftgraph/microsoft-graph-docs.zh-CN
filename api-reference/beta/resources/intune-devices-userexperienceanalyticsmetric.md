---
title: userExperienceAnalyticsMetric 资源类型
description: 用户体验分析指标包含用户体验分析类别指标的分数和单位。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 352a89293bb38e7f03bd7e83d003d465d052335b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125699"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>userExperienceAnalyticsMetric 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析指标包含用户体验分析类别指标的分数和单位。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsMetrics](../api/intune-devices-userexperienceanalyticsmetric-list.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 集合|列出 [userExperienceAnalyticsMetric 对象的属性和](../resources/intune-devices-userexperienceanalyticsmetric.md) 关系。|
|[获取 userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|读取 [userExperienceAnalyticsMetric 对象的属性和](../resources/intune-devices-userexperienceanalyticsmetric.md) 关系。|
|[创建 userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|创建新的 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) 对象。|
|[删除 userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|无|删除 [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)。|
|[更新 userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|更新 [userExperienceAnalyticsMetric 对象](../resources/intune-devices-userexperienceanalyticsmetric.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析指标的唯一标识符。|
|值|双精度|用户体验分析指标的值。|
|unit|String|用户体验分析指标的单位。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "String (identifier)",
  "value": "4.2",
  "unit": "String"
}
```



