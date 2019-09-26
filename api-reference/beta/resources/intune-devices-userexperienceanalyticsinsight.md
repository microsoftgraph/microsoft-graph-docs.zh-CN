---
title: userExperienceAnalyticsInsight 资源类型
description: 用户体验分析见解是改进用户体验分析分数的建议。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70cb1e7405fdffcff0f1fd6a8a8361df6d941788
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196698"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a>userExperienceAnalyticsInsight 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户体验分析见解是改进用户体验分析分数的建议。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|userExperienceAnalyticsMetricId|String|用户体验分析洞察力的唯一标识符。|
|insightId|String|用户体验分析洞察力的唯一标识符。|
|values|[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)集合|用户体验分析洞察力的价值。|
|severity|[userExperienceAnalyticsInsightSeverity](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|用户体验分析洞察力的价值。 可取值为：`none`、`informational`、`warning`、`error`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
  "userExperienceAnalyticsMetricId": "String",
  "insightId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble",
      "value": "<Unknown Primitive Type Edm.Double>"
    }
  ],
  "severity": "String"
}
```



