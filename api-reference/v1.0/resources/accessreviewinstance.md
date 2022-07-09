---
title: accessReviewInstance 资源类型
description: 表示 accessReviewScheduleDefinition 对象的重复周期。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5fe495a689a27f5d7dcd76f9148e51185339bdbe
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698308"
---
# <a name="accessreviewinstance-resource-type"></a>accessReviewInstance 资源类型

命名空间：microsoft.graph

表示 Azure AD [访问评审](accessreviewsv2-overview.md) 定期。 基于父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象生成的系统。 所有属性都是只读的。

如果实例是定期访问评审的一部分，则实例表示每一次重复。 不重复的审阅将完全有一个实例。 实例还表示计划定义中正在审查的每个唯一资源。 如果计划定义对多个资源进行评审，则每个资源将为每个重复周期提供唯一实例。

每个 **accessReviewInstance** 都包含审阅者可以执行的 [决策](accessreviewinstancedecisionitem.md) 列表。 每个标识都有一个要审查的决定。

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewInstances](../api/accessreviewscheduledefinition-list-instances.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。|
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。|
|[更新 accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|更新 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的审阅者。|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|返回调用用户为审阅者的定义上的所有实例对象。|
|[列出联系的审阅者](../api/accessreviewinstance-list-contactedreviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md) 集合|获取收到访问评审实例通知的审阅者。|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|无|向 accessReviewInstance 的审阅者发送提醒。|
|[stop](../api/accessreviewinstance-stop.md)|无|手动停止 accessReviewInstance。|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|无| 允许调用用户接受针对每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议，即他们是特定 accessReviewInstance 的审阅者。|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|无|对 accessReviewInstance 手动应用决策。|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|无|在一次调用中查看主体或资源的批处理。|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|无|将实例上的所有决策项重置为 `notReviewed`|
|[列出决策](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|从决策导航属性获取 accessReviewInstanceDecisionItem 资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| endDateTime | DateTimeOffset | 当审阅实例计划结束时，DateTime。DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。|
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果未从指定的审阅者列表中找到任何用户，则会通知这些回退审阅者采取行动。 如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的管理器不存在，则可能会发生这种情况。 支持 `$select`。|
| id | String | 实例的唯一标识符。 继承自 [entity](../resources/entity.md)。 支持 `$select`。 只读。|
| scope | [accessReviewScope](accessreviewscope.md) | **基于** accessReviewScheduleDefinition 级别的范围和 **instanceEnumerationScope** 创建。 定义在组中审阅的用户的范围。 仅支持 `$select` 和 `$filter` (`contains`) 。 只读。 |
| startDateTime | DateTimeOffset | 计划启动审阅实例时的 DateTime。 将来可能。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。 |
| status | 字符串 | 指定 accessReview 的状态。 可能的值：`Initializing`、`NotStarted`、`Starting`、`InProgress`、`Completing`、`Completed`和 `AutoReviewing``AutoReviewed`。 仅支持`$select`和 `$orderby``$filter` (`eq`) 。 只读。|
| 评论家   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义审阅者是谁。 支持 `$select`。 有关分配审阅者的选项示例，请参阅[使用 Microsoft 图形 API 将审阅者分配到访问评审定义](/graph/accessreviews-scope-concept)。|


## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|决定|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|**AccessReviewInstance** 中审阅的每个主体都有一个决策项，表示它们是否已获得批准、拒绝或尚未审查。|
| contactedReviewers   |[accessReviewReviewer](../resources/accessreviewreviewer.md) 集合| 返回被联系以完成此评审的审阅者的集合。 虽然 **accessReviewScheduleDefinition** 的 **审阅者** 和 **fallbackReviewers** 属性可能会将组所有者或经理指定为 **审阅者**，但 **联系的Reviewers** 将返回其个人标识。 支持 `$select`。 只读。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstance",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
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
