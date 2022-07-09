---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD 访问评审功能中，表示 `accessReviewScheduleSettings` 与访问评审系列关联的设置。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bf56ecef7491c74de864f647b34086cf658f33e6
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697147"
---
# <a name="accessreviewschedulesettings-resource-type"></a>accessReviewScheduleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 的设置。 

## <a name="properties"></a>属性
| 属性    | 类型   | 说明 |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Boolean | 指示是启用还是禁用电子邮件。 默认值为 `false`。               |
| reminderNotificationsEnabled|布尔  | 指示是否启用或禁用提醒。 默认值为 `false`。  |
| justificationRequiredOnApproval|Boolean | 指示是否需要审阅者提供其决定的理由。 默认值为 `false`。 |
| defaultDecisionEnabled|Boolean | 指示在审阅者不响应时是否启用或禁用默认决策。 默认值为 `false`。 |
| defaultDecision|String | 如果 `defaultDecisionEnabled` 启用，则选择“决定”。 可以是其中之 `Approve`一， `Deny`或 `Recommendation`。 |
| instanceDurationInDays|Int32 | 每次复查的持续时间 () `accessReviewInstance` 天数。 <br/>**注意：** 如果定义 [了 accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 **stageSettings**，则会使用其 **durationInDays** 设置，而不是此属性的值。 |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | 使用标准 Outlook 定期对象的定期的详细设置。 <br/><br/>**注意：** 仅支持 **dayOfMonth**、 **interval** 和 **type** (`weekly`， `absoluteMonthly`) 属性。 在 **recurrenceRange** 上使用属性 **startDate** 来确定审阅开始的日期。 |
| autoApplyDecisionsEnabled|Boolean | 指示是否自动应用决策。 设置为 `false`后，管理员必须在审阅者完成访问评审后手动应用决策。 设置为 `true`后，无论审阅者是否已响应，访问评审实例持续时间结束后都会自动应用决策。 默认值为 `false`。 |
| applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合 | 可选字段。 介绍审阅完成后要执行的操作。 目前支持两种类型： `removeAccessApplyAction` (默认) 和 `disableAndDeleteUserApplyAction`。 字段只需在以下情况下 `disableAndDeleteUserApplyAction`指定。 |
| recommendationsEnabled|Boolean | 指示是启用还是禁用决策建议。 <br/>**注意：** 如果定义 [了 accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 **stageSettings**，则将使用其 **recommendationsEnabled** 设置，而不是此属性的值。 |
| recommendationLookBackDuration | 持续时间| 可选字段。 指示将从中配置建议) 审阅实例的开始日期 (的非活动期。 建议 `deny` 在回首持续时间内用户是否处于非活动状态。 对于组和 Azure AD 角色的评审，将接受任何持续时间。 对于应用程序评审，30 天是最长持续时间。 如果未指定，则持续时间为 30 天。 <br/><br/>**注意：** 如果定义 [了 accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 **stageSettings**，则将使用其 **recommendationLookBackDuration** 设置，而不是此属性的值。 |
|decisionHistoriesForReviewersEnabled|Boolean| 指示对于具有多个后续阶段的 **accessReviewInstance** 上的审阅者，是否可以对以前的访问评审阶段做出决策。 如果未提供，则默认 () `false` 禁用。|
| recommendationInsightSettings|[accessReviewRecommendationInsightSetting](../resources/accessReviewRecommendationInsightSetting.md) 集合 | 可选。 介绍帮助审阅者做出访问评审决策的见解类型。 <br/><br/>**注意：** 如果定义 [了 accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 对象的 **stageSettings**，则将使用其 **recommendationInsightSettings** 设置，而不是此属性的值。 |

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
