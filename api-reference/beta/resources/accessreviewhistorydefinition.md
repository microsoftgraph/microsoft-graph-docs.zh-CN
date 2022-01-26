---
title: accessReviewHistoryDefinition 资源类型
description: 表示访问评审历史记录数据的集合。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b36062da1387e50f4ffbae88a8e7cae1fa31f268
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225551"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>accessReviewHistoryDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示访问评审历史数据和用于收集数据的范围的集合。

**accessReviewHistoryDefinition** 包含 [accessReviewHistoryInstance 对象](accessReviewHistoryInstance.md)的列表。 历史记录定义的每次重复都创建一个实例。 对于一次历史记录定义，只会创建一个实例。

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
|createdDateTime|DateTimeOffset|创建访问评审定义的时间戳。|
|决策|字符串集合|确定提取的审阅历史记录数据中将包含哪些审阅决策（如果已指定）。 创建时可选。 如果未提供创建决策，则默认情况下将包含所有决策。 可能的值是 `approve` `deny` `dontKnow` ：、、、 `notReviewed` 和 `notNotified` 。|
|displayName|String|访问评审历史记录数据收集的名称。 必需。|
|id|String|为访问评审历史记录定义分配的唯一标识符。|
|reviewHistoryPeriodEndDateTime|DateTimeOffset| 时间戳。 在此日期或之前结束的审阅将包含在提取的历史记录数据中。 仅在未定义 **scheduleSettings** 时是必需的。 |
|reviewHistoryPeriodStartDateTime|DateTimeOffset|时间戳。 在此日期或之前开始审阅将包含在提取的历史记录数据中。 仅在未定义 **scheduleSettings** 时是必需的。|
| scheduleSettings  |[accessReviewHistoryScheduleSettings](accessReviewHistoryScheduleSettings.md)| 定期访问评审历史记录定义系列的设置。 仅在未定义 **reviewHistoryPeriodStartDateTime** 或 **reviewHistoryPeriodEndDateTime** 时是必需的。|
|scopes|[accessReviewScope](accessreviewscope.md) 集合|用于确定提取的历史记录数据中包含的审阅的范围。 获取其范围与提供的范围匹配的审阅。 必需。|
|状态|字符串集合|表示审阅历史记录数据收集的状态。 可能的值包括 `done`、`inProgress`、`error`、`requested`、`unknownFutureValue`。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|实例|[accessReviewHistoryInstance](accessreviewhistoryinstance.md) 集合| 如果 **accessReviewHistoryDefinition** 是定期定义，则实例表示每个定期。 不重复的定义将只有一个实例。|

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
