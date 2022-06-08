---
author: JeremyKelley
description: columnDefinition 资源上的 choiceColumn 指示可从所选列表中选择列的值。
ms.date: 09/11/2017
title: ChoiceColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 4aac6e565274ef17263e0bbf5a3c8eeade9d729c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944911"
---
# <a name="choicecolumn-resource-type"></a>ChoiceColumn 资源类型

命名空间：microsoft.graph

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

| 属性           | 类型               | 说明                                                                                                   |
| :----------------- | :----------------- | :------------------------------------------------------------------------------------------------------------ |
| **allowTextEntry** | boolean            | 如果为 true，则允许配置选择之外的自定义值。                                          |
| **choices**        | collection(string) | 可用于此列的值列表。                                                                 |
| **displayAs**      | string             | 选择在用户体验中的显示方式。 必须为 `checkBoxes`、`dropDownMenu` 或 `radioButtons` 的其中一个。 |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
