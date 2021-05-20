---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD 访问评审功能中，表示与访问 `accessReviewScheduleSettings` 评审系列关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b354ebfc2b5e6c8093f65c8712516421f0b1d332
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579730"
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
| justificationRequiredOnApproval|布尔 | 指示是否要求审阅者提供其决策的理由。 默认值为 `false`。 |
| defaultDecisionEnabled|布尔 | 指示在审阅者未响应时是启用还是禁用默认决策。 默认值为 `false`。 |
| defaultDecision|String | 如果已启用， `defaultDecisionEnabled` 则选择决策。 可以是 、 `Approve` `Deny` 或 `Recommendation` 之一。 |
| instanceDurationInDays|Int32 | 每次重复审阅的持续时间 () `accessReviewInstance` 天数表示。 |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | 使用标准定期对象定期Outlook设置。 仅 `weekly` 支持 `absoluteMonthly` **recurrencePattern 和 recurrencePattern。** 使用 **recurrenceRange 上的 属性 startDate** 确定审阅开始的一天。  |
| autoApplyDecisionsEnabled|布尔 | 指示是否自动应用决策。 设置为 时，用户必须在审阅者完成访问评审后 `false` 手动应用决策。 设置为 时，会在访问评审实例持续时间结束后自动应用决策，无论审阅 `true` 者是否已回复。 默认值为 `false`。 |
| applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合 | 可选字段。 介绍审阅完成后要采取的操作。 目前支持两种类型：默认 (`removeAccessApplyAction` 和) `disableAndDeleteUserApplyAction` 。 只需在 的情况下指定字段 `disableAndDeleteUserApplyAction` 。 请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。 |
| recommendationsEnabled|布尔 | 指示是否启用/禁用决策建议。 |

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
  "recommendationsEnabled": "Boolean"
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
