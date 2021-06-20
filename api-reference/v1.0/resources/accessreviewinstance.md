---
title: accessReviewInstance 资源类型
description: 表示 重复发生 `accessReviewScheduleDefinition` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2d1575e749927ee924b752c1bb69f9b31f923471
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031050"
---
# <a name="accessreviewinstance-resource-type"></a>accessReviewInstance 资源类型

命名空间：microsoft.graph

表示 Azure AD [访问评审](accessreviewsv2-root.md) 定期。 基于父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的系统生成。 所有属性都是只读的。

如果实例是定期访问评审的一部分，则实例表示每个重复周期。 不重复的审阅将只具有一个实例。 实例还表示计划定义中正在审阅的每个唯一资源。 如果计划定义审阅多个资源，则每个资源将具有每个重复周期的唯一实例。

每个 **accessReviewInstance** 都包含审阅 [](accessreviewinstancedecisionitem.md)者可以采取措施的决策列表。 每个正在审阅的身份有一个决策。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewInstances](../api/accessreviewinstance-list.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。|
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。|
|[stop](../api/accessreviewinstance-stop.md)|无|手动停止 accessReviewInstance。|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|无|向 accessReviewInstance 的审阅者发送提醒。|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|无|将实例上的所有决策项重置为 `notReviewed`|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|无|手动对 accessReviewInstance 应用决策。|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|无| 允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|无|在一次调用中查看主体或资源的批次。|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|返回调用用户是审阅者的定义上的所有实例对象。|
|[列出决策](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|从 decisions 导航属性获取 accessReviewInstanceDecisionItem 资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| id | String | 实例的唯一标识符。 继承自 [实体](../resources/entity.md)。 支持 `$select`。 只读。|
| startDateTime | DateTimeOffset | 计划启动审阅实例的 DateTime。 可能在将来。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。 |
| endDateTime | DateTimeOffset | 将审阅实例计划结束的 DateTime。DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。|
| 状态 | String | 指定 accessReview 的状态。 可能的值 `Initializing` `NotStarted` `Starting` ：、、、、、、、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。 仅 `$select` `$orderby` 支持 、 (`$filter` 和 `eq`) 。 只读。|
| scope | [accessReviewScope](accessreviewscope.md) | 基于 accessReviewScheduleDefinition 级别的 scope 和 **instanceEnumerationScope** 创建。  定义在组中查看的用户范围。 仅 `$select` 支持 `$filter` (`contains` 和) 。 只读。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|决策|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|在 中审核的每个主体都有一个决策项，该项目表示它们被批准、拒绝还是 `accessReviewInstance` 尚未被审阅。|

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
  }
}
```
