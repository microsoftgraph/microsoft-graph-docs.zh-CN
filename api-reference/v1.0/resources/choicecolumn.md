---
author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
description: columnDefinition 资源上的 choiceColumn 指示可从所选列表中选择列的值。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9f8a5f333c0904732ef47bcac0c962f522d3ecd4c5e11a6884eaf396e354b49b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121303"
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn 资源类型

命名空间：microsoft.graph

[columnDefinition](columndefinition.md) 资源上的 **choiceColumn** 指示可从所选列表中选择列的值。

## <a name="json-representation"></a>JSON 表示形式

下面是 **choiceColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a>属性

| 属性名称      | 类型               | 说明
|:-------------------|:-------------------|:----------------------------------------------
| **allowTextEntry** | boolean            | 如果为 true，则允许配置选择之外的自定义值。
| **choices**        | collection(string) | 可用于此列的值列表。
| **displayAs**      | string             | 选择在用户体验中的显示方式。 必须为 `checkBoxes`、`dropDownMenu` 或 `radioButtons` 的其中一个。


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->

