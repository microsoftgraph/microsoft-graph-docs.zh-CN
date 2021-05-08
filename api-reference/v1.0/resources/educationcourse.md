---
title: educationCourse 资源类型
description: 表示课程的课程信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 347eb92cd0b36789cc7ecce1dea72af6985ea330
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232135"
---
# <a name="educationcourse-resource-type"></a>educationCourse 资源类型

命名空间：microsoft.graph

表示课程的课程信息。 在 [educationClass](educationclass.md) 中使用。

## <a name="properties"></a>属性

| 属性     | 类型   | 说明                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | String | 课程的唯一标识符。         |
| 说明  | String | 课程说明。                |
| displayName  | String | 课程名称。                       |
| externalId   | String | 同步系统中课程的 ID。 |
| subject      | String | 课程主题。                    |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationCourse"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationCourse",
  "subject": "String",
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String"
}
```
