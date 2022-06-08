---
author: JeremyKelley
description: columnDefinition 资源上的 currencyColumn 指示该列的值代表货币。
ms.date: 09/11/2017
title: CurrencyColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: d355d6e7226d538b214958f936d656799e999a21
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944995"
---
# <a name="currencycolumn-resource-type"></a>CurrencyColumn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。

## <a name="json-representation"></a>JSON 表示形式

下面是 **currencyColumn** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a>属性

| 属性   | 类型   | 说明                                                   |
| :--------- | :----- | :------------------------------------------------------------ |
| **locale** | string | 指定要从中推断货币符号的区域设置。 |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": []
}
-->
