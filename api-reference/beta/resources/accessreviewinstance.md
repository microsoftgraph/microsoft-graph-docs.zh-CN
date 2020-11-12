---
title: accessReviewInstance 资源类型
description: 表示的定期 `accessReviewScheduleDefinition` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 480774950e2257b7af099c02cbe7c6571c0ce4c6
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000844"
---
# <a name="accessreviewinstance-resource-type"></a>accessReviewInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示定期的 Azure AD [访问审核](accessreviewsv2-root.md) 。 如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 是定期访问审核，则实例表示每个重复周期。 不重复的审阅将只有一个实例。 实例还表示在日程安排定义中审阅的每个唯一组。 如果计划定义检查多个组，则每个组都将具有每个重复的唯一实例。

每个 **accessReviewInstance** 都包含审阅者可对其执行操作的 [决策](accessreviewinstancedecisionitem.md) 列表。 每个标识的检查都有一个决定。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstances](../api/accessreviewinstance-list.md) | [accessReviewInstance](accessreviewinstance.md) 集合 | 获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。 |
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | 返回 accessReviewScheduleDefinition 的 accessReviewInstance。 不包括对象中关联的 accessReviewInstanceDecisionItem。 |
|[列出 pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance](accessreviewinstance.md) 集合。 | 获取分配给呼叫用户的所有待处理的 accessReviewInstance 资源。 |
|[发送 accessReviewInstance 提醒](../api/accessreviewinstance-sendreminder.md) | 无。 | 向 accessReviewInstance 的审阅者发送提醒。 |
|[停止 accessReviewInstance](../api/accessreviewinstance-stop.md) | 无。 | 手动停止 accessReviewInstance。 |
|[接受建议](../api/accessreviewinstance-acceptrecommendations.md) | 无。 | 允许呼叫用户接受针对特定 accessReviewInstance 的审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。 |
|[应用决策](../api/accessreviewinstance-applydecisions.md) | 无。 | 手动对 accessReviewInstance 应用决策。 |



## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------------------------------- | :---------- |
| id | 字符串 | 实例的唯一标识符。 |
| displayName | 字符串 | 父 accessReviewScheduleDefinition 的名称。 |
| startDateTime | DateTimeOffset | 将审阅实例安排为启动时的日期/时间。 可能是将来的。 |
| endDateTime | DateTimeOffset | 将审阅实例安排结束时的日期/时间。 |
| 状态 | string | 指定 accessReview 的状态。 典型状态包括、、、、、、 `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。  只读。|
| scope | [accessReviewScope](accessreviewscope.md) | 根据 **作用域** 和 **instanceEnumerationScope** 在 accessReviewScheduleDefinition 级别创建。 定义在组中审阅的用户的范围。 在单组审阅的情况下，在该级别定义的作用域 `accessReviewScheduleDefinition` 适用于所有实例。 在所有组审阅的情况下，每个组的作用域可能会有所不同。 只读。  | 
| 针对 | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 在 accessReviewInstance 中审阅的每个用户都有一个决定其访问是已被批准、被拒绝还是尚未审阅的决议项目。 |
| 定义 |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 与每个实例关联的 accessReviewScheduleDefinition 正好有一个。 它是实例的父计划，其中实例是为每个评审定义的每个重复项创建的，每个组选择由定义评审。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `definition`               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | `accessReviewScheduleDefinition`与每个实例关联的只有一个。 它是实例的父计划，其中实例是为每个评审定义的每个重复项创建的，每个组选择由定义评审。 |
| `decisions`               |[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合        | 中审阅的每个用户 `accessReviewInstance` 都有一个决策项目，表示他们是已批准、已拒绝还是尚未审阅。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "",
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
  }
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
