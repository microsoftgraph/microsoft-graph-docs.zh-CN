---
title: addToReviewSetOperation 资源类型
description: 将 sourceCollection 的结果添加到 reviewSet
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d7323fbd6d2d068888d556328fc3ea4e399ab2fe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446674"
---
# <a name="addtoreviewsetoperation-resource-type"></a>addToReviewSetOperation 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示将 [sourceCollection](../resources/ediscovery-sourcecollection.md) 添加到 [reviewSet 的操作](../resources/ediscovery-reviewset.md)。

继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。

## <a name="methods"></a>Methods

无。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|action|[microsoft.graph.ediscovery.caseAction](../resources/ediscovery-caseoperation.md#caseaction-values)| 此实体的大小写操作将始终为 `addToReviewSet` 。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|completedDateTime|DateTimeOffset|操作完成的日期和时间。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdBy|[identitySet](../resources/identityset.md)|创建操作的用户。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)|
|createdDateTime|DateTimeOffset|操作开始的日期和时间。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)|
|id|String| 操作 ID。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|percentProgress|Int32|操作的进度。 只读。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|resultInfo|[resultInfo](../resources/resultinfo.md)|包含特定于成功和失败的结果信息。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。|
|status|[microsoft.graph.ediscovery.caseOperationStatus](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|案例操作的状态。 继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。 可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。|

### <a name="datacollectionscope-values"></a>dataCollectionScope 值

|成员|说明|
|:----|-----------|
|allVersions|包含网站中文件的所有版本。|
|linkedFiles|将 **云附件** 与电子邮件一起包括在集合中。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|reviewSet|[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)| 与源集合查询匹配的项添加到的审阅集。 |
|sourceCollection|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourceCollection.md)| 正在从中添加项目的 sourceCollection。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.addToReviewSetOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
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
