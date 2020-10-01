---
title: accessReviewSettings 资源类型
description: 在创建访问评审时提供其他设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4de925ecb2fac65e3ab339ba8d4e602fcdc2af3
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330352"
---
# <a name="accessreviewsettings-resource-type"></a>accessReviewSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在创建访问评审时提供其他设置，以在启动访问评审时控制功能行为。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | 布尔值 | 指示是否已启用向审阅者发送邮件和审阅创建者。 |
| remindersEnabled | 布尔值 | 指示是否启用了向审阅者发送提醒电子邮件。 |
| justificationRequiredOnApproval | 布尔值 | 指示审阅 access 时是否需要审阅者提供理由。 |
| activityDurationInDays | Int64 | 向审阅者显示的用户活动的天数。 |
| autoReviewEnabled | 布尔值 | 指示是否应在审阅者未提供某个决定时对其进行设置。 在启用自动应用程序时使用。 如果您不希望在审阅者做出明确选择的情况下记录审阅决策，请将其设置为 `false` 。|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | 有关功能应如何设置评审决策的详细设置。 在启用自动应用程序时使用。 |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | 定期的详细设置。 |
| autoApplyReviewResultsEnabled | 布尔值 | 指示是否启用自动更改目标对象访问资源的自动应用功能。  如果未启用，则用户必须在评审完成后应用访问评审。 |
| accessRecommendationsEnabled | 布尔值 | 指示是否已启用向审阅者显示建议。 |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
```json
{
  "mailNotificationsEnabled": true,
  "remindersEnabled": true,  
  "justificationRequiredOnApproval": true,
  "activityDurationInDays": 1024,
  "autoReviewEnabled": false,
  "autoReviewSettings": {"@odata.type": "microsoft.graph.autoReviewSettings"},
  "recurrenceSettings": {"@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"},
  "autoApplyReviewResultsEnabled": false,
  "accessRecommendationsEnabled": false
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->