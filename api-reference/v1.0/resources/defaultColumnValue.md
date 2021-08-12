---
author: daspek
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: columnDefinition 资源上的 defaultColumnValue 指定此列的默认值。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 27c4d687ca1ef1601a1f687aef1af5b93906405e2a533cb4f924fc91d325d26d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152766"
---
# <a name="defaultcolumnvalue-resource-type"></a>DefaultColumnValue 资源类型

命名空间：microsoft.graph

[columnDefinition](columndefinition.md) 资源上的 **defaultColumnValue** 指定此列的默认值。
默认值可以直接指定或以公式形式指定。

## <a name="json-representation"></a>JSON 表示形式

下面是 **defaultColumnValue** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| **formula**   | string | 用于计算此列的默认值的公式。
| **value**     | string | 用作此列的默认值的直接值。

一次只能指定 **formula** 或 **value** 两者之一。

SharePoint 公式使用一种类似于 Excel 公式的语法。
有关详细信息[，请参阅 SharePoint 列表中常见][SPFormulas]公式的示例。

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/DefaultColumnValue"
} -->

