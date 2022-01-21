---
title: accessReviewInstance 资源类型
description: 表示 accessReviewScheduleDefinition 对象的定期发生。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84f687726978eb03c08de19aac10015128eb1944
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161247"
---
# <a name="accessreviewinstance-resource-type"></a>accessReviewInstance 资源类型

命名空间：microsoft.graph

表示访问Azure AD[重复周期](accessreviewsv2-overview.md)。 基于父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的系统生成。 所有属性都是只读的。

如果实例是定期访问评审的一部分，则实例表示每个重复周期。 不重复的审阅将只具有一个实例。 实例还表示计划定义中正在审阅的每个唯一资源。 如果计划定义审阅多个资源，则每个资源将具有每个重复周期的唯一实例。

每个 **accessReviewInstance** 都包含审阅 [](accessreviewinstancedecisionitem.md)者可以采取措施的决策列表。 每个正在审阅的身份有一个决策。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewInstances](../api/accessreviewscheduledefinition-list-instances.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。|
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。|
|[更新 accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|更新 [accessReviewInstance 对象的](../resources/accessreviewinstance.md) 审阅者。|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|返回调用用户是审阅者的定义上的所有实例对象。|
|[列出联系的审阅者](../api/accessreviewinstance-list-contactedreviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md) 集合|获取收到访问评审实例通知的审阅者。|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|None|向 accessReviewInstance 的审阅者发送提醒。|
|[stop](../api/accessreviewinstance-stop.md)|None|手动停止 accessReviewInstance。|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|None| 允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|None|手动对 accessReviewInstance 应用决策。|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|None|在一次调用中查看主体或资源的批次。|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|None|将实例上的所有决策项重置为 `notReviewed`|
|[列出决策](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|从 decisions 导航属性获取 accessReviewInstanceDecisionItem 资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| endDateTime | DateTimeOffset | 将审阅实例计划结束的 DateTime。DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。|
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。 当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。 支持 `$select`。|
| id | String | 实例的唯一标识符。 继承自 [实体](../resources/entity.md)。 支持 `$select`。 只读。|
| scope | [accessReviewScope](accessreviewscope.md) | 基于 accessReviewScheduleDefinition 级别的 scope 和 **instanceEnumerationScope** 创建。  定义在组中查看的用户范围。 仅 `$select` 支持 `$filter` (`contains` 和) 。 只读。 |
| startDateTime | DateTimeOffset | 计划启动审阅实例的 DateTime。 可能在将来。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。 |
| 状态 | String | 指定 accessReview 的状态。 可能的值 `Initializing` `NotStarted` `Starting` ：、、、、、、、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。 仅 `$select` `$orderby` 支持 `$filter` `eq` (、 和) 。 只读。|
| reviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义审阅者是谁。 支持 `$select`。 有关分配审阅者的选项示例，请参阅使用 Microsoft Graph API 将审阅者分配给你的访问[Graph定义](/graph/accessreviews-scope-concept)。|


## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|决策|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|在 **accessReviewInstance** 中审阅的每个主体都有一个决策项，表示它们被批准、拒绝还是尚未审阅。|
| contactedReviewers   |[accessReviewReviewer](../resources/accessreviewreviewer.md) 集合| 返回为完成此审阅而联系的审阅者的集合。 虽然 **accessReviewScheduleDefinition** 的 **reviewers** 和 **fallbackReviewers** 属性可能会将组所有者或经理指定为审阅者，**但 contactedReviewers** 将返回其个人标识。 支持 `$select`。 只读。 |

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
