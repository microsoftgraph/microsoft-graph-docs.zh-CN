---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 80135827abb2dbf934e7ebec5e25ae6a52e58513
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822048"
---
# <a name="educationstudent-resource-type"></a>educationStudent 资源类型

添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|birthDate|Date| 学生的出生日期。|
|externalId|String| 源系统中学生的 ID。|
|gender|educationGender| 可能的值为： `female`， `male`， `other`， `unknownFutureValue`。|
|grade|String|学生的当前年级。|
|graduationYear|String| 学生从学校毕业的年份。|
|studentNumber|String| 学生编号。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
