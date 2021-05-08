---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41a878f58736f608cf9cc9f0c45867bf48669b1a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231834"
---
# <a name="educationterm-resource-type"></a>educationTerm 资源类型

命名空间：microsoft.graph

一个学期。 它表示学年的指定部分。 在 [educationClass](educationclass.md) 中使用。

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                       |
| :---------- | :----- | :-------------------------------- |
| displayName | String | 学期的显示名称。         |
| externalId  | String | 同步系统中的学期 ID。 |
| startDate   | Date   | 学期开始日期。                |
| endDate     | Date   | 学期结束日期。                  |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTerm"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTerm",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date",
  "displayName": "String"
}
```
