---
title: accessReviewHistoryDefinition 资源类型
description: 表示访问评审历史记录数据的集合。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 96619cb95c11a77106c86cbdcc720f1a486721c7
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232912"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>accessReviewHistoryDefinition 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示访问评审历史记录数据和用于收集数据的范围的集合。 **reviewHistoryPeriodStartDateTime**、 **reviewHistoryPeriodEndDateTime**、 **decisions** 和 **scopes** 属性的 **accessReviewHistoryDefinition** are used when selecting review history data， and can be modified. 每个 **accessReviewHistoryDefinition** 对象只能使用 30 天。 一旦历史记录定义的状态移动到链接，就可以通过调用 `done` [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md)来检索定义的数据。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewHistoryDefinitions](../api/accessreviewhistorydefinition-list.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 集合|获取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象及其属性的列表。|
|[创建 accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-post.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|创建新的 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象。|
|[获取 accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|读取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象的属性和关系。|
|[generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|生成可用于检索审阅历史记录数据的 URI。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdBy|[userIdentity](useridentity.md)| 创建此审阅历史记录定义的用户。 |
|createdDateTime|DateTimeOffset|创建访问评审定义的时间戳。|
|决策|String collection|确定提取的审阅历史记录数据中将包含哪些审阅决策（如果已指定）。 创建时可选。 如果未提供创建决策，则默认情况下将包含所有决策。 可能的值是 `approve` `deny` `dontKnow` ：、、、 `notReviewed` 和 `notNotified` 。|
|displayName|String|访问评审历史记录数据收集的名称。 必需。|
|downloadUri|String|可用于检索审阅历史记录数据的 Uri。 生成后，此 URI 将处于活动状态 24 小时。|
|fulfilledDateTime|DateTimeOffset|收集此定义的所有可用数据的时间戳。 This will be set after this definition's status is set to `done` .|
|id|String|为访问评审历史记录定义分配的唯一标识符。|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|时间戳、在此日期当天或之后开始审阅将包含在提取的历史记录数据中。 必需。|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|时间戳、在此日期或之前开始审阅将包含在提取的历史记录数据中。 必需。|
|scopes|microsoft.graph.accessReviewQueryScope 集合|用于确定提取的历史记录数据中包含的审阅的范围。 获取其范围与提供的范围匹配的审阅。 请参阅 [accessreviewqueryscope](accessreviewqueryscope.md)。 必需。|
|状态|String collection|表示审阅历史记录数据收集的状态。 可取值为：`done`、`inprogress`、`error`、`requested`。|

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
  "decisions": [
    {
      "@odata.type": "String"
    }
  ],
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "createdBy": {
    "@odata.type": "#microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    }
  ]
}
```
