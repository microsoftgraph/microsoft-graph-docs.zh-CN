---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: columnDefinition 资源上的 numberColumn 指示该列的值为数字。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f2d8955ac71a7a6e9979542f08e4d0634274b69b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083020"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="583a7-103">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="583a7-103">NumberColumn resource type</span></span>

<span data-ttu-id="583a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="583a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="583a7-105">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="583a7-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="583a7-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="583a7-106">JSON representation</span></span>

<span data-ttu-id="583a7-107">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="583a7-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="583a7-108">属性</span><span class="sxs-lookup"><span data-stu-id="583a7-108">Properties</span></span>

| <span data-ttu-id="583a7-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="583a7-109">Property name</span></span>      | <span data-ttu-id="583a7-110">类型</span><span class="sxs-lookup"><span data-stu-id="583a7-110">Type</span></span>   | <span data-ttu-id="583a7-111">说明</span><span class="sxs-lookup"><span data-stu-id="583a7-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="583a7-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="583a7-112">**decimalPlaces**</span></span>  | <span data-ttu-id="583a7-113">string</span><span class="sxs-lookup"><span data-stu-id="583a7-113">string</span></span> | <span data-ttu-id="583a7-114">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="583a7-114">How many decimal places to display.</span></span> <span data-ttu-id="583a7-115">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="583a7-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="583a7-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="583a7-116">**displayAs**</span></span>      | <span data-ttu-id="583a7-117">string</span><span class="sxs-lookup"><span data-stu-id="583a7-117">string</span></span> | <span data-ttu-id="583a7-118">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="583a7-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="583a7-119">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="583a7-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="583a7-120">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="583a7-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="583a7-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="583a7-121">**maximum**</span></span>        | <span data-ttu-id="583a7-122">double</span><span class="sxs-lookup"><span data-stu-id="583a7-122">double</span></span> | <span data-ttu-id="583a7-123">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="583a7-123">The maximum permitted value.</span></span>
| <span data-ttu-id="583a7-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="583a7-124">**minimum**</span></span>        | <span data-ttu-id="583a7-125">double</span><span class="sxs-lookup"><span data-stu-id="583a7-125">double</span></span> | <span data-ttu-id="583a7-126">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="583a7-126">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="583a7-127">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="583a7-127">DecimalPlaces</span></span>

| <span data-ttu-id="583a7-128">值</span><span class="sxs-lookup"><span data-stu-id="583a7-128">Value</span></span>          | <span data-ttu-id="583a7-129">说明</span><span class="sxs-lookup"><span data-stu-id="583a7-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="583a7-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="583a7-130">**automatic**</span></span>  | <span data-ttu-id="583a7-131">默认值。</span><span class="sxs-lookup"><span data-stu-id="583a7-131">Default.</span></span> <span data-ttu-id="583a7-132">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="583a7-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="583a7-133">**none**</span><span class="sxs-lookup"><span data-stu-id="583a7-133">**none**</span></span>       | <span data-ttu-id="583a7-134">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="583a7-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="583a7-135">**one**</span><span class="sxs-lookup"><span data-stu-id="583a7-135">**one**</span></span>        | <span data-ttu-id="583a7-136">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="583a7-136">Always display one decimal place.</span></span>
| <span data-ttu-id="583a7-137">**two**</span><span class="sxs-lookup"><span data-stu-id="583a7-137">**two**</span></span>        | <span data-ttu-id="583a7-138">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="583a7-138">Always display two decimal places.</span></span>
| <span data-ttu-id="583a7-139">**three**</span><span class="sxs-lookup"><span data-stu-id="583a7-139">**three**</span></span>      | <span data-ttu-id="583a7-140">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="583a7-140">Always display three decimal places.</span></span>
| <span data-ttu-id="583a7-141">**four**</span><span class="sxs-lookup"><span data-stu-id="583a7-141">**four**</span></span>       | <span data-ttu-id="583a7-142">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="583a7-142">Always display four decimal places.</span></span>
| <span data-ttu-id="583a7-143">**five**</span><span class="sxs-lookup"><span data-stu-id="583a7-143">**five**</span></span>       | <span data-ttu-id="583a7-144">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="583a7-144">Always display five decimal places.</span></span>

<span data-ttu-id="583a7-145">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="583a7-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="583a7-146">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="583a7-146">These properties may be updated.</span></span>

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

