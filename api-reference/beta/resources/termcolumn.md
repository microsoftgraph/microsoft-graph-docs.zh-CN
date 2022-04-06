---
author: swapnil1993
title: termColumn 资源类型
description: 术语Column 资源指示列的值包含分类数据。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 6ccf926f646f11f12bc150fd22b339777df4208b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757743"
---
# <a name="termcolumn-resource-type"></a>termColumn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
指示列的值包含分类数据。

## <a name="properties"></a>属性

| 属性               | 类型                           | Description                                                               |
| :--------------------- | :----------------------------- | :------------------------------------------------------------------------ |
| allowMultipleValues    | Boolean                        | 指定列是否允许多个值               |
| showFullyQualifiedName | Boolean                        | 指定是显示整个术语路径还是仅显示术语标签。 |

## <a name="relationships"></a>关系

| 关系   | 类型                      | Description
|:----------------|:--------------------------|:-------------------------------
| parentTerm     | microsoft.graph.termStore.term | 指定子术语可以选作列值的父术语。
| termSet      | microsoft.graph.termStore.set | 可以选择其子项作为列值的术语集。

## <a name="json-representation"></a>JSON 表示形式

下面是 **termColumn** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.termColumn" } -->

```json
{
    "allowMultipleValues": true,
    "showFullyQualifiedName": false,
}
```
