---
title: accessReviewStage 资源类型
description: 表示 accessReviewInstance 的阶段。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 20e23693bce96e0e10eb0f173ceb65ee1516a0a8
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698077"
---
# <a name="accessreviewstage-resource-type"></a>accessReviewStage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示 Azure AD [访问评审](accessreviewsv2-overview.md) 重复的阶段。 如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 定义了 **stageSettings** 属性， [则 accessReviewInstance](accessReviewInstance.md) 最多由三个后续阶段组成。 每个阶段可能有一组不同的审阅者，他们可以对舞台决策采取行动，并设置确定哪些决策将从阶段传递到阶段。

每个 **accessReviewStage** 都包含审阅者可以执行的 [决策](accessreviewinstancedecisionitem.md) 列表。 每个标识只审查一个决定。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewStages](../api/accessreviewinstance-list-stages.md)|[accessReviewStage](../resources/accessreviewstage.md) 集合|获取 [accessReviewStage](../resources/accessreviewstage.md) 对象及其属性的列表。|
|[获取 accessReviewStage](../api/accessreviewstage-get.md)|[accessReviewStage](../resources/accessreviewstage.md)|读取 [accessReviewStage](../resources/accessreviewstage.md) 对象的属性和关系。|
|[更新 accessReviewStage](../api/accessreviewstage-update.md)|[accessReviewStage](../resources/accessreviewstage.md)|更新 [accessReviewStage](../resources/accessreviewstage.md) 对象的属性。|
|[stop](../api/accessreviewstage-stop.md)|无| 手动停止 accessReviewStage。|
|[filterByCurrentUser](../api/accessreviewstage-filterbycurrentuser.md)|[accessReviewStage](../resources/accessreviewstage.md) 集合|返回给定 [accessReviewInstance](accessReviewInstance.md)  上调用用户为审阅者的所有阶段。|
|[列出决策](../api/accessreviewstage-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|获取 accessReviewStage 中所做的决策。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|endDateTime|DateTimeOffset|计划结束审阅阶段时的 DateTime。 DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 此属性是所有阶段的 **持续时间的** 累计总计。 只读。 |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|此审阅者范围集合用于定义回退审阅者列表。 如果未从指定的审阅者列表中找到任何用户，则会通知这些回退审阅者采取行动。 如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的管理器不存在，则可能会发生这种情况。|
|id|字符串|阶段的唯一标识符。 只读。|
|评论家|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|此访问评审范围集合用于定义审阅者是谁。 有关分配审阅者的选项示例，请参阅[使用 Microsoft 图形 API 将审阅者分配到访问评审定义](/graph/accessreviews-scope-concept)。|
|startDateTime|DateTimeOffset|计划开始审阅阶段时的 DateTime。 将来可能。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 只读。 |
|status|String|指定 accessReviewStage 的状态。 可能的值：`Initializing`、`NotStarted`、`Starting`、`InProgress`、`Completing`、`Completed`和 `AutoReviewing``AutoReviewed`。 支持 `$orderby`，仅 `$filter` (`eq`) 。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|决定|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|AccessReviewStage 中审阅的每个用户都有一个决策项，表示是否已批准、拒绝或尚未审核。|

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

