---
title: accessReviewRecurrenceSettings 资源类型
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: ''
ms.openlocfilehash: 807be44f256fa3a9080cc3cb458033726aadc107
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508469"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>accessReviewRecurrenceSettings 资源类型

命名空间： microsoft. graph

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



