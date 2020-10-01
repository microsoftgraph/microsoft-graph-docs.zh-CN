---
title: accessReview 资源类型
description: '在 Azure AD access 评论功能中， `accessReview` 表示访问评审。  '
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a63291d9cefb1b6a0c249b09a95430303b3597d
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330164"
---
# <a name="accessreview-resource-type"></a>accessReview 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD [访问评审](accessreviews-root.md)。  

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviews](../api/accessreview-list.md) | [accessReview](accessreview.md) 集合 | 列出 businessFlowTemplate 的 accessReviews。 |
|[获取 accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   获取具有特定 id 的访问评审。 |
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新的 accessReview。 |
|[更新 accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | 更新 accessReview。 |
|[删除 accessReview](../api/accessreview-delete.md) | 无。   | 删除 accessReview。 |
|[列出 accessReview 审阅者](../api/accessreview-listreviewers.md) | [userIdentity](useridentity.md) 集合|  获取 accessReview 的审阅者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) | 无。    |   向 accessReview 添加审阅者。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。 |    从 accessReview 中删除审阅者。 |
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) | [accessReviewDecision](accessreviewdecision.md) 集合 | 获取 accessReview 的决策。 |
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) | [accessReviewDecision](accessreviewdecision.md) 集合 | 作为审阅者，请 accessReview 的决策。 |
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) | 无。 | 向 accessReview 的审阅者发送提醒。 |
|[停止 accessReview](../api/accessreview-stop.md) | 无。 | 停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) | 无。   |   在进行中的 accessReview 中重置决策。 |
|[应用 accessReview 决策](../api/accessreview-apply.md) | 无。 | 从已完成的 accessReview 应用决策。 |

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:-------- |:---- |:----------- |
| id | 字符串 | 用于访问评审的功能分配的唯一标识符。 |
| displayName | 字符串 | 访问审阅名称。 创建时为必需项。 |
| startDateTime | DateTimeOffset | 计划开始评审时的日期时间。  这可能是将来的日期。  创建时为必需项。 |
| endDateTime | DateTimeOffset | 计划结束评审时的日期/时间。 此时间必须至少为一个晚于开始日期的一天。  创建时为必需项。 |
| 状态 | 字符串 | 此只读字段指定 accessReview 的状态。 典型状态包括、、、、、、 `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。 |
| description | 字符串 | 由 access 评审创建者提供的说明，用于向审阅者显示。 |
| businessFlowTemplateId | 字符串 | 业务流模板标识符。 创建时为必需项。  此值区分大小写。 |
| reviewerType | 字符串 | 目标对象的审阅者的关系类型，一个 `self` `delegated` 或 `entityOwners` 。 创建时为必需项。 | 
| createdBy | [userIdentity](useridentity.md) | 创建此评审的用户。 |
| reviewedEntity | [identity](identity.md) | 访问权检查其访问权限分配的对象。 此组可以是查看组中用户的成员身份的组，也可以是用于查看对应用程序的用户分配的应用程序。 创建时为必需项。 | 
| settings | [accessReviewSettings](accessreviewsettings.md) | AccessReview 的设置，请参阅下面的类型定义。 |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
|:------------ |:---- |:----------- |
| 审批 | [userIdentity](useridentity.md) 集合 | 访问评审的审阅者的集合（如果 access 评审 reviewerType 的类型为） `delegated` 。 |
| 针对 | [accessReviewDecision](accessreviewdecision.md) 集合 | 此访问评审的决策集合。 |
| myDecisions | [accessReviewDecision](accessreviewdecision.md) 集合 | 如果呼叫者是审阅者，则为呼叫者做出决策的集合。 |
| instances | [accessReview](accessreview.md) 集合 | 如果此对象是定期访问审核，则 access 的集合将审阅过去、现在和将来的实例。 |

对象中是否存在这些关系，取决于该对象是一次性访问评审、定期访问评审的系列，还是定期访问评审的实例。

| 方案 | 是否有审阅者？ | 是否有决策和 myDecisions？ | 有实例吗？ |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| 一次性访问审核 | 是 | 是，启动后 | 否 |
| 定期访问审核 | 是 | 否 | 是 |
| 定期访问审核实例 | 是 | 是，启动后 | 否 |

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


