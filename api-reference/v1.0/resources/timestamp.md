---
title: timeStamp 资源类型
description: 时间点的日期和时间信息。
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f284439f63d15c1cf6d070894a8f9f9074f69e24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59093986"
---
# <a name="timestamp-resource-type"></a>timeStamp 资源类型

命名空间：microsoft.graph

时间点的日期和时间信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|date|Date|时间戳的日期部分。|
|time|TimeOfDay|时间戳的时间部分。|
|timeZone|String|时间戳的时区部分，它是世界上 24 个纵向区域之一。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

