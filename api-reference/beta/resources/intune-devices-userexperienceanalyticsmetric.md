---
title: userExperienceAnalyticsMetric 资源类型
description: User experience analytics 指标包含 user experience anlaytics 类别的分数和度量单位。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 307e8c9430c5eb8d0d7bd6bc51bc772dacb6392b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371459"
---
# <a name="userexperienceanalyticsmetric-resource-type"></a>userExperienceAnalyticsMetric 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

User experience analytics 指标包含 user experience anlaytics 类别的分数和度量单位。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsMetrics](../api/intune-devices-userexperienceanalyticsmetric-list.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)集合|列出[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)对象的属性和关系。|
|[获取 userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|读取[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)对象的属性和关系。|
|[创建 userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-create.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|创建新的[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)对象。|
|[删除 userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-delete.md)|无|删除[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)。|
|[更新 userExperienceAnalyticsMetric](../api/intune-devices-userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|更新[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|User experience analytics 指标的唯一标识符。|
|displayName|String|User experience analytics 指标的名称。|
|值|双精度|User experience analytics 指标的值。|
|处理器|String|User experience analytics 指标的单位。|

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
  "displayName": "String",
  "value": "<Unknown Primitive Type Edm.Double>",
  "unit": "String"
}
```



