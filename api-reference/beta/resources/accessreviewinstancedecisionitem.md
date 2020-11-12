---
title: accessReviewInstanceDecisionItem 资源类型
description: 代表用户对 accessReviewInstance 的访问的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9ad5f8a49d44c82f1a43a1666f08f2b49853395
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000843"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对评审实例的 Azure AD [访问审核](accessreviewsv2-root.md) 决定。 此决定表示确定用户或服务主体对给定的 [访问评审实例](accessreviewinstance.md)的访问权限。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 列出特定 accessReviewInstance 的每个 accessReviewInstanceDecisionItem。 |
|[列出 accessReviewInstanceDecisionItems 待审批](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。 | 获取特定 accessReviewInstance 的所有分配给呼叫用户的 accessReviewInstanceDecisionItems。 |
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | 无。 | 对于呼叫用户分配了审阅者的任何 accessReviewInstanceDecisionItems，呼叫用户可以通过修补决策对象来记录决策。 |

## <a name="properties"></a>属性
| 属性 | 类型 |  说明 |
| :---------------| :---- | :---------- |
| id | 字符串 | 决策的标识符。 |
| accessReviewId | 字符串 | AccessReviewInstance 父级的标识符。 |
| reviewedBy | [userIdentity](useridentity.md) | 审阅者的标识符。 |
| reviewedDateTime | DateTimeOffset | 评审发生时的日期时间。 |
| 权 | 字符串 | 评审的结果。 可能的值： `Approve` 、、 `Deny` `NotReviewed` 或 `DontKnow` 。 |
| 合理化 | 字符串 | 评审决策理由。 |
| appliedBy | [userIdentity](useridentity.md) | 应用决策的用户的标识符。 |
| appliedDateTime | DateTimeOffset | 应用审批决定时的日期时间。 |
| applyResult | 字符串 | 应用决策的结果。 可能的值： `NotApplied` 、 `Success` 、、 `Failed` `NotFound` 或 `NotSupported` 。 |
| 提出 | 字符串 | 系统生成的审批决策建议。 可能的值： `Approve` 、 `Deny` 或 `NotAvailable` 。  |
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | 此特定决策的目标。 决策目标可以是不同的类型–每种类型都有其自己的特定属性。 请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。 |

## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| 情况 |[accessReviewInstance](accessreviewinstance.md) | 与每个决策相关联的 accessReviewInstance 正好有一个。 该实例是决策项的父项，表示对进行决定的访问审核的重复。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "",
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
