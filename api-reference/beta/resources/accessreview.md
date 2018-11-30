---
title: accessReview 资源类型
description: '在 Azure AD 中访问审阅功能，`accessReview`代表访问审阅。  '
ms.openlocfilehash: 1ad1edc9d3909ea2648f2644e1ba5438ce981c2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042535"
---
# <a name="accessreview-resource-type"></a>accessReview 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](accessreviews-root.md)功能中，`accessReview`代表访问审阅。  


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   获取与特定 id 访问审阅。 |
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新 accessReview。 |
|[删除 accessReview](../api/accessreview-delete.md) | 无。   | 删除 accessReview。 |
|[更新 accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | 更新 accessReview。 |
|[列表 accessReview 审阅者](../api/accessreview-listreviewers.md) |      [userIdentity](useridentity.md)集合| 要获取 accessReview 审阅的者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) |      无。   |   将审阅者添加到 accessReview。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。  |   删除 accessReview 审阅者。 |
|[列表 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)集合| 获取 accessReview 的决策。|
|[列出我 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)集合| 审阅者，以获取 accessReview 我决策。|
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) |        无。   |   向审阅者的 accessReview 发送提醒。 |
|[停止 accessReview](../api/accessreview-stop.md) |     无。   |   停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) |     无。   |   重置正在进行 accessReview 决策。|
|[应用 accessReview 决策](../api/accessreview-apply.md) |     无。   |   应用已完成 accessReview 从的决策。|

## <a name="permissions"></a>Permissions

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.Read.All AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | 功能分配的唯一标识符访问审阅。 |
| `displayName`             |`String`                                                        | 访问审阅名称。 所需在创建。 |
| `startDateTime`           |`DateTimeOffset`                                                | 审阅安排在启动时 DateTime。  这可能是在将来的日期。  所需在创建。 |
| `endDateTime`             |`DateTimeOffset`                                                | 审阅安排结束时 DateTime。 这必须是至少一个日期晚于开始日期。  所需在创建。 |
| `status`                  |`String`                                                        | 此只读字段指定 accessReview 的当前状态。 典型的状态包括`Initializing`， `NotStarted`， `Starting`，`InProgress`， `Completing`， `Completed`， `AutoReviewing`，和`AutoReviewed`。 |
| `description`             |`String`                                                        | 访问审阅创建者提供，向审阅者显示说明。 |
| `businessFlowTemplateId`  |`String`                                                        | 业务流程模板标识符。 所需在创建。 |
| `reviewerType`            |`String`                                                        | 对目标对象，之一的审阅者的关系类型`self`，`delegate`或`entityOwners`。 所需在创建。 | 
| `createdBy`               |[userIdentity](useridentity.md)                                 | 创建此审查的用户。 |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | 访问权限分配，如用户迁移到一组的成员身份或分配用户迁移到应用程序的访问其审阅的对象。 所需在创建。 | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | AccessReview 的设置，，请参阅下面的类型定义。 |



## <a name="relationships"></a>Relationships




| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
| `reviewers`               |[userIdentity](useridentity.md)集合                     | 访问审阅，如果访问审阅 reviewerType 的类型的审阅者的集合`delegate`。 |
| `decisions`               |[accessReviewDecision](accessreviewdecision.md)集合 | 此访问审查的决策的集合。 |
| `myDecisions`             |[accessReviewDecision](accessreviewdecision.md)集合 | 呼叫者，呼叫者是否审阅者的决策的集合。 |
| `instances`               |[accessReview](accessreview.md)集合         | 访问评论一实例过去、 存在和未来，如果此对象是定期访问回顾。 |

是否存在对某个对象的关系，依赖于对象是否是一次性访问回顾、 的一系列定期访问审阅或定期访问回顾的实例。

| 应用场景 | 有审阅者？ | 具有决策和 myDecisions？ | 具有实例？ |
|:---------|:---------------|:---------------|:---------------|
|一次性访问审阅|是 | 是，一次启动 | 否 |
| 定期访问审阅 | 是 | 否 | 是 |
| 定期访问回顾的实例 | 是 | 是，一次启动 | 否 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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

`accessReviewSettings`创建访问检查，以控制时开始访问审阅功能行为时提供其他设置。  此类型具有以下属性： 

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | 用于指示是否启用将邮件发送给审阅者和审阅创建者的标志。                |
| `remindersEnabled`|`Boolean`       | 用于指示是否启用发送给审阅者的提醒电子邮件标志。       |
| `justificationRequiredOnApproval`|`Boolean` | 用于指示审阅者是否需要提供理由审阅访问时的标志。|
| `activityDurationInDays`|`Int64` | 用户活动以向审阅者显示的天数。 |
| `autoReviewEnabled`|`Boolean` | 启用标志以指示是否审阅者未提供一个用于 auto-apply，该功能是否应设置决定。 |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | 功能设置的审阅决策，用于 auto-apply，如下所述的方式的详细的设置。 |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | 详细的定期，如下所述的设置。 |
| `autoApplyReviewResultsEnabled`|`Boolean` | 标志，指示是否自动应用启用功能，自动更改目标对象访问资源。  如果未启用，用户必须随后应用访问审阅的更改后访问审核完成。 |
| `accessRecommendationsEnabled`|`Boolean` | 用于指示是否启用向审阅者显示建议的标志。 |



## <a name="the-autoreviewsettings-type"></a>AutoReviewSettings 类型

`autoReviewSettings`嵌入访问查看设置，并访问查看完成时指定功能的行为。  该类型具有一个属性， `notReviewedResult`。

| 属性                     | 类型     | 说明                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | 必须为 `Approve`、`Deny` 或 `Recommendation` 的其中一个。 |


## <a name="the-accessreviewrecurrencesettings-type"></a>AccessReviewRecurrenceSettings 类型

`accessReviewRecurrenceSettings`嵌入访问查看设置，并指定访问审阅重复的时间间隔定期。  此类型具有以下属性：

| 属性                     | 类型                                                                                                          | 说明 |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | 重复出现的间隔，其必须是下列之一的`onetime`， `weekly`， `monthly`，`quarterly`或`annual`。                                                                   |
| `recurrenceEndType`|`String` | 如何循环将结束。 它可以是一个`Never`，是否存在重复系列，没有明确结束`Endby`，在特定日期的定期结束和`occurrences`，系列结束后完成一定数量的审阅的实例。 |
| `durationInDays`|`Int32`     | 持续的定期的天数。                                                                              |
| `recurrenceCount`|`Int32`    | 定期事件的计数如果的值`recurrenceEndType`是`occurrences`。                                                        |



<!-- {
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
