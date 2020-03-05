---
title: educationalActivityDetail 资源类型
description: educationalActivityDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ccacf02184bbf54e49949d7671d34dde93b3859f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502821"
---
# <a name="educationalactivitydetail-resource-type"></a>educationalActivityDetail 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表用户已进行并在[educationalActivity](educationalActivity.md)资源中使用的 undergraduate、毕业、postgraduate 学位或其他教学活动的其他详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|缩写  |String       |缩短学位或程序的名称（示例： PhD、MBA）    |
|activities    |String       |课外与程序一起开展的活动。   |
|奖励        |String       |与该计划相关的任何奖项或荣誉。              |
|说明   |字符串       |用户提供的程序的简短说明。         |
|displayName   |字符串       |用户提供的程序的长格式名称。      |
|fieldsOfStudy |String       |与程序关联的 Majors 和未成年人。 （如果适用） |
|grade         |String       |最终成绩、类、GPA 或分数。                          |
|notes         |String       |用户提供的其他笔记。                        |
|webUrl        |String       |指向 "度" 或 "程序" 页面的链接。                            |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivityDetail",
  "baseType": null
}-->

```json
{
  "abbreviation": "String",
  "activities": "String",
  "awards": "String",
  "description": "String",
  "displayName": "String",
  "fieldsOfStudy": "String",
  "grade": "String",
  "notes": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivityDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->