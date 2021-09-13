---
author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
ms.localizationpriority: medium
description: columnDefinition 资源上的 textColumn 指示该列的值为文本。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 26d03141bc0520d4d957e853af28c241771d8dac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084004"
---
# <a name="textcolumn-resource-type"></a>TextColumn 资源类型

命名空间：microsoft.graph

[columnDefinition](columndefinition.md) 资源上的 **textColumn** 指示该列的值为文本。

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

| 属性名称                   | 类型    | 说明
|:--------------------------------|:--------|:---------------------------------
| **allowMultipleLines**          | 布尔 | 是否支持多行文本。
| **appendChangesToExistingText** | 布尔 | 对此列的更新应替换现有文本，还是附加到现有文本。
| **linesForEditing**             | int32   | 文本框的大小。
| **maxLength**                   | int32   | 值的最大字符数。
| **textType**                    | string  | 要存储的文本类型。 必须为 `plain` 或 `richText`.的其中一个

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->

