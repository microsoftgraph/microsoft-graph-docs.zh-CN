---
title: accessReview 资源类型
description: '在 Azure AD 访问评审功能中， `accessReview` 表示访问评审。  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: da155d49eedf03cdc935eeefc6b6808847176a41
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292712"
---
# <a name="accessreview-resource-type"></a>accessReview 资源类型

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
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) | [accessReviewDecision](accessreviewdecision.md) 集合 | 作为审阅者，获取我关于 accessReview 的决定。 |
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) | 无。 | 向 accessReview 的审阅者发送提醒。 |
|[Stop accessReview](../api/accessreview-stop.md) | 无。 | 停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) | 无。   |   重置正在进行中的 accessReview 中的决策。 |
|[应用 accessReview 决策](../api/accessreview-apply.md) | 无。 | 从已完成的 accessReview 应用决策。 |

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:-------- |:---- |:----------- |
| id | String | 访问评审的功能分配的唯一标识符。 |
| displayName | String | 访问评审名称。 创建时为必需项。 |
| startDateTime | DateTimeOffset | 计划开始审阅的日期/时间。  这可能是将来的日期。  创建时为必需项。 |
| endDateTime | DateTimeOffset | 计划结束审阅的日期/时间。 这必须至少比开始日期晚一天。  创建时为必需项。 |
| status | String | 此只读字段指定 accessReview 的状态。 典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。 |
| description | String | 访问评审创建者提供的说明，向审阅者显示。 |
| businessFlowTemplateId | String | 业务流程模板标识符。 创建时为必需项。  此值区分大小写。 |
| reviewerType | String | 审阅者与目标对象的关系类型，其中一个 `self` 或 `delegated` `entityOwners` 。 创建时为必需项。 | 
| createdBy | [userIdentity](useridentity.md) | 创建此评价的用户。 |
| reviewedEntity | [identity](identity.md) | 访问评审正在审阅其访问权限分配的对象。 此组可以是审阅组中用户成员身份的组，或者是查看用户到应用程序的分配的应用。 创建时为必需项。 | 
| settings | [accessReviewSettings](accessreviewsettings.md) | accessReview 的设置，请参阅下面的类型定义。 |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:------------ |:---- |:----------- |
| 审阅者 | [userIdentity](useridentity.md) 集合 | 访问评审审阅者的集合，如果访问审阅审阅者Type 的类型 `delegated` 。 |
| 决策 | [accessReviewDecision](accessreviewdecision.md) 集合 | 此访问评审的决策集合。 |
| myDecisions | [accessReviewDecision](accessreviewdecision.md) 集合 | 呼叫者的决策集合（如果呼叫者是审阅者）。 |
| instances | [accessReview](accessreview.md) 集合 | 如果此对象是定期访问评审，则访问评审实例的集合将过去、现在和未来。 |

这些关系是否存在于对象上取决于对象是一次性访问评审、定期访问评审系列还是定期访问评审的实例。

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


