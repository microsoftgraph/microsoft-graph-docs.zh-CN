---
title: purgeDataOperation 资源类型
description: 表示用于永久删除 sourceCollection 中数据的操作。 目前，该操作的范围是Microsoft Teams邮件。
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 5562658c40831cea39922dfd5d1e1edc1d214392
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608409"
---
# <a name="purgedataoperation-resource-type"></a>purgeDataOperation 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于永久删除 sourceCollection 中数据的操作。 此操作当前的范围是Microsoft Teams消息;将来将有更多的数据源位于范围内。

继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| 操作表示的操作类型。 可能的值包括：`addToReviewSet`、`applyTags`、`contentExport`、`convertToPdf``estimateStatistics`、`purgeData`。|
|completedDateTime|DateTimeOffset| 操作完成的日期和时间。 |
|createdBy|[identitySet](../resources/identityset.md)| 创建操作的用户。 |
|createdDateTime|DateTimeOffset| 创建该操作的日期和时间。 |
|id|String| 操作 ID。 只读。 |
|percentProgress|Int32| 操作的进度。 |
|resultInfo|[resultInfo](../resources/resultinfo.md)| 包含特定于成功和失败的结果信息。 |
|状态|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| 案例操作的状态。 可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.purgeDataOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.purgeDataOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```
