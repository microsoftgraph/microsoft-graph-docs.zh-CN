---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD 访问评审功能中，表示与访问 `accessReviewScheduleSettings` 评审系列关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a58ba9a682e443efbc159befaea61b15e3fdc81
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133442"
---
# <a name="accessreviewschedulesettings-resource-type"></a>accessReviewScheduleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。 

## <a name="properties"></a>属性
| 属性    | 类型   | 说明 |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Boolean | 指示电子邮件是否已启用/禁用的标志。                |
| reminderNotificationsEnabled|Boolean  | 指示是否启用/禁用提醒的标志。   |
| justificationRequiredOnApproval|Boolean | 用于指示是否需要审阅者提供其决策理由的标志。 |
| defaultDecisionEnabled|Boolean | 指示在审阅者未响应时是否启用/禁用默认决策的标志。 |
| defaultDecision|字符串 | 如果已启用， `defaultDecisionEnabled` 则选择决策。 可以是"批准"、"拒绝"或"建议"之一。 |
| instanceDurationInDays|Int32 | 每次重复审阅的持续时间 `accessReviewInstance` () 天数。 |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | 定期的详细设置。 使用标准 Outlook 定期对象。  |
| autoApplyDecisionsEnabled|Boolean | 用于指示是否已启用自动应用功能的标志。 |
| applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合 | 可选字段。 介绍在审阅完成后要采取的操作。 目前支持两种类型：默认 (`removeAccessApplyAction` 和 `disableAndDeleteUserApplyAction`) 。 字段只需要在 . `disableAndDeleteUserApplyAction` 请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。 |
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
