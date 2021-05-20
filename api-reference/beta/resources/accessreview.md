---
title: accessReview 资源类型
description: '在 Azure AD 访问评审功能中， `accessReview` 表示访问评审。  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 75f844a165b8e5603f2d423a9d0a7aef17ab9186
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579278"
---
# <a name="accessreview-resource-type-deprecated"></a>accessReview 资源类型 (已弃) 

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
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) | 无。    |   将审阅者添加到 accessReview。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。 |    从 accessReview 中删除审阅者。 |
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) | [accessReviewDecision](accessreviewdecision.md) 集合 | 获取 accessReview 的决策。 |
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) | [accessReviewDecision](accessreviewdecision.md) 集合 | 作为审阅者，获取我在 accessReview 上的决定。 |
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) | 无。 | 向 accessReview 的审阅者发送提醒。 |
|[Stop accessReview](../api/accessreview-stop.md) | 无。 | 停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) | 无。   |   重置进行中的 accessReview 中的决策。 |
|[应用 accessReview 决策](../api/accessreview-apply.md) | 无。 | 从已完成的 accessReview 应用决策。 |

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:-------- |:---- |:----------- |
| id | String | 访问评审的功能分配的唯一标识符。 |
| displayName | String | 访问评审名称。 创建时为必需项。 |
| startDateTime | DateTimeOffset | 计划开始审阅的 DateTime。  这可以是将来的日期。  创建时为必需项。 |
| endDateTime | DateTimeOffset | 计划结束审阅的 DateTime。 这必须至少比开始日期晚一天。  创建时为必需项。 |
| 状态 | String | 此只读字段指定 accessReview 的状态。 典型状态包括 `Initializing` `NotStarted` `Starting` `InProgress` 、、、、、、 `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。 |
| 说明 | String | 由访问评审创建者提供的向审阅者显示的说明。 |
| businessFlowTemplateId | String | 业务流程模板标识符。 创建时为必需项。  此值区分大小写。 |
| reviewerType | String | 审阅者与目标对象的关系类型，为 或 `self` 之 `delegated` 一 `entityOwners` 。 创建时为必需项。 | 
| createdBy | [userIdentity](useridentity.md) | 创建此评价的用户。 |
| reviewedEntity | [identity](identity.md) | 访问评审正在审阅其访问权限分配的对象。 它可以是查看组中用户的成员身份的组，或者是查看用户到应用程序的分配的应用。 创建时为必需项。 | 
| settings | [accessReviewSettings](accessreviewsettings.md) | accessReview 的设置，请参阅下面的类型定义。 |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:------------ |:---- |:----------- |
| reviewers | [userIdentity](useridentity.md) 集合 | 访问评审的审阅者集合（如果访问评审审阅者类型为 `delegated` ）。 |
| 决策 | [accessReviewDecision](accessreviewdecision.md) 集合 | 此访问评审的决策集合。 |
| myDecisions | [accessReviewDecision](accessreviewdecision.md) 集合 | 调用方的决策集合（如果呼叫者是审阅者）。 |
| instances | [accessReview](accessreview.md) 集合 | 如果此对象是定期访问评审，访问评审实例的集合将过去、现在和将来发生。 |

这些关系是否存在于对象上取决于对象是一次性访问评审、一系列定期访问评审还是定期访问评审的实例。

| 应用场景 | 有审阅者吗？ | 有决策和 myDecisions 吗？ | 具有实例？ |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| 一次访问评审 | 是 | 是，一旦启动 | 否 |
| 定期访问评审 | 是 | 否 | 是 |
| 定期访问评审的实例 | 是 | 是，一旦启动 | 否 |

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


