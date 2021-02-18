---
title: accessReviewDecision 资源类型
description: accessReviewDecision 表示对特定实体的访问的 Azure AD 访问评审决定。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 52d4e2a262d3a90010cc0e254e11f2d723a5e550
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292691"
---
# <a name="accessreviewdecision-resource-type"></a>accessReviewDecision 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

在 Azure AD [访问评审](accessreviews-root.md) 功能中，表示特定实体访问权限的 `accessReviewDecision` Azure AD 访问评审决定。  在访问评审或定期访问评审的实例中，每个审阅的用户 `accessReviewDecision` 有一个。  例如，如果一个组有两个来宾和一个非来宾作为成员，并且对该组执行来宾的访问评审，则有两个访问评审决策对象。  如果审阅者更改其决定，或者另一个审阅者替代他们，则更新 `accessReviewDecision` 。


## <a name="methods"></a>方法

无。  当访问评审初始化时，此功能会自动创建此类型的对象，并且无法删除。  可以使用决策和决定关系从访问评审[中检索](../api/accessreview-listmydecisions.md)它们[](../api/accessreview-listdecisions.md)。

## <a name="properties"></a>属性

此表说明了此类型对象的基本属性。 

| 属性                        | 类型                         | 说明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | 访问评审中决策的 ID。                                                                                     |
| `accessReviewId`                |`String`                      | 访问评审的功能生成 ID。                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| 审阅者的标识。 如果将建议用作审阅，则 userPrincipalName 为空。                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | 提供了此访问权限的最新审阅日期和时间。                                                                         |
| `reviewResult`                  |`String`                      | 审阅的结果，其中一个 `NotReviewed` ， `Deny` 或 `DontKnow` `Approve` 。                                                                                    |
| `justification`                 |`String`                      | 审阅者的业务理由（如果提供）。                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| 审阅完成后，如果手动应用了结果，则应用该决定的用户的用户标识。 如果自动应用评价，则 userPrincipalName 为空。                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | 应用审阅决策的日期和时间。                                                          |
| `applyResult`                   |`String`                      | 应用决策的结果，其中一个 ， `NotApplied` `Success` 或 `Failed` `NotFound` `NotSupported` 。                      |
| `accessRecommendation`          |`String`                      | 向审阅者显示的功能生成的建议，其中一 `Approve` 个或 `Deny` `NotAvailable` 。 |


此外，根据拥有已对象类型访问权限的对象的属性，可能会存在其他属性。  例如，如果访问评审决策是特定用户的组成员身份或应用程序访问权限，则可能会删除其访问权限的用户通过以下属性进行标识：

| 属性                        | 类型                         | 说明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | 已审阅其访问权限的用户的 ID。                                                                                    |
| `userDisplayName`                            |`String`                      | 已显示名称访问权限的用户的用户名。                                                                                     |
| `userPrincipalName`                            |`String`                      | 已审阅其访问权限的用户的用户主体名称。                                                                                     |



## <a name="relationships"></a>关系

无。  可以使用[accessReview](accessreview.md)对象的决策和决定关系从访问评审[](../api/accessreview-listdecisions.md)中检索[](../api/accessreview-listmydecisions.md)此类型的对象。

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md) 集合| 获取 accessReview 的决策。|
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md) 集合| 作为审阅者，获取我关于 accessReview 的决定。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


