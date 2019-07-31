---
title: accessReview 资源类型
description: '在 Azure AD access 评论功能中, `accessReview`表示访问评审。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4205f0995b0e8c71c8e01991837b4d721ecfaaf7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974561"
---
# <a name="accessreview-resource-type"></a>accessReview 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [access 评论](accessreviews-root.md)功能中, `accessReview`表示访问评审。  


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   获取具有特定 id 的访问评审。 |
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新的 accessReview。 |
|[删除 accessReview](../api/accessreview-delete.md) | 无。   | 删除 accessReview。 |
|[更新 accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | 更新 accessReview。 |
|[列出 accessReview 审阅者](../api/accessreview-listreviewers.md) |      [userIdentity](useridentity.md)集合| 获取 accessReview 的审阅者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) |      无。   |   向 accessReview 添加审阅者。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。  |   从 accessReview 中删除审阅者。 |
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)集合| 获取 accessReview 的决策。|
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)集合| 作为审阅者, 请 accessReview 的决策。|
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) |        无。   |   向 accessReview 的审阅者发送提醒。 |
|[停止 accessReview](../api/accessreview-stop.md) |     无。   |   停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) |     无。   |   在进行中的 accessReview 中重置决策。|
|[应用 accessReview 决策](../api/accessreview-apply.md) |     无。   |   从已完成的 accessReview 应用决策。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | 用于访问评审的功能分配的唯一标识符。 |
| `displayName`             |`String`                                                        | 访问审阅名称。 创建时为必需项。 |
| `startDateTime`           |`DateTimeOffset`                                                | 计划开始评审时的日期时间。  这可能是将来的日期。  创建时为必需项。 |
| `endDateTime`             |`DateTimeOffset`                                                | 计划结束评审时的日期/时间。 此时间必须至少为一个晚于开始日期的一天。  创建时为必需项。 |
| `status`                  |`String`                                                        | 此只读字段指定 accessReview 的状态。 典型状态包括`Initializing`、 `NotStarted`、 `Starting``InProgress` `Completing` `Completed` `AutoReviewed`、、、、和。 `AutoReviewing` |
| `description`             |`String`                                                        | 由 access 评审创建者提供的说明, 用于向审阅者显示。 |
| `businessFlowTemplateId`  |`String`                                                        | 业务流模板标识符。 创建时为必需项。 |
| `reviewerType`            |`String`                                                        | 目标对象的审阅者的关系类型, 一个`self` `delegated`或。 `entityOwners` 创建时为必需项。 | 
| `createdBy`               |[userIdentity](useridentity.md)                                 | 创建此评审的用户。 |
| `reviewedEntity`          |[identity](identity.md)                                      | 访问权检查其访问权限分配的对象。 此组可以是查看组中用户的成员身份的组, 也可以是用于查看对应用程序的用户分配的应用程序。 创建时为必需项。 | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | AccessReview 的设置, 请参阅下面的类型定义。 |



## <a name="relationships"></a>关系




| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `reviewers`               |[userIdentity](useridentity.md)集合                     | 访问评审的审阅者的集合 (如果 access 评审 reviewerType 的类型`delegate`为)。 |
| `decisions`               |[accessReviewDecision](accessreviewdecision.md)集合 | 此访问评审的决策集合。 |
| `myDecisions`             |[accessReviewDecision](accessreviewdecision.md)集合 | 如果呼叫者是审阅者, 则为呼叫者做出决策的集合。 |
| `instances`               |[accessReview](accessreview.md)集合         | 如果此对象是定期访问审核, 则 access 的集合将审阅过去、现在和将来的实例。 |

对象中是否存在这些关系, 取决于该对象是一次性访问评审、定期访问评审的系列, 还是定期访问评审的实例。

| 应用场景 | 是否有审阅者？ | 是否有决策和 myDecisions？ | 有实例吗？ |
|:---------|:---------------|:---------------|:---------------|
|一次性访问审核|是 | 是, 启动后 | 否 |
| 定期访问审核 | 是 | 否 | 是 |
| 定期访问审核实例 | 是 | 是, 启动后 | 否 |

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
 "createdBy": "microsoft.graph.userIdentity",
 "reviewedEntity": "microsoft.graph.identity",
 "settings": "microsoft.graph.accessReviewSettings",
 "reviewers": "Collection(microsoft.graph.userIdentity)"
}

```

## <a name="the-accessreviewsettings-type"></a>AccessReviewSettings 类型

在`accessReviewSettings`创建访问评审时提供其他设置, 以在启动访问评审时控制功能行为。  此类型具有以下属性: 

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | 指示是否已启用向审阅者发送邮件和审阅创建者的标志。                |
| `remindersEnabled`|`Boolean`       | 指示是否启用了向审阅者发送提醒电子邮件的标志。       |
| `justificationRequiredOnApproval`|`Boolean` | 指示审阅 access 时是否需要审阅者提供理由的标志。|
| `activityDurationInDays`|`Int64` | 向审阅者显示的用户活动的天数。 |
| `autoReviewEnabled`|`Boolean` | 用于指示功能是否应在审阅者未提供且与自动应用一起使用时设置决策的标志。 |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | 有关功能应如何设置审阅决定 (用于自动应用) 的详细设置, 请参阅下文所述。 |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | 定期的详细设置, 如下所述。 |
| `autoApplyReviewResultsEnabled`|`Boolean` | 用于指示是否启用自动更改目标对象访问资源的自动应用功能的标志。  如果未启用, 则用户必须在评审完成后应用访问评审。 |
| `accessRecommendationsEnabled`|`Boolean` | 指示是否已启用向审阅者显示建议的标志。 |

## <a name="the-autoreviewsettings-type"></a>AutoReviewSettings 类型

`autoReviewSettings`嵌入访问审阅设置中, 并指定访问评审完成时的功能行为。  类型具有一个属性`notReviewedResult`。

| 属性                     | 类型     | 说明                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | 必须为 `Approve`、`Deny` 或 `Recommendation` 的其中一个。 |


## <a name="the-accessreviewrecurrencesettings-type"></a>AccessReviewRecurrenceSettings 类型

嵌入`accessReviewRecurrenceSettings`到 access 评审设置中, 并指定以固定间隔重复进行访问评审。  此类型具有以下属性:

| 属性                     | 类型                                                                                                          | 说明 |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | 定期`onetime`间隔, 必须为、 `weekly`、 `monthly` `quarterly`、或`annual`的其中一个。                                                                   |
| `recurrenceEndType`|`String` | 重复周期的结束方式。 如果是`Never`, 则不会出现定期系列的显式结束。 如果是`endBy`, 则重复周期将在特定日期结束。 如果是`occurrences`, 则在审阅的实例完成`recurrentCount`后, 该系列将结束。 |
| `durationInDays`|`Int32`     | 定期的持续时间 (以天为单位)。                                                                              |
| `recurrenceCount`|`Int32`    | 如果值`recurrenceEndType`为, 则为`occurrences`定期计数, 否则为0。                                                        |


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
