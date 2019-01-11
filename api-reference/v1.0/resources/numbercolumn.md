---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: 25db21e6495edb6c42746c47d257ae60a4c1cc07
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867408"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="4c9af-102">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c9af-102">NumberColumn resource type</span></span>

<span data-ttu-id="4c9af-103">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="4c9af-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c9af-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c9af-104">JSON representation</span></span>

<span data-ttu-id="4c9af-105">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c9af-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="4c9af-106">属性</span><span class="sxs-lookup"><span data-stu-id="4c9af-106">Properties</span></span>

| <span data-ttu-id="4c9af-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="4c9af-107">Property name</span></span>      | <span data-ttu-id="4c9af-108">类型</span><span class="sxs-lookup"><span data-stu-id="4c9af-108">Type</span></span>   | <span data-ttu-id="4c9af-109">说明</span><span class="sxs-lookup"><span data-stu-id="4c9af-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="4c9af-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="4c9af-110">**decimalPlaces**</span></span>  | <span data-ttu-id="4c9af-111">string</span><span class="sxs-lookup"><span data-stu-id="4c9af-111">string</span></span> | <span data-ttu-id="4c9af-112">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="4c9af-112">How many decimal places to display.</span></span> <span data-ttu-id="4c9af-113">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="4c9af-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="4c9af-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="4c9af-114">**displayAs**</span></span>      | <span data-ttu-id="4c9af-115">string</span><span class="sxs-lookup"><span data-stu-id="4c9af-115">string</span></span> | <span data-ttu-id="4c9af-116">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="4c9af-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="4c9af-117">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="4c9af-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="4c9af-118">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="4c9af-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="4c9af-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="4c9af-119">**maximum**</span></span>        | <span data-ttu-id="4c9af-120">double</span><span class="sxs-lookup"><span data-stu-id="4c9af-120">double</span></span> | <span data-ttu-id="4c9af-121">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="4c9af-121">The maximum permitted value.</span></span>
| <span data-ttu-id="4c9af-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="4c9af-122">**minimum**</span></span>        | <span data-ttu-id="4c9af-123">double</span><span class="sxs-lookup"><span data-stu-id="4c9af-123">double</span></span> | <span data-ttu-id="4c9af-124">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="4c9af-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="4c9af-125">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="4c9af-125">DecimalPlaces</span></span>

| <span data-ttu-id="4c9af-126">值</span><span class="sxs-lookup"><span data-stu-id="4c9af-126">Value</span></span>          | <span data-ttu-id="4c9af-127">说明</span><span class="sxs-lookup"><span data-stu-id="4c9af-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="4c9af-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="4c9af-128">**automatic**</span></span>  | <span data-ttu-id="4c9af-129">默认值。</span><span class="sxs-lookup"><span data-stu-id="4c9af-129">Default.</span></span> <span data-ttu-id="4c9af-130">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="4c9af-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="4c9af-131">**none**</span><span class="sxs-lookup"><span data-stu-id="4c9af-131">**none**</span></span>       | <span data-ttu-id="4c9af-132">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="4c9af-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="4c9af-133">**one**</span><span class="sxs-lookup"><span data-stu-id="4c9af-133">**one**</span></span>        | <span data-ttu-id="4c9af-134">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="4c9af-134">Always display one decimal place.</span></span>
| <span data-ttu-id="4c9af-135">**two**</span><span class="sxs-lookup"><span data-stu-id="4c9af-135">**two**</span></span>        | <span data-ttu-id="4c9af-136">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="4c9af-136">Always display two decimal places.</span></span>
| <span data-ttu-id="4c9af-137">**three**</span><span class="sxs-lookup"><span data-stu-id="4c9af-137">**three**</span></span>      | <span data-ttu-id="4c9af-138">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="4c9af-138">Always display three decimal places.</span></span>
| <span data-ttu-id="4c9af-139">**four**</span><span class="sxs-lookup"><span data-stu-id="4c9af-139">**four**</span></span>       | <span data-ttu-id="4c9af-140">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="4c9af-140">Always display four decimal places.</span></span>
| <span data-ttu-id="4c9af-141">**five**</span><span class="sxs-lookup"><span data-stu-id="4c9af-141">**five**</span></span>       | <span data-ttu-id="4c9af-142">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="4c9af-142">Always display five decimal places.</span></span>

<span data-ttu-id="4c9af-143">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="4c9af-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="4c9af-144">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="4c9af-144">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
