---
title: ediscoveryEstimateOperation 资源类型
description: 表示在电子数据展示搜索)  (项计数、大小和位置数估算统计信息的过程。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f4edad31ab7e5c1018cae4e681559d189ba8ef30
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838253"
---
# <a name="ediscoveryestimateoperation-resource-type"></a>ediscoveryEstimateOperation 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在电子数据展示搜索)  (项计数、大小和位置数估算统计信息的过程。

继承自 [caseOperation](../resources/security-caseoperation.md)。

## <a name="methods"></a>方法
无。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|microsoft.graph.security.caseAction| 操作表示的操作类型。 可能的值为：，`addToReviewSet``applyTags`，，`contentExport``convertToPdf`，`estimateStatistics`，`purgeData`|
|completedDateTime|DateTimeOffset|操作完成的日期和时间。 只读。 |
|createdBy|[identitySet](../resources/identityset.md)|创建操作的用户。 只读。 |
|createdDateTime|DateTimeOffset|操作开始的日期和时间。 只读。|
|id|String| 操作的 ID。 只读。|
|indexedItemCount|Int64|与内容查询匹配的 **搜索** 项的估计计数。|
|indexedItemsSize|Int64|与内容查询匹配的 **搜索** 项的估计大小。|
|mailboxCount|Int32|具有搜索命中次数的邮箱数。|
|percentProgress|Int32|操作的进度。 只读。 |
|resultInfo|[resultInfo](../resources/resultinfo.md)|包含成功和失败特定的结果信息。 |
|siteCount|Int32|具有搜索命中次数的邮箱数。|
|status|microsoft.graph.security.caseOperationStatus| 事例操作的状态。 可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。|
|unindexedItemCount|Int64|集合的未表达项的估计计数。|
|unindexedItemsSize|Int64|集合的未表达项的估计大小。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|search|[microsoft.graph.security.ediscoverySearch](../resources/security-ediscoverysearch.md)|电子数据展示搜索。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryEstimateOperation",
  "baseType": "microsoft.graph.security.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryEstimateOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "percentProgress": "Integer",
  "status": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "indexedItemCount": "Integer",
  "indexedItemsSize": "Integer",
  "unindexedItemCount": "Integer",
  "unindexedItemsSize": "Integer",
  "mailboxCount": "Integer",
  "siteCount": "Integer"
}
```

