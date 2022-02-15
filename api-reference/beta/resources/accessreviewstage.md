---
title: accessReviewStage 资源类型
description: 表示 accessReviewInstance 的阶段。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 53d0fa58f4aa494f1815a1205f45ba2673b9620c
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816179"
---
# <a name="accessreviewstage-resource-type"></a>accessReviewStage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示访问评审定期Azure AD[阶段](accessreviewsv2-overview.md)。 如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 已定义 **stageSettings** 属性， [则 accessReviewInstance](accessReviewInstance.md) 最多包含三个后续阶段。 每个阶段可能都有一组不同的审阅者，这些审阅者可以就阶段决策采取行动，并设置确定将在不同阶段传递哪些决策。

每个 **accessReviewStage** 都包含审阅 [者可以采取措施](accessreviewinstancedecisionitem.md) 的决策列表。 每个正在审阅的标识只有一个决策。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewStages](../api/accessreviewinstance-list-stages.md)|[accessReviewStage](../resources/accessreviewstage.md) 集合|获取 [accessReviewStage](../resources/accessreviewstage.md) 对象及其属性的列表。|
|[获取 accessReviewStage](../api/accessreviewstage-get.md)|[accessReviewStage](../resources/accessreviewstage.md)|读取 [accessReviewStage](../resources/accessreviewstage.md) 对象的属性和关系。|
|[更新 accessReviewStage](../api/accessreviewstage-update.md)|[accessReviewStage](../resources/accessreviewstage.md)|更新 [accessReviewStage 对象](../resources/accessreviewstage.md) 的属性。|
|[stop](../api/accessreviewstage-stop.md)|无| 手动停止 accessReviewStage。|
|[filterByCurrentUser](../api/accessreviewstage-filterbycurrentuser.md)|[accessReviewStage](../resources/accessreviewstage.md) 集合|返回调用用户是审阅者的给定 [accessReviewInstance](accessReviewInstance.md)  上的所有阶段。|
|[列出决策](../api/accessreviewstage-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|获取在 accessReviewStage 中做出的决策。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|endDateTime|DateTimeOffset|将审阅阶段安排为结束的 DateTime。 DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 此属性是所有阶段的 **durationInDays** 累积总计。 只读。 |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|此审阅者范围集合用于定义回退审阅者列表。 如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。 当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。|
|id|String|阶段的唯一标识符。 只读。|
|reviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|此访问评审范围集合用于定义审阅者是谁。 有关分配审阅者的选项示例，请参阅使用 Microsoft Graph API 将审阅者分配给你的访问[Graph定义](/graph/accessreviews-scope-concept)。|
|startDateTime|DateTimeOffset|计划启动审阅阶段的 DateTime。 可能在将来。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|状态|String|指定 accessReviewStage 的状态。 可能的值：、`Initializing`、`Starting``NotStarted`、`InProgress`、`Completing`、`Completed`、`AutoReviewing`、 和 `AutoReviewed`。 仅 `$orderby`支持 (`$filter` `eq` 和) 。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|决策|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|在 accessReviewStage 中审阅的每个用户都有一个决策项，该项目表示他们被批准、拒绝还是尚未审阅。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewStage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewStage",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```

