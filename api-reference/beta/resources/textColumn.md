---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 87a5e27544a49613d1d1e44cd6f3e0e3b7fcf8c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822566"
---
# <a name="textcolumn-resource-type"></a>TextColumn 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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

| 属性名称                   | 类型   | 说明
|:--------------------------------|:-------|:-----------------------------------------------
| **allowMultipleLines**          | string | 是否支持多行文本。
| **appendChangesToExistingText** | string | 对此列的更新应替换现有文本，还是附加到现有文本。
| **linesForEditing**             | int    | 文本框的大小。
| **maxLength**                   | int    | 值的最大字符数。
| **textType**                    | string | 要存储的文本类型。 必须为 `plain` 或 `richText`.的其中一个

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
