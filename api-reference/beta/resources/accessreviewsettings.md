---
title: accessReviewSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: ''
ms.openlocfilehash: 21915811da771bd0eebdb5fb2c16df5cfbdea096
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508455"
---
# <a name="accessreviewsettings-resource-type"></a>accessReviewSettings 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| mailNotificationsEnabled | boolean |  |
| remindersEnabled | boolean |  |
| justificationRequiredOnApproval | boolean |  |
| recurrenceSettings | accessReviewRecurrenceSettings |  |
| autoReviewEnabled | boolean |  |
| activityDurationInDays | Int32 |  |
| autoReviewSettings | autoReviewSettings |  |
| autoApplyReviewResultsEnabled | boolean |  |
| accessRecommendationsEnabled | boolean |  |


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



