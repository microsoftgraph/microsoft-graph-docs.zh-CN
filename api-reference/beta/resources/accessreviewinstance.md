---
title: accessReviewInstance 资源类型
description: 表示 .. 的 `accessReviewScheduleDefinition`重复周期。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5dece4ad638758a51e8aa839cbb755ec5b79d6fd
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697216"
---
# <a name="accessreviewinstance-resource-type"></a>accessReviewInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示 Azure AD [访问评审](accessreviewsv2-overview.md) 定期。 如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 是定期访问评审，则实例表示每个重复访问。 不重复的审阅将完全有一个实例。 实例还表示计划定义中正在审查的每个唯一组。 如果计划定义对多个组进行评审，则每个组将为每个重复周期提供唯一实例。

每个 **accessReviewInstance** 都包含审阅者可以执行的 [决策](accessreviewinstancedecisionitem.md) 列表。 每个标识都有一个要审查的决定。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstances](../api/accessreviewscheduledefinition-list-instances.md) | [accessReviewInstance](accessreviewinstance.md) 集合 | 获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。 |
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | 读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。 |
|[更新 accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|更新 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的审阅者。|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|返回给定 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 上的所有实例，调用用户是一个或多个决策的审阅者。|
|[列出联系的审阅者](../api/accessreviewinstance-list-contactedreviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md) 集合|获取收到访问评审实例通知的审阅者。|
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | 无。 | 向 accessReviewInstance 的审阅者发送提醒。 |
|[stop](../api/accessreviewinstance-stop.md) | 无。 | 手动停止 accessReviewInstance。 |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | 无。 | 允许调用用户接受针对每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议，即他们是特定 accessReviewInstance 的审阅者。 |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | 无。 | 在 accessReviewInstance 上手动应用决策。 |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|无|在一次调用中查看主体或资源的批处理。|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|无|将实例上的所有决策项重置为 `notReviewed`。|
|[列出阶段](../api/accessreviewinstance-list-stages.md)|[accessReviewStage](../resources/accessreviewstage.md) 集合| 检索多阶段访问评审实例中的阶段。|
|[列出决策](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|从决策导航属性获取 accessReviewInstanceDecisionItem 资源。|
|[列出挂起的AccessReviewInstances (已弃用) ](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance](accessreviewinstance.md) 集合。 | 获取分配给调用用户的所有挂起的 accessReviewInstance 资源。 此方法已被弃用并替换为 [filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)。 |

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------------------------------- | :---------- |
| endDateTime | DateTimeOffset | 当审阅实例计划结束时，DateTime。DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。|
| 错误 | [accessReviewError](accessreviewerror.md) 集合| 访问评审实例生命周期中的错误集合。 只读。 |
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果未从指定的审阅者列表中找到任何用户，则会通知这些回退审阅者采取行动。 如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的管理器不存在，则可能会发生这种情况。 支持 `$select`。|
| id | String | 实例的唯一标识符。 支持 `$select`。 只读。|
| scope | [accessReviewScope](accessreviewscope.md) | **基于** accessReviewScheduleDefinition 级别的范围和 **instanceEnumerationScope** 创建。 定义在组中审阅的用户的范围。 仅支持 `$select` 和 `$filter` (`contains`) 。 只读。 |
| startDateTime | DateTimeOffset | 计划启动审阅实例时的 DateTime。 将来可能。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。 |
| status | 字符串 | 指定 accessReview 的状态。 可能的值：`Initializing`、`NotStarted`、`Starting`、`InProgress`、`Completing`、`Completed`和 `AutoReviewing``AutoReviewed`。 仅支持`$select`和 `$orderby``$filter` (`eq`) 。 只读。|
| 评论家   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义审阅者是谁。 支持 `$select`。 有关分配审阅者的选项示例，请参阅[使用 Microsoft 图形 API 将审阅者分配到访问评审定义](/graph/accessreviews-scope-concept)。|


## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| contactedReviewers   |[accessReviewReviewer](../resources/accessreviewreviewer.md) 集合| 返回被联系以完成此评审的审阅者的集合。 虽然 **accessReviewScheduleDefinition** 的 **审阅者** 和 **fallbackReviewers** 属性可能会将组所有者或经理指定为 **审阅者**，但 **联系的Reviewers** 将返回其个人标识。 支持 `$select`。 只读。 |
| 定义               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | 与每个实例完全关联了一个 **accessReviewScheduleDefinition** 。 它是实例的父计划，其中为审阅定义的每个重复周期以及由定义选择的每个组创建实例。 |
|stages|[accessReviewStage](accessreviewstage.md) 集合| 如果实例有多个阶段，则返回阶段的集合。 只有在上一阶段结束时才会创建新阶段。 审阅实例上阶段的存在、编号和设置是基于父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 上的 [accessReviewStageSettings](accessreviewstagesettings.md) 创建的。 |
| 决定               |[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合        | **AccessReviewInstance** 中审阅的每个用户都有一个决策项，该决定项表示是否已批准、拒绝或尚未审核。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
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
  ],
  "contactedReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewer"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
