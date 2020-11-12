---
title: accessReviewScheduleSettings 资源类型
description: 在 Azure AD access 评论功能中， `accessReviewScheduleSettings` 表示与访问审阅系列相关联的设置。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cca1fa7fd0da05719c22728dd472087d9737d4e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000833"
---
# <a name="accessreviewschedulesettings-resource-type"></a>accessReviewScheduleSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**AccessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)的设置。 

## <a name="properties"></a>属性
| 属性    | 类型   | 说明 |
| :---------------| :---------- | :---------- |
| mailNotificationsEnabled|Boolean | 用于指示是否启用/禁用电子邮件的标志。                |
| reminderNotificationsEnabled|Boolean  | 指示是否启用/禁用提醒的标志。   |
| justificationRequiredOnApproval|Boolean | 指示是否需要审阅者根据自己的决定提供理由的标志。 |
| defaultDecisionEnabled|Boolean | 指示在审阅者不响应时是否启用/禁用默认决定的标志。 |
| defaultDecision|字符串 | `defaultDecisionEnabled`已启用决策选择。 可以是 "批准"、"拒绝" 或 "建议" 之一。 |
| instanceDurationInDays|Int32 | 每次重复检查的持续时间 (`accessReviewInstance`) 的天数。 |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | 定期的详细设置。 使用标准的 Outlook 定期对象。  |
| autoApplyDecisionsEnabled|Boolean | 用于指示是否启用自动应用功能的标志。 |
| applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合 | 可选字段。 介绍完成审阅后要执行的操作。 当前支持以下两种类型： `removeAccessApplyAction` (默认) 和 `disableAndDeleteUserApplyAction` 。 只需在的情况下指定字段 `disableAndDeleteUserApplyAction` 。 请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。 |
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
