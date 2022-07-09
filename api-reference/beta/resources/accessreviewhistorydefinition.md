---
title: accessReviewHistoryDefinition 资源类型
description: 表示访问评审历史记录数据的集合。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 935f27083f2c2f49d92079cad02aa1174d1cb68f
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697244"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>accessReviewHistoryDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示访问评审历史数据的集合以及用于收集该数据的范围。

**accessReviewHistoryDefinition** 包含 [accessReviewHistoryInstance](accessReviewHistoryInstance.md) 对象的列表。 历史记录定义的每次重复都会创建一个实例。 对于一次性历史记录定义，只创建一个实例。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewHistoryDefinitions](../api/accessreviewset-list-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 集合|获取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象及其属性的列表。|
|[创建 accessReviewHistoryDefinition](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|创建新的 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象。|
|[获取 accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|读取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象的属性和关系。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[userIdentity](useridentity.md)| 创建此审阅历史记录定义的用户。 |
|createdDateTime|DateTimeOffset|创建访问评审定义时的时间戳。|
|决定|String collection|确定如果指定，哪些评审决定将包含在提取的审阅历史记录数据中。 创建时可选。 如果在创建时未提供任何决策，则默认情况下将包含所有决策。 可能的值为：`approve`、`deny`、`dontKnow`和 `notReviewed``notNotified`。|
|displayName|String|访问评审历史记录数据收集的名称。 必需。|
|id|String|访问评审历史记录定义的分配的唯一标识符。|
|reviewHistoryPeriodEndDateTime|DateTimeOffset| 时间戳。 在此日期或之前结束的评论将包含在提取的历史记录数据中。 仅当未定义 **scheduleSettings** 时才需要。 |
|reviewHistoryPeriodStartDateTime|DateTimeOffset|时间戳。 从此日期开始或之前的评审将包含在提取的历史记录数据中。 仅当未定义 **scheduleSettings** 时才需要。|
| scheduleSettings  |[accessReviewHistoryScheduleSettings](accessReviewHistoryScheduleSettings.md)| 定期访问评审历史记录定义系列的设置。 仅当未定义 **reviewHistoryPeriodStartDateTime** 或 **reviewHistoryPeriodEndDateTime 时** 才需要。 尚不支持。|
|scopes|[accessReviewScope](accessreviewscope.md) 集合|用于对提取的历史记录数据中包含的评论进行范围。 提取其范围与此提供的范围匹配的评审。 必填。|
|status| accessReviewHistoryStatus|表示审阅历史记录数据收集的状态。 可能的值包括 `done`、`inProgress`、`error`、`requested`、`unknownFutureValue`。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|实例|[accessReviewHistoryInstance](accessreviewhistoryinstance.md) 集合| 如果 **accessReviewHistoryDefinition** 是一个定期定义，则实例表示每个重复周期。 不重复的定义将完全有一个实例。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "status": "String",
  "decisions": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "scheduleSettings": {
    "@odata.type": "microsoft.graph.accessReviewHistoryScheduleSettings"
  }
}
```
