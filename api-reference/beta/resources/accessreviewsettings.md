---
title: accessReviewSettings 资源类型
description: 在创建访问评审时提供其他设置。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fdc8d22639d098619ef7183ebe22fc9da7bc0287
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293083"
---
# <a name="accessreviewsettings-resource-type"></a>accessReviewSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

在创建访问评审时提供其他设置，以控制开始访问评审时的功能行为。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| mailNotificationsEnabled | Boolean | 指示是否已启用向审阅者和审阅创建者发送邮件。 |
| remindersEnabled | Boolean | 指示是否已启用向审阅者发送提醒电子邮件。 |
| justificationRequiredOnApproval | Boolean | 指示审阅者在审阅访问权限时是否需要提供理由。 |
| activityDurationInDays | Int64 | 要向审阅者显示的用户活动天数。 |
| autoReviewEnabled | Boolean | 指示如果审阅者未提供决策，是否应该设置决策。 在启用自动应用时使用。 如果不希望记录审阅决定，除非审阅者做出明确选择，请设置为 `false` 。|
| autoReviewSettings | [autoReviewSettings](autoreviewsettings.md) | 功能如何设置审阅决定的详细设置。 在启用自动应用时使用。 |
| recurrenceSettings | [accessReviewRecurrenceSettings](accessreviewrecurrencesettings.md) | 定期的详细设置。 |
| autoApplyReviewResultsEnabled | Boolean | 指示是否启用自动应用功能以自动更改目标对象访问资源。  如果未启用，则用户必须在审阅完成后应用访问评审。 |
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
