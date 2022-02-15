---
title: accessReviewInstance 资源类型
description: 表示 重复发生 `accessReviewScheduleDefinition`。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 68863a90e4b059a22525c6f8342c32fb513a2e7c
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62815977"
---
# <a name="accessreviewinstance-resource-type"></a>accessReviewInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示访问Azure AD[重复周期](accessreviewsv2-overview.md)。 如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 是定期访问评审，则实例表示每个重复周期。 不重复的审阅将只具有一个实例。 实例还表示计划定义中正在审阅的每个唯一组。 如果计划定义审阅多个组，则每个组将具有每个重复周期的唯一实例。

每个 **accessReviewInstance** 都包含审阅者可以 [](accessreviewinstancedecisionitem.md)采取措施的决策列表。 每个正在审阅的身份有一个决策。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstances](../api/accessreviewscheduledefinition-list-instances.md) | [accessReviewInstance](accessreviewinstance.md) 集合 | 获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。 |
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | 读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。 |
|[更新 accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|更新 [accessReviewInstance 对象的](../resources/accessreviewinstance.md) 审阅者。|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|返回给定 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 上的所有实例，调用用户是一个或多个决策的审阅者。|
|[列出联系的审阅者](../api/accessreviewinstance-list-contactedreviewers.md)|[accessReviewReviewer](../resources/accessreviewreviewer.md) 集合|获取收到访问评审实例通知的审阅者。|
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | 无。 | 向 accessReviewInstance 的审阅者发送提醒。 |
|[stop](../api/accessreviewinstance-stop.md) | 无。 | 手动停止 accessReviewInstance。 |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | 无。 | 允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。 |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | 无。 | 手动对 accessReviewInstance 应用决策。 |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|无|在一次调用中查看主体或资源的批次。|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|无|将实例上的所有决策项重置为 `notReviewed`。|
|[列出阶段](../api/accessreviewinstance-list-stages.md)|[accessReviewStage](../resources/accessreviewstage.md) 集合| 检索多阶段访问评审实例中的阶段。|
|[列出决策](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|从 decisions 导航属性获取 accessReviewInstanceDecisionItem 资源。|
|[列出已弃 (pendingAccessReviewInstances) ](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance](accessreviewinstance.md) 集合。 | 获取分配给调用用户的所有待定 accessReviewInstance 资源。 此方法已被弃用，并替换为 [filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)。 |

## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------------------------------- | :---------- |
| endDateTime | DateTimeOffset | 将审阅实例计划结束的 DateTime。DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。|
| 错误 | [accessReviewError](accessreviewerror.md) 集合| 访问评审实例生命周期中的错误集合。 只读。 |
| fallbackReviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此审阅者范围集合用于定义回退审阅者列表。 如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。 当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。 支持 `$select`。|
| id | String | 实例的唯一标识符。 支持 `$select`。 只读。|
| scope | [accessReviewScope](accessreviewscope.md) | 基于 accessReviewScheduleDefinition 级别的 scope 和 **instanceEnumerationScope** 创建。 定义在组中查看的用户范围。 仅 `$select` 支持 `$filter` (`contains` 和) 。 只读。 |
| startDateTime | DateTimeOffset | 计划启动审阅实例的 DateTime。 可能在将来。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 支持 `$select`。 只读。 |
| 状态 | String | 指定 accessReview 的状态。 可能的值：、`Initializing`、`Starting``NotStarted`、`InProgress`、`Completing`、`Completed`、`AutoReviewing`、 和 `AutoReviewed`。 仅 `$select`支持 `$orderby`、 (`$filter` `eq` 和) 。 只读。|
| reviewers   |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此访问评审范围集合用于定义审阅者是谁。 支持 `$select`。 有关分配审阅者的选项示例，请参阅使用 Microsoft Graph API 将审阅者分配给你的访问[Graph定义](/graph/accessreviews-scope-concept)。|


## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| contactedReviewers   |[accessReviewReviewer](../resources/accessreviewreviewer.md) 集合| 返回为完成此审阅而联系的审阅者的集合。 虽然 **accessReviewScheduleDefinition** 的 **reviewers** 和 **fallbackReviewers** 属性可能会将组所有者或经理指定为审阅者，**但 contactedReviewers** 将返回其个人标识。 支持 `$select`。 只读。 |
| definition               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | 每个实例只关联一 **个 accessReviewScheduleDefinition** 。 它是实例的父计划，其中为审阅定义的每个重复周期创建实例，并按定义选择查看每个组。 |
|stages|[accessReviewStage](accessreviewstage.md) 集合| 如果实例具有多个阶段，这将返回阶段的集合。 只有在上一阶段结束时，才能创建一个新阶段。 审阅实例上阶段的存在、数量和设置是基于父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 上的 [accessReviewStageSettings](accessreviewstagesettings.md) 创建的。 |
| 决策               |[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合        | 在 **accessReviewInstance** 中查看的每个用户都有一个决策项，代表他们被批准、拒绝还是尚未被审阅。 |

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
