---
title: 'accessReviewSettings 资源类型 (已弃用) '
description: 创建访问评审时提供其他设置。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f197ca69132252a58508aa57b2c192eaae34077f
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821202"
---
# <a name="accessreviewsettings-resource-type-deprecated"></a>accessReviewSettings 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

在创建访问评审时提供其他设置，以控制启动访问评审时的功能行为。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | Boolean | 指示是否已启用向审阅者和审阅创建者发送邮件。 |
| remindersEnabled | Boolean | 指示是否启用向审阅者发送提醒电子邮件。 |
| justificationRequiredOnApproval | Boolean | 指示审阅者是否需要在审阅访问权限时提供理由。 |
| activityDurationInDays | Int64 | 要向审阅者显示的用户活动天数。 |
| autoReviewEnabled | Boolean | 指示如果审阅者未提供决策，是否应设置决策。 启用自动应用时使用。 如果你不想记录审阅决定，除非审阅者做出明确的选择，请将其设置为 `false`。|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | 有关该功能应如何设置评审决策的详细设置。 启用自动应用时使用。 |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | 定期的详细设置。 |
| autoApplyReviewResultsEnabled | Boolean | 指示是否启用自动应用功能，以自动更改目标对象访问资源。  如果未启用，则用户必须在评审完成后应用访问评审。 |
| accessRecommendationsEnabled | Boolean | 指示是否已启用向审阅者显示建议。 |

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
