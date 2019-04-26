---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
localization_priority: Normal
ms.openlocfilehash: 8d968b8177da942c1b8940618c8ba965c362c914
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341867"
---
# <a name="timezonebase-resource-type"></a>timeZoneBase 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

时区的基本表示形式。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
| name | string | 时区的名称。 它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。 |


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
