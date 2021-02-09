---
title: accessReviewInstance 资源类型
description: 表示定期的 `accessReviewScheduleDefinition` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0f480b870af2fd4717ff1341a1ab66b73301fc7f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158532"
---
# <a name="accessreviewinstance-resource-type"></a>accessReviewInstance 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD [访问评审](accessreviewsv2-root.md) 定期。 如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 是定期访问评审，则实例表示每个定期。 不重复的审阅将只具有一个实例。 实例还表示计划定义中正在审阅的每个唯一组。 如果计划定义审阅多个组，则每个组将具有每个重复周期的唯一实例。

每个 **accessReviewInstance** 都包含审阅 [](accessreviewinstancedecisionitem.md)者可以采取措施的决策列表。 要审阅每个标识有一个决策。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstances](../api/accessreviewinstance-list.md) | [accessReviewInstance](accessreviewinstance.md) 集合 | 获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。 |
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | 返回 accessReviewScheduleDefinition 的 accessReviewInstance。 对象中不包含关联的 accessReviewInstanceDecisionItem。 |
|[列出 pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance](accessreviewinstance.md) 集合。 | 获取分配给调用用户的所有待定 accessReviewInstance 资源。 |
|[发送 accessReviewInstance 提醒](../api/accessreviewinstance-sendreminder.md) | 无。 | 向 accessReviewInstance 的审阅者发送提醒。 |
|[停止 accessReviewInstance](../api/accessreviewinstance-stop.md) | 无。 | 手动停止 accessReviewInstance。 |
|[接受建议](../api/accessreviewinstance-acceptrecommendations.md) | 无。 | 允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。 |
|[应用决策](../api/accessreviewinstance-applydecisions.md) | 无。 | 手动对 accessReviewInstance 应用决策。 |



## <a name="properties"></a>属性
| 属性 | 类型 | 说明 |
| :-------------------------| :---------------------------------- | :---------- |
| id | String | 实例的唯一标识符。 |
| displayName | String | 父 accessReviewScheduleDefinition 的名称。 |
| startDateTime | DateTimeOffset | 计划启动审阅实例的 DateTime。 可能在将来。 |
| endDateTime | DateTimeOffset | 审核实例计划结束的 DateTime。 |
| 状态 | string | 指定 accessReview 的状态。 典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。  只读。|
| scope | [accessReviewScope](accessreviewscope.md) | 基于作用域 **和** **instanceEnumerationScope** 在 accessReviewScheduleDefinition 级别创建。 定义在组中查看的用户范围。 对于单组评审，在级别定义的范围 `accessReviewScheduleDefinition` 适用于所有实例。 对于所有组审阅，每个组的范围可能不同。 只读。  | 
| 决策 | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 在 accessReviewInstance 中审阅的每个用户都有一个决策项，它表示其访问是否得到批准、拒绝或尚未审查。 |
| definition |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 每个实例只关联一个 accessReviewScheduleDefinition。 它是实例的父计划，其中将针对每次定期审阅定义创建实例，并按定义选择查看每个组。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `definition`               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | 每个实例 `accessReviewScheduleDefinition` 只关联一个。 它是实例的父计划，其中将针对每次定期审阅定义创建实例，并按定义选择查看每个组。 |
| `decisions`               |[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合        | 在一个决策项中审阅的每个用户都有一个决策项，它表示他们被批准、拒绝 `accessReviewInstance` 还是尚未被审阅。 |

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
