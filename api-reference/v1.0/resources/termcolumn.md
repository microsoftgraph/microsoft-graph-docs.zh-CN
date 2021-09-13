---
author: swapnil1993
title: termColumn 资源类型
description: 术语Column 资源指示列的值包含分类数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d89d389b78c4c8dc1a370722a5b40c7cff794d3d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128037"
---
# <a name="termcolumn-resource-type"></a>termColumn 资源类型

命名空间：microsoft.graph

表示托管元数据列中的SharePoint。

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明|
|:--------------|:-------|:----------------------------------------------------|
| allowMultipleValues | Boolean | 指定列是否允许多个值。|
| parentTerm     | microsoft.graph.termStore.term | 指定可选择其子项作为列值的术语 GUID。  |
| showFullyQualifiedName | Boolean | 指定是显示整个术语路径还是仅显示术语标签。  |
| termSet      | microsoft.graph.termStore.set | 可以选择其子项作为列值的术语集。 |

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

