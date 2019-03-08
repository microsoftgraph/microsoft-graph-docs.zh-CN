---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 065ac52a4d5216a4b3e62df892c8fe0a07a82ed0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481529"
---
# <a name="currencycolumn-resource-type"></a>CurrencyColumn 资源类型

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

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| **locale**    | string | 指定要从中推断货币符号的区域设置。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
