---
title: '已弃用的 accessReview 资源类型 () '
description: '在 Azure AD 访问评审功能中，表示 `accessReview` 访问评审。  '
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 353dfec671a400e87f613779f9d50a6e68845a34
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819473"
---
# <a name="accessreview-resource-type-deprecated"></a>已弃用的 accessReview 资源类型 () 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

表示 Azure AD [访问评审](accessreviews-root.md)。  

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviews](../api/accessreview-list.md) | [accessReview](accessreview.md) 集合 | 列出 businessFlowTemplate 的 accessReviews。 |
|[获取 accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   获取具有特定 ID 的访问评审。 |
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新的 accessReview。 |
|[更新 accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | 更新 accessReview。 |
|[删除 accessReview](../api/accessreview-delete.md) | 无。   | 删除 accessReview。 |
|[列出 accessReview 审阅者](../api/accessreview-listreviewers.md) | [userIdentity](useridentity.md) 集合|  获取 accessReview 的审阅者。 |
|[添加 accessReview 审阅器](../api/accessreview-addreviewer.md) | 无。    |   将审阅者添加到 accessReview。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。 |    从 accessReview 中删除审阅者。 |
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) | [accessReviewDecision](accessreviewdecision.md) 集合 | 获取 accessReview 的决策。 |
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) | [accessReviewDecision](accessreviewdecision.md) 集合 | 作为审阅者，获取 AccessReview 的决策。 |
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) | 无。 | 向 accessReview 的审阅者发送提醒。 |
|[停止 accessReview](../api/accessreview-stop.md) | 无。 | 停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) | 无。   |   在正在进行的 accessReview 中重置决策。 |
|[应用 accessReview 决策](../api/accessreview-apply.md) | 无。 | 应用已完成的 accessReview 中的决策。 |

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:-------- |:---- |:----------- |
| id | String | 访问评审的功能分配的唯一标识符。 |
| displayName | String | 访问评审名称。 创建时为必需项。 |
| startDateTime | DateTimeOffset | 计划开始评审时的 DateTime。  这可能是将来的日期。  创建时为必需项。 |
| endDateTime | DateTimeOffset | 计划结束评审时的 DateTime。 这必须至少比开始日期晚一天。  创建时为必需项。 |
| status | String | 此只读字段指定 accessReview 的状态。 典型的状态包括`Initializing`，，`NotStarted`，`Starting``InProgress`，`Completing``Completed`，`AutoReviewing`和 `AutoReviewed`。 |
| description | String | 访问评审创建者提供的说明，以向审阅者显示。 |
| businessFlowTemplateId | String | 业务流模板标识符。 创建时为必需项。  此值区分大小写。 |
| reviewerType | String | 审阅者与目标对象的关系类型，其中 `self`一个或 `delegated` `entityOwners`。 创建时为必需项。 | 
| createdBy | [userIdentity](useridentity.md) | 创建此评审的用户。 |
| reviewedEntity | [identity](identity.md) | 访问评审正在审查访问权限分配的对象。 这可以是用于评审组中用户成员身份的组，也可以是用于评审用户分配到应用程序的应用的组。 创建时为必需项。 | 
| settings | [accessReviewSettings](accessreviewsettings.md) | accessReview 的设置，请参阅下面的类型定义。 |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:------------ |:---- |:----------- |
| 评论家 | [userIdentity](useridentity.md) 集合 | 访问评审评审的审阅者集合（如果访问评审审阅者类型） `delegated`。 |
| 决定 | [accessReviewDecision](accessreviewdecision.md) 集合 | 此访问评审的决策集合。 |
| myDecisions | [accessReviewDecision](accessreviewdecision.md) 集合 | 如果调用方是审阅者，则为调用方的决策集合。 |
| 实例 | [accessReview](accessreview.md) 集合 | 如果此对象是定期访问评审，则访问评审实例的集合包括过去、现在和将来。 |

这些关系是否存在于对象上，取决于对象是一次性访问评审、定期访问评审的系列，还是定期访问评审的实例。

| 应用场景 | 审阅者有吗？ | 是否具有决策和 myDecisions？ | 有实例吗？ |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| 一次性访问评审 | 是 | 是的，一旦启动 | 否 |
| 定期访问评审 | 是 | 否 | 是 |
| 定期访问评审的实例 | 是 | 是的，一旦启动 | 否 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReview"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "description": "string",
 "businessFlowTemplateId": "string (identifier)",
 "reviewerType": "string",
 "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
 "reviewedEntity": {"@odata.type": "microsoft.graph.identity"},
 "settings": {"@odata.type": "microsoft.graph.accessReviewSettings"},
 "reviewers": [{"@odata.type": "microsoft.graph.userIdentity"}]
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


