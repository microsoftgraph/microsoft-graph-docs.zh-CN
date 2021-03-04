---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示有关用户访问 accessReviewInstance 的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 228fbe473fe65fe84c9dfa7c62f3689681d47e39
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443186"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示有关评价 [实例的](accessreviewsv2-root.md) Azure AD 访问评审决定。 此决定表示确定用户或服务主体对给定访问评审实例 [的访问权限](accessreviewinstance.md)。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 列出特定 accessReviewInstance 的每个 accessReviewInstanceDecisionItem。 |
|[列出待审批的 accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。 | 获取分配给调用用户的所有 accessReviewInstanceDecisionItems，用于特定 accessReviewInstance。 |
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | 无。 | 对于分配了呼叫用户审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。 |

## <a name="properties"></a>属性
| 属性 | 类型 |  说明 |
| :---------------| :---- | :---------- |
| id | String | 决策的标识符。 |
| accessReviewId | String | accessReviewInstance 父项的标识符。 |
| reviewedBy | [userIdentity](useridentity.md) | 审阅者的标识符。 |
| reviewedDateTime | DateTimeOffset | 审阅发生的 DateTime。 |
| 决策 | String | 评价结果。 可能的值 `Approve` `Deny` ：、、 `NotReviewed` 或 `DontKnow` 。 |
| justification | String | 审阅决策理由。 |
| appliedBy | [userIdentity](useridentity.md) | 应用决策的用户的标识符。 |
| appliedDateTime | DateTimeOffset | 应用审批决定的日期/时间。 |
| applyResult | String | 应用决策的结果。 可能的值 `NotApplied` `Success` `Failed` ：、、、 `NotFound` 或 `NotSupported` 。 |
| recommendation | String | 针对审批决策的系统生成的建议。 可能的值： `Approve` ， `Deny` 或 `NotAvailable` 。  |
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | 此特定决策的目标。 决策目标可以是不同类型的 ， 每个类型都有其自己的特定属性。 请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| 实例 |[accessReviewInstance](accessreviewinstance.md) | 每个决策只关联一个 accessReviewInstance。 该实例是决策项的父项，表示做出该决策的访问评审的定期发生。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "openType": true
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
 "id": "string (identifier)",
 "accessReviewId": "string",
 "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
 },
 "reviewedDateTime": "string (timestamp)",
 "decision": "string",
 "justification": "string",
 "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
 "appliedDateTime": "DateTimeOffset",
 "applyResult": "string",
 "recommendation": "string",
 "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstanceDecisionItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
