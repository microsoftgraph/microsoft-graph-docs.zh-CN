---
author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
ms.localizationpriority: medium
description: columnDefinition 资源上的 dateTimeColumn 指示该列的值为日期或时间。
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 462110be3c0972745570e935e9d7a432b0415708
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2022
ms.locfileid: "65970991"
---
# <a name="datetimecolumn-resource-type"></a>DateTimeColumn 资源类型

命名空间：microsoft.graph

[columnDefinition](columndefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。

## <a name="json-representation"></a>JSON 表示形式

下面是 **dateTimeColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a>属性

| 属性名称      | 类型               | 说明
|:-------------------|:-------------------|:----------------------------------------------
| **displayAs**      | string             | 值在用户体验中的显示方式。 必须为 `default`、`friendly` 或 `standard` 的其中一个。 有关详细信息，请参阅下文。 如果未指定，则视为 `default`。
| **format**         | string             | 指示值是否应该只显示为日期或日期和时间。 必须为 `dateOnly` 或 `dateTime` 的其中一个

## <a name="displayas-options"></a>DisplayAs 选项

| 值        | 说明
|:-------------|:--------------------------------------------------------------
| **default**  | 使用用户体验中呈现的默认值。
| **friendly** | 使用友好相对表示形式（如 “今天下午 3:00”）
| **standard** | 使用标准绝对表示形式（如 “2017 年 5 月 10 日下午 3:20”）


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->

