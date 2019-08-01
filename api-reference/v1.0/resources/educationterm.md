---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 36426a7e3f1fb79264a788d8af7e7768f5bae26a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032618"
---
# <a name="educationterm-resource-type"></a>educationTerm 资源类型

一个学期。 它表示学年的指定部分。 在 [educationClass](educationclass.md) 中使用。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|displayName| String| 学期的显示名称。| 
|externalId|String| 同步系统中的学期 ID。|
|startDate|日期|学期开始日期。|
|endDate|Date|学期结束日期。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
