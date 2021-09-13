---
title: accessReviewScheduleSettings 资源类型
description: 表示与访问评审系列关联的设置。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fa090e7e51a9df31ce5a988fc6f79167e106b800
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084704"
---
# <a name="accessreviewschedulesettings-resource-type"></a>accessReviewScheduleSettings 资源类型

命名空间：microsoft.graph

**accessReviewScheduleSettings** 定义 [accessReviewScheduleDefinition 的设置](accessreviewscheduledefinition.md)。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| mailNotificationsEnabled|Boolean | 指示是启用还是禁用电子邮件。 默认值为 `false`。               |
| reminderNotificationsEnabled|布尔值  | 指示是启用还是禁用提醒。 默认值为 `false`。  |
| justificationRequiredOnApproval|Boolean | 指示是否要求审阅者提供其决策的理由。 默认值为 `false`。 |
| defaultDecisionEnabled|布尔值 | 指示在审阅者未响应时是启用还是禁用默认决策。 默认值为 `false`。 |
| defaultDecision|String | 如果 **defaultDecisionEnabled** 为 ，则选择决策 `true` 。 可以是 、 `Approve` `Deny` 或 `Recommendation` 之一。 |
| instanceDurationInDays|Int32 | 每次定期审阅的持续时间 (**accessReviewInstance)** 天数表示。 |
| recurrence|[patternedRecurrence](../resources/patternedrecurrence.md) | 使用标准定期对象定期Outlook设置。 仅 `weekly` 支持 `absoluteMonthly` **recurrencePattern 和 recurrencePattern。** 使用 **recurrenceRange 上的 属性 startDate** 确定审阅开始的哪一天。  |
| autoApplyDecisionsEnabled|布尔值 | 指示是否自动应用决策。 设置为 时，用户必须在审阅者完成访问评审后手动 `false` 应用决策。 设置为 时，会在访问评审实例持续时间结束后自动应用决策，无论审阅 `true` 者是否已回复。 默认值为 `false`。 |
| applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) 集合 | 可选字段。 介绍审阅完成后要采取的操作。 目前支持两种类型：默认 (和 `removeAccessApplyAction` `disableAndDeleteUserApplyAction`) 。 只需在 的情况下指定字段 `disableAndDeleteUserApplyAction` 。 请参阅 [accessReviewApplyAction](accessreviewapplyaction.md)。 |
| recommendationsEnabled|Boolean | 指示是启用还是禁用决策建议。 |

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
