---
title: educationCourse 资源类型
description: 表示类的课程信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9ba29e98150db6ffa9938585540d9b77f8a755cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502268"
---
# <a name="educationcourse-resource-type"></a>educationCourse 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示类的课程信息。 在 [educationClass](educationclass.md) 中使用。

## <a name="properties"></a>属性

| 属性     | 类型   | 说明                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | String | 课程的唯一标识符。         |
| 说明  | 字符串 | 课程的说明。                |
| displayName  | 字符串 | 课程的名称。                       |
| externalId   | String | 来自同步系统的课程 ID。 |
| subject      | String | 课程的主题。                    |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCourse"
}-->

```json
{
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationCourse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
