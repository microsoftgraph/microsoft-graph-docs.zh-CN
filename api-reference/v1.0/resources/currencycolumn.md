---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
description: columnDefinition 资源上的 currencyColumn 指示该列的值代表货币。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1270900c11a65bf974ac78ffe6af37bf93c51af6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531742"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="c04b2-103">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="c04b2-103">CurrencyColumn resource type</span></span>

<span data-ttu-id="c04b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c04b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c04b2-105">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="c04b2-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c04b2-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c04b2-106">JSON representation</span></span>

<span data-ttu-id="c04b2-107">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c04b2-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="c04b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="c04b2-108">Properties</span></span>

| <span data-ttu-id="c04b2-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="c04b2-109">Property name</span></span> | <span data-ttu-id="c04b2-110">类型</span><span class="sxs-lookup"><span data-stu-id="c04b2-110">Type</span></span>   | <span data-ttu-id="c04b2-111">说明</span><span class="sxs-lookup"><span data-stu-id="c04b2-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c04b2-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="c04b2-112">**locale**</span></span>    | <span data-ttu-id="c04b2-113">string</span><span class="sxs-lookup"><span data-stu-id="c04b2-113">string</span></span> | <span data-ttu-id="c04b2-114">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="c04b2-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
