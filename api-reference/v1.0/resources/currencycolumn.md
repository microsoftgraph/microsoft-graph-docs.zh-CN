---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: e4ee085882cadafc0102ee31e17841978cef7822
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836454"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="fa69f-102">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa69f-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="fa69f-103">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="fa69f-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa69f-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa69f-104">JSON representation</span></span>

<span data-ttu-id="fa69f-105">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa69f-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="fa69f-106">属性</span><span class="sxs-lookup"><span data-stu-id="fa69f-106">Properties</span></span>

| <span data-ttu-id="fa69f-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="fa69f-107">Property name</span></span> | <span data-ttu-id="fa69f-108">类型</span><span class="sxs-lookup"><span data-stu-id="fa69f-108">Type</span></span>   | <span data-ttu-id="fa69f-109">说明</span><span class="sxs-lookup"><span data-stu-id="fa69f-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="fa69f-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="fa69f-110">**locale**</span></span>    | <span data-ttu-id="fa69f-111">string</span><span class="sxs-lookup"><span data-stu-id="fa69f-111">string</span></span> | <span data-ttu-id="fa69f-112">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="fa69f-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
