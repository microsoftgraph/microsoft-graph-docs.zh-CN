---
title: userExperienceAnalyticsMetricHistory 资源类型
description: 用户体验分析指标历史记录。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 480be2d3dfa7287b4da5c707536a95e8d8ffb316
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444474"
---
# <a name="userexperienceanalyticsmetrichistory-resource-type"></a>userExperienceAnalyticsMetricHistory 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析指标历史记录。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userExperienceAnalyticsMetricHistories](../api/intune-devices-userexperienceanalyticsmetrichistory-list.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 集合|列出 [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 对象的属性和关系。|
|[获取 userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-get.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|读取 [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 对象的属性和关系。|
|[创建 userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-create.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|创建新的 [userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 对象。|
|[删除 userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-delete.md)|无|删除用户 [ExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)。|
|[更新 userExperienceAnalyticsMetricHistory](../api/intune-devices-userexperienceanalyticsmetrichistory-update.md)|[userExperienceAnalyticsMetricHistory](../resources/intune-devices-userexperienceanalyticsmetrichistory.md)|更新 [userExperienceAnalyticsMetricHistory 对象](../resources/intune-devices-userexperienceanalyticsmetrichistory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户体验分析指标历史记录的唯一标识符。|
|deviceId|String|用户体验分析设备 ID。|
|metricDateTime|DateTimeOffset|用户体验分析指标日期时间。|
|metricType|String|用户体验分析指标类型。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|userExperienceAnalyticsMetric|[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)|用户体验分析指标。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetricHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetricHistory",
  "id": "String (identifier)",
  "deviceId": "String",
  "metricDateTime": "String (timestamp)",
  "metricType": "String"
}
```




