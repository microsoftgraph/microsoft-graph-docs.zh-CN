---
author: swapnil1993
title: termColumn 资源类型
description: 术语Column 资源指示列的值包含分类数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: fcdad019f3eb2496116767e560f63a4668ed7508
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720865"
---
# <a name="termcolumn-resource-type"></a>termColumn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
指示列的值包含分类数据。

## <a name="properties"></a>属性

| 属性               | 类型                           | 说明                                                               |
| :--------------------- | :----------------------------- | :------------------------------------------------------------------------ |
| allowMultipleValues    | Boolean                        | 指定列是否允许多个值               |
| parentTerm             | microsoft.graph.termStore.term | 指定可选择其子项作为列值的术语 guid。 |
| showFullyQualifiedName | Boolean                        | 指定是显示整个术语路径还是仅显示术语标签。 |
| termSet                | microsoft.graph.termStore.set  | 可以选择其子项作为列值的术语集。                 |

## <a name="json-representation"></a>JSON 表示形式

下面是 **termColumn** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "parentTerm": { "@type": "microsoft.graph.termStore.term" },
    "showFullyQualifiedName": false,
    "termSet": { "@type": "microsoft.graph.termStore.set" }
}
```
