---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 792f490ef9aa8ccdf6155b0eee0daf9f7c66b3b9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118664"
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
