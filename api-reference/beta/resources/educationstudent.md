---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 355230339129a351f5a609292e7e7623a39a59b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049729"
---
# <a name="educationstudent-resource-type"></a>educationStudent 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。

> [!IMPORTANT]
> 使用委派权限作用域时，Graph 将仅返回 `externalId` 属性。 所有其他属性都需要应用程序范围。

## <a name="properties"></a>属性

| 属性       | 类型            | 说明                                     |
| :------------- | :-------------- | :---------------------------------------------- |
| birthDate      | Date            | 学生的出生日期。                      |
| externalId     | String          | 源系统中学生的 ID。         |
| gender         | educationGender | 可取值为：`female`、`male`、`other`。 |
| grade          | String          | 学生的当前年级。             |
| graduationYear | String          | 学生从学校毕业的年份。 |
| studentNumber  | String          | 学生编号。                                 |

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
<!--
{
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


