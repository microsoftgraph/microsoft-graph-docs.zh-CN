---
author: swapnil1993
title: termColumn 资源类型
description: termColumn 资源指示列的值包含分类数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6d29ec570d7f3fad798fb1e2ba213b5a998643dc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446614"
---
# <a name="termcolumn-resource-type"></a>termColumn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
指示列的值包含分类数据。

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| allowMultipleValues | 布尔 | 指定列是否允许多个值   
| parentTerm     | microsoft.graph.termStore.term | 指定可选择其子项作为列值的术语 guid。  
| showFullyQualifiedName | 布尔 | 指定是显示整个术语路径还是仅显示术语标签。  
| termSet      | microsoft.graph.termStore.set | 可以选择其子项作为列值的术语集。 

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

