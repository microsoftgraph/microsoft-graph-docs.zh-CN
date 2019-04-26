---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 8b39f20830da6621b1b6379674d5ef191afe5d9f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341019"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="da4a5-102">CurrencyColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="da4a5-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da4a5-103">[columnDefinition](columndefinition.md) 资源上的 **currencyColumn** 指示该列的值代表货币。</span><span class="sxs-lookup"><span data-stu-id="da4a5-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da4a5-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da4a5-104">JSON representation</span></span>

<span data-ttu-id="da4a5-105">下面是 **currencyColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da4a5-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="da4a5-106">属性</span><span class="sxs-lookup"><span data-stu-id="da4a5-106">Properties</span></span>

| <span data-ttu-id="da4a5-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="da4a5-107">Property name</span></span> | <span data-ttu-id="da4a5-108">类型</span><span class="sxs-lookup"><span data-stu-id="da4a5-108">Type</span></span>   | <span data-ttu-id="da4a5-109">说明</span><span class="sxs-lookup"><span data-stu-id="da4a5-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="da4a5-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="da4a5-110">**locale**</span></span>    | <span data-ttu-id="da4a5-111">string</span><span class="sxs-lookup"><span data-stu-id="da4a5-111">string</span></span> | <span data-ttu-id="da4a5-112">指定要从中推断货币符号的区域设置。</span><span class="sxs-lookup"><span data-stu-id="da4a5-112">Specifies the locale from which to infer the currency symbol.</span></span>

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
