---
title: accessReviewDecision 资源类型
description: 在 Azure AD 中访问审阅功能，`accessReviewDecision`代表 Azure AD 访问检查决策的特定实体的访问。  内访问审阅或定期访问回顾实例，还有一`accessReviewDecision`每个已审阅的用户。  例如，如果组具有两个来宾和一个非访客成员，作为来宾访问审阅执行为该组，然后将两个访问审阅决策对象。  如果审阅者更改其决策，或其他审阅者重写它们，则`accessReviewDecision`更新。
ms.openlocfilehash: 8eebbc6d99e6197da68731fe3a39d3b47e743573
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049515"
---
# <a name="accessreviewdecision-resource-type"></a>accessReviewDecision 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](accessreviews-root.md)功能中，`accessReviewDecision`代表 Azure AD 访问检查决策的特定实体的访问。  内访问审阅或定期访问回顾实例，还有一`accessReviewDecision`每个已审阅的用户。  例如，如果组具有两个来宾和一个非访客成员，作为来宾访问审阅执行为该组，然后将两个访问审阅决策对象。  如果审阅者更改其决策，或其他审阅者重写它们，则`accessReviewDecision`更新。


## <a name="methods"></a>方法

无。  访问查看初始化，并不能删除时，此类型的对象会自动创建功能。  它们可以使用的[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系访问查看从检索。

## <a name="properties"></a>属性

下表说明了此类型的对象的基本属性。 

| 属性                        | 类型                         | 说明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | 内访问审阅决策的 id。                                                                                     |
| `accessReviewId`                |`String`                      | 功能生成访问审阅的 id。                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| 审阅者的标识。                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | 提供的日期和时间，此最新的审阅访问权限。                                                                         |
| `reviewResult`                  |`String`                      | 审阅结果。                                                                                    |
| `justification`                 |`String`                      | 审阅者的业务理由，如果提供。                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| 审阅完成后，如果已手动应用的结果，应用决策的用户的用户标识。                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | 日期和时间时应用的审阅决策。                                                          |
| `applyResult`                   |`String`                      | 应用的决策，之一的结果`NotApplied`， `Success`， `Failed`，`NotFound`或`NotSupported`。                      |
| `accessRecommendation`          |`String`                      | 显示给审阅者，之一功能-生成建议`Approve`，`Deny`或`NotAvailable`。 |


此外，其他属性可能会出现根据拥有已决定的访问权限的对象的对象类型。  例如，如果访问检查决策为特定用户的组成员身份或应用程序访问，可能要让他们要删除的访问权限的用户被标识通过这些属性：

| 属性                        | 类型                         | 说明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | 已检查其访问权限的用户的 id。                                                                                    |
| `userDisplayName`                            |`String`                      | 已检查其访问权限的用户的显示名称。                                                                                     |
| `userPrincipalName`                            |`String`                      | 已检查其访问权限的用户的用户主体名称。                                                                                     |



## <a name="relationships"></a>Relationships

无。  可以使用[accessReview](accessreview.md)对象的[决策](../api/accessreview-listdecisions.md)和[mydecisions](../api/accessreview-listmydecisions.md)关系访问查看从检索此类型的对象。

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)集合| 获取 accessReview 的决策。|
|[列出我 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)集合| 审阅者，以获取 accessReview 我决策。|

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

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->