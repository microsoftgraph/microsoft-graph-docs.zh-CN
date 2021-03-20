---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示有关用户访问 accessReviewInstance 的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e5d9b64faafb7dfe4ec4e6f3487643e62885236a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952814"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示有关审阅 [实例](accessreviewsv2-root.md) 的 Azure AD 访问评审决定。 此决定表示确定用户或服务主体对给定访问评审实例 [的访问权限](accessreviewinstance.md)。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 列出特定 accessReviewInstanceDecisionItem 的每个 accessReviewInstance。 |
|[列出 accessReviewInstanceDecisionItems 待审批](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。 | 获取分配给特定 accessReviewInstance 的调用用户的所有 accessReviewInstanceDecisionItems。 |
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | 无。 | 对于为调用用户分配审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。 |

## <a name="properties"></a>属性
| 属性 | 类型 |  说明 |
| :---------------| :---- | :---------- |
| id | String | 决策的标识符。 |
| accessReviewId | String | accessReviewInstance 父项的标识符。 |
| reviewedBy | [userIdentity](useridentity.md) | 审阅者的标识符。 |
| reviewedDateTime | DateTimeOffset | 评价发生时的时间戳。 |
| decision | String | 评价的结果。 可能的值 `Approve` `Deny` ：、、 `NotReviewed` 或 `DontKnow` 。 |
| justification | String | 审阅决策理由。 |
| appliedBy | [userIdentity](useridentity.md) | 应用了该决策的用户的标识符。 |
| appliedDateTime | DateTimeOffset | 应用批准决策的时间戳。 DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
| applyResult | String | 应用决策的结果。 可能的值 `NotApplied` `Success` `Failed` ：、、、 `NotFound` 或 `NotSupported` 。 |
| 建议 | String | 针对审批决策的系统生成的建议。 可能的值 `Approve` ：、 `Deny` 或 `NotAvailable` 。  |
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | 此特定决策的目标。 决策目标可以是不同类型的 ，每个类型都有其自己的特定属性。 请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| 实例 |[accessReviewInstance](accessreviewinstance.md) | 每个决策只关联一个 accessReviewInstance。 实例是决策项的父项，代表做出该决策的访问评审的重复发生。 |


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
