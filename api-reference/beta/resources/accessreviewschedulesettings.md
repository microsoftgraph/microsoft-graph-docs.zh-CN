---
title: accessReviewScheduleSettings 资源类型
description: 在Azure AD评审"功能中，`accessReviewScheduleSettings`表示与访问评审系列关联的设置。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb7dbc40944d42f50b68b82cf2be8a2499020f8a
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816054"
---
# <a name="accessreviewschedulesettings-resource-type"></a>accessReviewScheduleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。 

## <a name="properties"></a>属性
| 属性    | 类型   | 说明 |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|布尔 | 指示是启用还是禁用电子邮件。 默认值为 `false`。               |
| reminderNotificationsEnabled|布尔  | 指示是启用还是禁用提醒。 默认值为 `false`。  |
| justificationRequiredOnApproval|Boolean | 指示是否要求审阅者提供其决策的理由。 默认值为 `false`。 |
| defaultDecisionEnabled|布尔 | 指示在审阅者未响应时是启用还是禁用默认决策。 默认值为 `false`。 |
| defaultDecision|字符串 | 如果已启用，则 `defaultDecisionEnabled` 选择决策。 可以是 、 `Approve`或 `Deny`之一 `Recommendation`。 |
| instanceDurationInDays|Int32 | 每次重复审阅的持续时间 () `accessReviewInstance` 天数表示。 <br/>**注意：** 如果定义了 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 **stageSettings**，则使用 **其 durationInDays** 设置，而不是此属性的值。 |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | 使用标准定期对象定期Outlook设置。 <br/><br/>**注意：** 只有 **dayOfMonth****、interval** 和 **type (** `weekly`， `absoluteMonthly`) 属性才受支持。 使用 **recurrenceRange 上的 属性 startDate** 确定审阅开始的哪一天。 |
| autoApplyDecisionsEnabled|Boolean | 指示是否自动应用决策。 设置为 时 `false`，管理员必须在审阅者完成访问评审后手动应用决策。 设置为 时 `true`，会在访问评审实例持续时间结束后自动应用决策，无论审阅者是否已回复。 默认值为 `false`。 |
| applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合 | 可选字段。 介绍审阅完成后要采取的操作。 目前支持两种类型：默认 (`removeAccessApplyAction` 和) `disableAndDeleteUserApplyAction`。 只需在 的情况下指定字段 `disableAndDeleteUserApplyAction`。 |
| recommendationsEnabled|Boolean | 指示是启用还是禁用决策建议。 <br/>**注意：** 如果定义了 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 **stageSettings**，则使用 **其 recommendationsEnabled** 设置，而不是此属性的值。 |
| recommendationLookBackDuration | 期限| 可选字段。 指示与将配置 (的审阅实例的开始日期) 不活动时间段。 如果用户在回看 `deny` 持续时间处于非活动状态，则建议为 。 对于组和角色Azure AD，接受任何持续时间。 对于应用程序审查，最长期限为 30 天。 如果未指定，持续时间为 30 天。 <br/><br/>**注意：** 如果定义了 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 **stageSettings**，则使用 **其 recommendationLookBackDuration** 设置，而不是此属性的值。 |
|decisionHistoriesForReviewersEnabled|Boolean| 指示在具有多个后续阶段的 **accessReviewInstance** 上，审阅者是否可以做出有关以前访问评审阶段的决策。 如果未提供，则默认情况下 () `false` 。|
| recommendationInsightSettings|[accessReviewRecommendationInsightSetting](../resources/accessReviewRecommendationInsightSetting.md) 集合 | 可选。 介绍帮助审阅者做出访问评审决策的见解类型。 <br/><br/>**注意：** 如果定义了 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 **stageSettings**，则使用 **其 recommendationInsightSettings** 设置，而不是此属性的值。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "mailNotificationsEnabled": "Boolean",
  "reminderNotificationsEnabled": "Boolean",
  "justificationRequiredOnApproval": "Boolean",
  "defaultDecisionEnabled": "Boolean",
  "defaultDecision": "String",
  "instanceDurationInDays": "Integer",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "autoApplyDecisionsEnabled": "Boolean",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.removeAccessApplyAction"
    }
  ],
  "recommendationsEnabled": "Boolean",
  "recommendationLookBackDuration": "Duration",
  "decisionHistoriesForReviewersEnabled": "Boolean",
  "recommendationInsightSettings": [
    {
      "@odata.type": "microsoft.graph.accessReviewRecommendationInsightSetting"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
