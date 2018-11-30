---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
ms.openlocfilehash: f6f4218c4e33937fa510461bc9de4689aefea71f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011400"
---
# <a name="defaultcolumnvalue-resource-type"></a>DefaultColumnValue 资源类型

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
请参阅 [SharePoint 列表中的常用公式示例][ SPFormulas]，了解详细信息。

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
