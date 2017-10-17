---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 80e41b379b9b4ce51a3ee6c910447a22f43356c3
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="textcolumn-resource-type"></a>TextColumn 资源类型

[columnDefinition](columnDefinition.md) 资源上的 **textColumn** 指示该列的值为文本。

## <a name="json-representation"></a>JSON 表示形式

下面是 **textColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a>属性

| 属性名称                   | 类型   | 说明
|:--------------------------------|:-------|:-----------------------------------------------
| **allowMultipleLines**          | string | 是否允许多行文本。
| **appendChangesToExistingText** | string | 对此列的更新是应替换现有文本，还是追加到现有文本。
| **linesForEditing**             | int    | 文本框的大小。
| **maxLength**                   | int    | 值的最大字符数。
| **textType**                    | string | 要存储的文本类型。 必须是 `plain` 或 `richText` 的其中一个

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
