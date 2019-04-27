---
title: accessReviewRecurrenceSettings 资源类型
description: ''
localization_priority: Normal
ms.openlocfilehash: 1a5235639209830d36cf69c027cfd309fab09c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348349"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>accessReviewRecurrenceSettings 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
| recurrenceType | string |  |
| recurrenceEndType | string |  |
| durationInDays | Int32 |  |
| recurrenceCount | Int32 |  |

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
``` json
{
    "recurrenceType":"string",
    "recurrenceEndType":"string",
    "durationInDays":"Int32",
    "recurrenceCount":"Int32"
}
```



