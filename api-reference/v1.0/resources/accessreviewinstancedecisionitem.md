---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示对 accessReviewInstance 的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 782c391a9149af2527401119b100d720918b3a7e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031045"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>accessReviewInstanceDecisionItem 资源类型

命名空间：microsoft.graph

表示有关审阅 [实例](accessreviewsv2-root.md) 的 Azure AD 访问评审决定。 此决定表示确定标识对给定 [accessReviewInstance](accessreviewinstance.md)的资源的访问权限。

每个决策项都是基于父 [accessReviewInstance 系统生成的](accessreviewinstance.md)。

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|获取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象及其属性的列表。|
|[获取 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。|
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|更新 [accessReviewInstanceDecisionItem 对象](../resources/accessreviewinstancedecisionitem.md) 的属性。|
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|返回调用用户作为审阅者的决策项。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accessReviewId|String|accessReviewInstance 父项的标识符。 支持 `$select`。 只读。|
|appliedBy|[userIdentity](../resources/useridentity.md)|应用了该决策的用户的标识符。 只读。|
|appliedDateTime|DateTimeOffset|应用批准决策的时间戳。 DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。  支持 `$select`。 只读。|
|applyResult|String|应用决策的结果。 可能的值 `New` `AppliedSuccessfully` ：、、 `AppliedWithUnknownFailure` `AppliedSuccessfullyButObjectNotFound` 和 `ApplyNotSupported` 。 仅 `$select` `$orderby` 支持 、 (`$filter` 和 `eq`) 。 只读。|
|decision|String|评价的结果。 可能的值 `Approve` `Deny` ：、、 `NotReviewed` 或 `DontKnow` 。 仅 `$select` `$orderby` 支持 、 (`$filter` 和 `eq`) 。 |
|id|String| 决策的标识符。 继承自 [实体](../resources/entity.md)。 支持 `$select`。 只读。|
|justification|String|审阅者做出决策时留下的理由。|
|principal|[identity](../resources/identity.md)|访问评审中的每个决策项表示主体对资源的访问权限。 此属性表示主体的详细信息。 例如，如果某个决策项表示用户"Bob"对组"Sales"的访问权限 - 主体为"Bob"，资源为"Sales"。 主体可以是两种类型 - userIdentity 和 servicePrincipalIdentity。 支持 `$select`。 只读。|
|principalLink|String|指向主体对象的链接。 例如，`https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`。 只读。|
|建议|String|针对基于上次交互式登录租户的审批决策的系统生成的建议。 如果登录是自审查开始起 30 天内，建议批准。 如果登录自审查开始超过 30 天，建议拒绝。 否则，建议不可用。 可能的值 `Approve` ：、 `Deny` 或 `NoInfoAvailable` 。 仅 `$select` `$orderby` 支持 、 (`$filter` 和 `eq`) 。 只读。|
|resource|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|访问评审中的每个决策项表示主体对资源的访问权限。 此属性表示资源的详细信息。 例如，如果决策项表示用户"Bob"对组"销售"的访问权限 - 主体为 Bob，资源为"Sales"。 资源可以是多种类型的。 请参阅 [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)。 只读。|
|resourceLink|String|指向资源的链接。 例如 https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8 ，""。 支持 `$select`。 只读。|
|reviewedBy|[userIdentity](../resources/useridentity.md)| 审阅者的标识符。 支持 `$select`。 只读。|
|reviewedDateTime|DateTimeOffset| 发生审阅决策的时间戳。 支持 `$select`。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
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
