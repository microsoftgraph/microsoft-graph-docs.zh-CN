---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD 访问评审功能中，表示与访问 `accessReviewScheduleSettings` 评审系列关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 77ea7d8601df36525aad7a3448aa3b6f031d98d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469316"
---
# <a name="accessreviewschedulesettings-resource-type"></a>accessReviewScheduleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。 

## <a name="properties"></a>属性
| 属性    | 类型   | 说明 |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Boolean | 指示电子邮件是否已启用/禁用的标志。                |
| reminderNotificationsEnabled|Boolean  | 指示是否启用/禁用提醒的标志。   |
| justificationRequiredOnApproval|Boolean | 用于指示是否需要审阅者提供其决策的理由的标志。 |
| defaultDecisionEnabled|Boolean | 指示在审阅者未响应时是否启用/禁用默认决策的标志。 |
| defaultDecision|String | 如果已启用， `defaultDecisionEnabled` 则选择决策。 可以是"批准"、"拒绝"或"建议"之一。 |
| instanceDurationInDays|Int32 | 每次重复审阅的持续时间 () `accessReviewInstance` 天数表示。 |
| 定期|[patternedRecurrence](../resources/patternedrecurrence.md) | 定期的详细设置。 使用标准 Outlook 定期对象。 请注意，dayOfMonth 不受支持 - 在 recurrenceRange 上使用属性 startDate 确定评价开始的那一天。 |
| autoApplyDecisionsEnabled|Boolean | 指示是否已启用自动应用功能的标志。 |
| applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合 | 可选字段。 介绍审阅完成后要采取的操作。 目前支持两种类型：默认 (`removeAccessApplyAction` 和) `disableAndDeleteUserApplyAction` 。 只需在 的情况下指定字段 `disableAndDeleteUserApplyAction` 。 请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。 |
| recommendationsEnabled|Boolean | 指示是否启用/禁用决策建议的标志。 |

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
