---
author: JeremyKelley
description: columnDefinition 资源上的 textColumn 指示该列的值为文本。
ms.date: 09/11/2017
title: TextColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8a6e8d3a06c3d34a321ec2fb5ff5d83586accb56
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724285"
---
# <a name="textcolumn-resource-type"></a>TextColumn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| 属性                        | 类型   | 说明                                                                   |
| :------------------------------ | :----- | :---------------------------------------------------------------------------- |
| **allowMultipleLines**          | string | 是否支持多行文本。                                      |
| **appendChangesToExistingText** | string | 对此列的更新应替换现有文本，还是附加到现有文本。 |
| **linesForEditing**             | int    | 文本框的大小。                                                     |
| **maxLength**                   | int    | 值的最大字符数。                               |
| **textType**                    | string | 要存储的文本类型。 必须为 `plain` 或 `richText`.的其中一个           |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": []
}
-->
