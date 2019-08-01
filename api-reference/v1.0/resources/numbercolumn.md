---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: columnDefinition 资源上的 numberColumn 指示该列的值为数字。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9196e2508ed3109ee56c24ad72943ca50aed11bc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035967"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="5b50f-103">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b50f-103">NumberColumn resource type</span></span>

<span data-ttu-id="5b50f-104">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="5b50f-104">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b50f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b50f-105">JSON representation</span></span>

<span data-ttu-id="5b50f-106">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b50f-106">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="5b50f-107">属性</span><span class="sxs-lookup"><span data-stu-id="5b50f-107">Properties</span></span>

| <span data-ttu-id="5b50f-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="5b50f-108">Property name</span></span>      | <span data-ttu-id="5b50f-109">类型</span><span class="sxs-lookup"><span data-stu-id="5b50f-109">Type</span></span>   | <span data-ttu-id="5b50f-110">说明</span><span class="sxs-lookup"><span data-stu-id="5b50f-110">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="5b50f-111">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="5b50f-111">**decimalPlaces**</span></span>  | <span data-ttu-id="5b50f-112">string</span><span class="sxs-lookup"><span data-stu-id="5b50f-112">string</span></span> | <span data-ttu-id="5b50f-113">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="5b50f-113">How many decimal places to display.</span></span> <span data-ttu-id="5b50f-114">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="5b50f-114">See below for information about the possible values.</span></span>
| <span data-ttu-id="5b50f-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="5b50f-115">**displayAs**</span></span>      | <span data-ttu-id="5b50f-116">string</span><span class="sxs-lookup"><span data-stu-id="5b50f-116">string</span></span> | <span data-ttu-id="5b50f-117">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="5b50f-117">How the value should be presented in the UX.</span></span> <span data-ttu-id="5b50f-118">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="5b50f-118">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="5b50f-119">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="5b50f-119">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="5b50f-120">**maximum**</span><span class="sxs-lookup"><span data-stu-id="5b50f-120">**maximum**</span></span>        | <span data-ttu-id="5b50f-121">double</span><span class="sxs-lookup"><span data-stu-id="5b50f-121">double</span></span> | <span data-ttu-id="5b50f-122">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="5b50f-122">The maximum permitted value.</span></span>
| <span data-ttu-id="5b50f-123">**minimum**</span><span class="sxs-lookup"><span data-stu-id="5b50f-123">**minimum**</span></span>        | <span data-ttu-id="5b50f-124">double</span><span class="sxs-lookup"><span data-stu-id="5b50f-124">double</span></span> | <span data-ttu-id="5b50f-125">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="5b50f-125">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="5b50f-126">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="5b50f-126">DecimalPlaces</span></span>

| <span data-ttu-id="5b50f-127">值</span><span class="sxs-lookup"><span data-stu-id="5b50f-127">Value</span></span>          | <span data-ttu-id="5b50f-128">说明</span><span class="sxs-lookup"><span data-stu-id="5b50f-128">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="5b50f-129">**automatic**</span><span class="sxs-lookup"><span data-stu-id="5b50f-129">**automatic**</span></span>  | <span data-ttu-id="5b50f-130">默认值。</span><span class="sxs-lookup"><span data-stu-id="5b50f-130">Default.</span></span> <span data-ttu-id="5b50f-131">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="5b50f-131">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="5b50f-132">**none**</span><span class="sxs-lookup"><span data-stu-id="5b50f-132">**none**</span></span>       | <span data-ttu-id="5b50f-133">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="5b50f-133">Do not display any decimal places.</span></span>
| <span data-ttu-id="5b50f-134">**one**</span><span class="sxs-lookup"><span data-stu-id="5b50f-134">**one**</span></span>        | <span data-ttu-id="5b50f-135">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="5b50f-135">Always display one decimal place.</span></span>
| <span data-ttu-id="5b50f-136">**two**</span><span class="sxs-lookup"><span data-stu-id="5b50f-136">**two**</span></span>        | <span data-ttu-id="5b50f-137">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="5b50f-137">Always display two decimal places.</span></span>
| <span data-ttu-id="5b50f-138">**three**</span><span class="sxs-lookup"><span data-stu-id="5b50f-138">**three**</span></span>      | <span data-ttu-id="5b50f-139">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="5b50f-139">Always display three decimal places.</span></span>
| <span data-ttu-id="5b50f-140">**four**</span><span class="sxs-lookup"><span data-stu-id="5b50f-140">**four**</span></span>       | <span data-ttu-id="5b50f-141">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="5b50f-141">Always display four decimal places.</span></span>
| <span data-ttu-id="5b50f-142">**five**</span><span class="sxs-lookup"><span data-stu-id="5b50f-142">**five**</span></span>       | <span data-ttu-id="5b50f-143">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="5b50f-143">Always display five decimal places.</span></span>

<span data-ttu-id="5b50f-144">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="5b50f-144">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="5b50f-145">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="5b50f-145">These properties may be updated.</span></span>

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
