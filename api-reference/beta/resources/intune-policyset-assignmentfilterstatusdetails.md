---
title: assignmentFilterStatusDetails 资源类型
description: 表示设备和有效负载以及所有关联的已应用筛选器的状态详细信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be36fae74e412395bd74a24b11b36b48cbf165ff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155972"
---
# <a name="assignmentfilterstatusdetails-resource-type"></a>assignmentFilterStatusDetails 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设备和有效负载以及所有关联的已应用筛选器的状态详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|managedDeviceId|String|设备对象的唯一标识符。|
|payloadId|String|有效负载对象的唯一标识符。|
|userId|String|UserId 对象的唯一标识符。 可以是 null|
|deviceProperties|[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合|在设备签入期间用于筛选器评估的设备属性。|
|evalutionSummaries|[assignmentFilterEvaluationSummary](../resources/intune-policyset-assignmentfilterevaluationsummary.md) 集合|与设备和负载关联的每个筛选器的评估结果摘要|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterStatusDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterStatusDetails",
  "managedDeviceId": "String",
  "payloadId": "String",
  "userId": "String",
  "deviceProperties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "evalutionSummaries": [
    {
      "@odata.type": "microsoft.graph.assignmentFilterEvaluationSummary",
      "assignmentFilterId": "String",
      "assignmentFilterLastModifiedDateTime": "String (timestamp)",
      "assignmentFilterDisplayName": "String",
      "assignmentFilterPlatform": "String",
      "evaluationResult": "String",
      "evaluationDateTime": "String (timestamp)",
      "assignmentFilterType": "String",
      "assignmentFilterTypeAndEvaluationResults": [
        {
          "@odata.type": "microsoft.graph.assignmentFilterTypeAndEvaluationResult",
          "assignmentFilterType": "String",
          "evaluationResult": "String"
        }
      ]
    }
  ]
}
```




