---
title: 'accessReviewDecision 资源类型 (已弃用) '
description: accessReviewDecision 表示对特定实体的访问权限的 Azure AD 访问评审决策。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb85de238c852d1e4e397cd142e7bb4863e3f2a1
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820796"
---
# <a name="accessreviewdecision-resource-type-deprecated"></a>accessReviewDecision 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

在 Azure AD [访问评审](accessreviews-root.md) 功能中，表示 `accessReviewDecision` 特定实体访问权限的 Azure AD 访问评审决策。  在访问评审或定期访问评审的实例中，每个已审阅的用户都有一个 `accessReviewDecision` 。  例如，如果一个组有两个来宾和一个非来宾作为成员，并且对该组执行来宾的访问评审，则将有两个访问评审决策对象。  如果审阅者更改了其决定，或者另一个审阅者替代了这些决定，则 `accessReviewDecision` 会更新。


## <a name="methods"></a>方法

无。  当访问评审初始化且无法删除时，该功能会自动创建此类型的对象。  可以使用 [决策](../api/accessreview-listdecisions.md) 和 [mydecisions](../api/accessreview-listmydecisions.md) 关系从访问评审中检索它们。

## <a name="properties"></a>属性

下表说明了此类型的对象的基本属性。 

| 属性                        | 类型                         | 说明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | 访问评审中决策的 ID。                                                                                     |
| `accessReviewId`                |`String`                      | 访问评审的功能生成 ID。                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| 审阅者的身份。 如果建议用作评审，则 userPrincipalName 为空。                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | 提供此访问权限的最新评审的日期和时间。                                                                         |
| `reviewResult`                  |`String`                      | 审查的结果，其中之`NotReviewed`一，`Deny``DontKnow`或 `Approve`。                                                                                    |
| `justification`                 |`String`                      | 审阅者的业务理由（如果提供）。                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| 评审完成后，如果手动应用了结果，则为应用该决定的用户的用户标识。 如果自动应用了评审，则 userPrincipalName 为空。                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | 应用审查决定的日期和时间。                                                          |
| `applyResult`                   |`String`                      | 应用决定的结果，其中之 `NotApplied`一， `Success`， `Failed`或 `NotFound` `NotSupported`。                      |
| `accessRecommendation`          |`String`                      | 向审阅者显示的功能生成的建议，其中 `Approve`一个或 `Deny` `NotAvailable`。 |


此外，可能存在其他属性，具体取决于具有已确定访问权限的对象的对象类型。  例如，如果访问评审决策是特定用户的组成员身份或应用程序访问权限，则可能会删除其访问权限的用户通过以下属性进行标识：

| 属性                        | 类型                         | 说明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | 已审阅其访问权限的用户的 ID。                                                                                    |
| `userDisplayName`                            |`String`                      | 已审阅其访问权限的用户的显示名称。                                                                                     |
| `userPrincipalName`                            |`String`                      | 已审阅其访问权限的用户的用户主体名称。                                                                                     |



## <a name="relationships"></a>关系

无。  可以使用 [accessReview](accessreview.md) 对象的[决策](../api/accessreview-listdecisions.md)和 [mydecisions](../api/accessreview-listmydecisions.md) 关系从访问评审中检索此类型的对象。

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md) 集合| 获取 accessReview 的决策。|
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md) 集合| 作为审阅者，获取 AccessReview 的决策。|

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


