---
title: accessReviewSettings 资源类型
description: ''
localization_priority: Normal
ms.openlocfilehash: b19db8add3143f02f51cc0ef9d38d483d54438e1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348352"
---
# <a name="accessreviewsettings-resource-type"></a>accessReviewSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| mailNotificationsEnabled | 布尔 |  |
| remindersEnabled | 布尔 |  |
| justificationRequiredOnApproval | 布尔 |  |
| recurrenceSettings | accessReviewRecurrenceSettings |  |
| autoReviewEnabled | 布尔 |  |
| activityDurationInDays | Int32 |  |
| autoReviewSettings | autoReviewSettings |  |
| autoApplyReviewResultsEnabled | 布尔 |  |
| accessRecommendationsEnabled | 布尔 |  |


## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
``` json
{
    "mailNotificationsEnabled":"boolean",
    "remindersEnabled":"boolean",
    "justificationRequiredOnApproval":"boolean",
    "recurrenceSettings":"microsoft.graph.accessReviewRecurrenceSettings",
    "autoReviewEnabled":"boolean",
    "activityDurationInDays":"Int32",
    "autoReviewSettings":"microsoft.graph.autoReviewSettings",
    "autoApplyReviewResultsEnabled":"boolean",
    "accessRecommendationsEnabled":"boolean"
}
```



