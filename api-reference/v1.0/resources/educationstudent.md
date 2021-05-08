---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b0e154beb5b8133c69392af8fa9611263c68945
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231848"
---
# <a name="educationstudent-resource-type"></a>educationStudent 资源类型

命名空间：microsoft.graph

添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。

## <a name="properties"></a>属性

| 属性       | 类型            | 说明                                                               |
| :------------- | :-------------- | :------------------------------------------------------------------------ |
| birthDate      | Date            | 学生的出生日期。                                                |
| externalId     | String          | 源系统中学生的 ID。                                   |
| gender         | educationGender | 可能的值包括 `female`、`male`、`other`、`unknownFutureValue`。 |
| grade          | String          | 学生的当前年级。                                       |
| graduationYear | String          | 学生从学校毕业的年份。                           |
| studentNumber  | String          | 学生编号。                                                           |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationStudent"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationStudent",
  "graduationYear": "String",
  "grade": "String",
  "birthDate": "DateTimeOffset",
  "gender": "String",
  "studentNumber": "String",
  "externalId": "String"
}
```
