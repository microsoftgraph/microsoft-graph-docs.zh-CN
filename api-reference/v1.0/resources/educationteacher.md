---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 68c6cde2b3e7027e94c9d1ce818eea46778b5d6c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118685"
---
# <a name="teacher-resource-type"></a>教师资源类型

命名空间：microsoft.graph

添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。

## <a name="properties"></a>属性

| 属性      | 类型   | 说明                             |
| :------------ | :----- | :-------------------------------------- |
| externalId    | String | 源系统中教师的 ID。 |
| teacherNumber | String | 教师编号。                         |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTeacher"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTeacher",
  "teacherNumber": "String",
  "externalId": "String"
}
```
