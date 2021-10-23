---
title: accessReviewScheduleSettings 资源类型
description: 在Azure AD评审功能中，表示与访问评审 `accessReviewScheduleSettings` 系列关联的设置。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7005294a36ca9eda338ed7d64b174cf0bc61b989
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559381"
---
# <a name="accessreviewschedulesettings-resource-type"></a>accessReviewScheduleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。 

## <a name="properties"></a>属性
| 属性    | 类型   | 说明 |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|布尔值 | 指示是启用还是禁用电子邮件。 默认值为 `false`。               |
| reminderNotificationsEnabled|布尔值  | 指示是启用还是禁用提醒。 默认值为 `false`。  |
| justificationRequiredOnApproval|布尔值 | 指示是否要求审阅者提供其决策的理由。 默认值为 `false`。 |
| defaultDecisionEnabled|布尔值 | 指示在审阅者未响应时是启用还是禁用默认决策。 默认值为 `false`。 |
| defaultDecision|String | 如果已启用， `defaultDecisionEnabled` 则选择决策。 可以是 、 `Approve` `Deny` 或 `Recommendation` 之一。 |
| instanceDurationInDays|Int32 | 每次重复审阅的持续时间 () `accessReviewInstance` 天数表示。 |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | 使用标准定期对象定期Outlook设置。 仅 `weekly` 支持 `absoluteMonthly` **recurrencePattern 和 recurrencePattern。** 使用 **recurrenceRange 上的 属性 startDate** 确定审阅开始的一天。  |
| autoApplyDecisionsEnabled|布尔值 | 指示是否自动应用决策。 设置为 时，管理员必须在审阅者完成访问评审后手动 `false` 应用决策。 设置为 时，会在访问评审实例持续时间结束后自动应用决策，无论审阅 `true` 者是否已回复。 默认值为 `false`。 |
| applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合 | 可选字段。 介绍审阅完成后要采取的操作。 目前支持两种类型：默认 (`removeAccessApplyAction` 和) `disableAndDeleteUserApplyAction` 。 只需在 的情况下指定字段 `disableAndDeleteUserApplyAction` 。 |
| recommendationsEnabled|布尔值 | 指示是启用还是禁用决策建议。 |
| recommendationLookBackDuration | 期限| 可选字段。 指示与将配置 (的审阅实例的开始日期) 不活动时间段。 如果用户在回看期间处于非活动状态 `deny` ，则建议为 。 对于组和角色Azure AD，接受任何持续时间。 对于应用程序审查，最长期限为 30 天。 如果未指定，持续时间为 30 天。 |

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
  "recommendationLookBackDuration": "Duration"
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
