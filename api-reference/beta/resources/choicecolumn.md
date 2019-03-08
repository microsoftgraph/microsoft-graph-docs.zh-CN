---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 21405fe3aa28e0eef1233cd6f27e63568fb4b00e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482215"
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/choicecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
