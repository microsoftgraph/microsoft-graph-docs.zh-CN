---
title: educationCourse 资源类型
description: 表示课程的课程信息。
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1b0345e6be308a175fbb14ab618fcf66564f45f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036709"
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
