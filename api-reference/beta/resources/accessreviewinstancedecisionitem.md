---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示用户对 accessReviewInstance 的访问权限的决策。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c1412a0354e4993de02ad5cdefc6fc732be545bc
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446376"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示对审阅实例的 Azure AD [访问评审](accessreviewsv2-overview.md) 决策。 此决定表示确定用户或服务主体对给定 [访问评审实例的访问权限](accessreviewinstance.md)。  此资源是允许传入其他属性的开放类型。

## <a name="methods"></a>Methods

| 方法 | 返回类型 | 说明 |
|:---------------|:--------|:----------|
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstance-list-decisions.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 获取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象及其属性的列表。|
|[获取 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。|
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | 无。 | 对于向调用用户分配审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。 |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|检索所有 [accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) 对象，其中调用使用是给定 [accessReviewInstance](accessreviewinstance.md) 的审阅者。|
|[列出待审批 (已弃用的 accessReviewInstanceDecisionItems) ](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。 | 获取分配给调用用户的所有 accessReviewInstanceDecisionItems，以获取特定 accessReviewInstance。 此方法已被弃用并替换为 [filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)。 |

## <a name="properties"></a>属性
| 属性 | 类型 |  说明 |
| :---------------| :---- | :---------- |
|accessReviewId|String|accessReviewInstance 父级的标识符。 支持 `$select`。 只读。|
|appliedBy|[userIdentity](../resources/useridentity.md)|应用决策的用户的标识符。 只读。|
|appliedDateTime|DateTimeOffset|应用审批决定的时间戳。 DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。  支持 `$select`。 只读。|
|applyResult|String|应用决策的结果。 可能的值：`New`、`AppliedSuccessfully`、 `AppliedSuccessfullyButObjectNotFound` `AppliedWithUnknownFailure`和 `ApplyNotSupported`. 仅支持`$select`和 `$orderby``$filter` (`eq`) 。 只读。|
|决定|String|评审结果。 可能的值：`Approve`、`Deny`或 `NotReviewed``DontKnow`。 仅支持`$select`和 `$orderby``$filter` (`eq`) 。 |
|id|String| 决策的标识符。 继承自 [entity](../resources/entity.md)。 支持 `$select`。 只读。|
|理由|String|审阅者做出决定时留下的理由。|
| target | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | 此特定决策的目标。 决策目标可以是不同类型 ，每个类型都有其自己的特定属性。 请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。 只读。 <br/> 此属性已替换为 `principal` v1.0 中的属性和 `resource` 属性。|
|主要|[identity](../resources/identity.md)|访问评审中的每个决策项都表示主体对资源的访问权限。 此属性表示主体的详细信息。 例如，如果决策项表示用户“Bob”对组“Sales”的访问权限 - 主体为“Bob”，资源为“Sales”。 主体可以是两种类型 - userIdentity 和 servicePrincipalIdentity。 支持 `$select`。 只读。|
|principalLink|String|链接到主体对象。 例如：`https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`。 只读。|
|建议|String|基于最后一次交互式登录到租户的审批决策的系统生成的建议。 如果登录在审阅开始后三十天内，建议批准。 如果登录超过 30 天的评审开始时间，建议拒绝。 否则，建议不可用。 可能的值：`Approve`或 `Deny``NoInfoAvailable`. 仅支持`$select`和 `$orderby``$filter` (`eq`) 。 只读。|
|resource|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|访问评审中的每个决策项都表示主体对资源的访问权限。 此属性表示资源的详细信息。 例如，如果决策项表示用户“Bob”对组“Sales”的访问权限 - 主体为 Bob，资源为“Sales”。 资源可以是多种类型。 请参阅 [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)。 只读。|
|resourceLink|String|指向资源的链接。 例如，`https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8`。 支持 `$select`。 只读。|
|reviewedBy|[userIdentity](../resources/useridentity.md)| 审阅者的标识符。 支持 `$select`。 只读。|
|reviewedDateTime|DateTimeOffset| 发生审阅决定时的时间戳。 支持 `$select`。 只读。|
|principalResourceMembership|[decisionItemPrincipalResourceMembership](../resources/decisionItemPrincipalResourceMembership.md)| 访问评审中的每个决策项都表示主体对资源的成员身份。 此属性提供成员身份的详细信息。 例如，主体是否具有对资源的直接访问权限或间接访问权限。 支持 `$select`。 只读。|


## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| 实例 |[accessReviewInstance](accessreviewinstance.md) | 与每个决策完全关联了一个 accessReviewInstance。 实例是决策项的父级，表示对决策进行的访问评审的重复性。 |
| insights |[governanceInsight](governanceinsight.md) 集合 | 见解是向审阅者建议是批准还是拒绝决定。 可以有多个见解与 **accessReviewInstanceDecisionItem** 相关联。 |


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
  "principalResourceMembership": {
    "@odata.type": "microsoft.graph.decisionItemPrincipalResourceMembership"
  },
  "resourceLink": "String"
}
```
