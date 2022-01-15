---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示有关用户访问 accessReviewInstance 的决定。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ec8d3fdd98c85caeb82552d41b0501fe06c80378
ms.sourcegitcommit: 94741ff7f61f20a39dacfa6ce451a77ca02dd68a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2022
ms.locfileid: "62047239"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示[Azure AD实例的访问](accessreviewsv2-overview.md)评审决定。 此决定是确定用户或服务主体对给定访问评审实例 [的访问权限](accessreviewinstance.md)。 accessReviewInstanceDecisionItem 是一个开放类型，允许传入其他属性。

## <a name="methods"></a>方法

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstance-list-decisions.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 获取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象及其属性的列表。|
|[获取 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。|
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | 无。 | 对于为调用用户分配审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。 |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|检索所有 [accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) 对象，其中调用的 use 是给定 [accessReviewInstance 的审阅者](accessreviewinstance.md)。|
|[列出 accessReviewInstanceDecisionItems 等待审批 (已弃) ](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。 | 获取分配给特定 accessReviewInstance 的调用用户的所有 accessReviewInstanceDecisionItems。 此方法已被弃用，并替换为 [filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)。 |

## <a name="properties"></a>属性
| 属性 | 类型 |  说明 |
| :---------------| :---- | :---------- |
|accessReviewId|String|accessReviewInstance 父项的标识符。 支持 `$select`。 只读。|
|appliedBy|[userIdentity](../resources/useridentity.md)|应用了该决策的用户的标识符。 只读。|
|appliedDateTime|DateTimeOffset|应用批准决策的时间戳。 DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。  支持 `$select`。 只读。|
|applyResult|String|应用决策的结果。 可能的值 `New` `AppliedSuccessfully` ：、、 `AppliedWithUnknownFailure` `AppliedSuccessfullyButObjectNotFound` 和 `ApplyNotSupported` 。 仅 `$select` `$orderby` 支持 (、 和 `$filter` `eq`) 。 只读。|
|decision|String|评价的结果。 可能的值 `Approve` `Deny` ：、、 `NotReviewed` 或 `DontKnow` 。 仅 `$select` `$orderby` 支持 (、 和 `$filter` `eq`) 。 |
|id|String| 决策的标识符。 继承自 [实体](../resources/entity.md)。 支持 `$select`。 只读。|
|justification|String|审阅者做出决策时留下的理由。|
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | 此特定决策的目标。 决策目标可以是不同类型的 ，每个类型都有其自己的特定属性。 请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。 只读。 <br/> 此属性已被 `principal` `resource` v1.0 中的 和 属性所取代。|
|principal|[identity](../resources/identity.md)|访问评审中的每个决策项表示主体对资源的访问权限。 此属性表示主体的详细信息。 例如，如果某个决策项表示用户"Bob"对组"Sales"的访问权限 - 主体为"Bob"，资源为"Sales"。 主体可以是两种类型 - userIdentity 和 servicePrincipalIdentity。 支持 `$select`。 只读。|
|principalLink|String|链接到主体对象。 例如：`https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`。 只读。|
|建议|String|针对基于上次交互式登录租户的审批决策的系统生成的建议。 如果登录是自审查开始起 30 天内，建议批准。 如果登录自审查开始超过 30 天，建议拒绝。 否则，建议不可用。 可能的值 `Approve` ：、 `Deny` 或 `NoInfoAvailable` 。 仅 `$select` `$orderby` 支持 (、 和 `$filter` `eq`) 。 只读。|
|resource|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|访问评审中的每个决策项表示主体对资源的访问权限。 此属性表示资源的详细信息。 例如，如果某个决策项表示用户"Bob"对组"销售"的访问权限 - 主体为 Bob，资源为"Sales"。 资源可以是多种类型的。 请参阅 [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)。 只读。|
|resourceLink|String|指向资源的链接。 例如，`https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8`。 支持 `$select`。 只读。|
|reviewedBy|[userIdentity](../resources/useridentity.md)| 审阅者的标识符。 支持 `$select`。 只读。|
|reviewedDateTime|DateTimeOffset| 发生审阅决策的时间戳。 支持 `$select`。 只读。|

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
  "id": "String (identifier)",
  "accessReviewId": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "reviewedDateTime": "String (timestamp)",
  "decision": "String",
  "justification": "String",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "String (timestamp)",
  "applyResult": "String",
  "recommendation": "String",
  "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  },
  "principal": {
    "@odata.type": "microsoft.graph.identity"
  },
  "principalLink": "String",
  "resource": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
  },
  "resourceLink": "String"
}
```
