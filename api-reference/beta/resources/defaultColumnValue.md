---
author: daspek
description: columnDefinition 资源上的 defaultColumnValue 指定此列的默认值。
ms.date: 09/12/2017
title: DefaultColumnValue
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 3c45329a44a5023b10950f49ef568d8be071e6db
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723505"
---
# <a name="defaultcolumnvalue-resource-type"></a>DefaultColumnValue 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| 属性    | 类型   | 说明                                                    |
| :---------- | :----- | :------------------------------------------------------------- |
| **formula** | string | 用于计算此列的默认值的公式。 |
| **value**   | string | 用作此列的默认值的直接值。  |

一次只能指定 **formula** 或 **value** 两者之一。

SharePoint 公式使用一种类似于 Excel 公式的语法。
有关详细信息[，请参阅 SharePoint 列表中常见][SPFormulas]公式的示例。

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": []
}
-->
