---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 3bc5ef0c2764fc941959a69ae58402ce3717e7b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010891"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="db6c4-102">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="db6c4-102">NumberColumn resource type</span></span>

<span data-ttu-id="db6c4-103">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="db6c4-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db6c4-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db6c4-104">JSON representation</span></span>

<span data-ttu-id="db6c4-105">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db6c4-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="db6c4-106">属性</span><span class="sxs-lookup"><span data-stu-id="db6c4-106">Properties</span></span>

| <span data-ttu-id="db6c4-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="db6c4-107">Property name</span></span>      | <span data-ttu-id="db6c4-108">类型</span><span class="sxs-lookup"><span data-stu-id="db6c4-108">Type</span></span>   | <span data-ttu-id="db6c4-109">说明</span><span class="sxs-lookup"><span data-stu-id="db6c4-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="db6c4-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="db6c4-110">**decimalPlaces**</span></span>  | <span data-ttu-id="db6c4-111">string</span><span class="sxs-lookup"><span data-stu-id="db6c4-111">string</span></span> | <span data-ttu-id="db6c4-112">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="db6c4-112">How many decimal places to display.</span></span> <span data-ttu-id="db6c4-113">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="db6c4-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="db6c4-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="db6c4-114">**displayAs**</span></span>      | <span data-ttu-id="db6c4-115">string</span><span class="sxs-lookup"><span data-stu-id="db6c4-115">string</span></span> | <span data-ttu-id="db6c4-116">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="db6c4-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="db6c4-117">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="db6c4-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="db6c4-118">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="db6c4-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="db6c4-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="db6c4-119">**maximum**</span></span>        | <span data-ttu-id="db6c4-120">double</span><span class="sxs-lookup"><span data-stu-id="db6c4-120">double</span></span> | <span data-ttu-id="db6c4-121">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="db6c4-121">The maximum permitted value.</span></span>
| <span data-ttu-id="db6c4-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="db6c4-122">**minimum**</span></span>        | <span data-ttu-id="db6c4-123">double</span><span class="sxs-lookup"><span data-stu-id="db6c4-123">double</span></span> | <span data-ttu-id="db6c4-124">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="db6c4-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="db6c4-125">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="db6c4-125">DecimalPlaces</span></span>

| <span data-ttu-id="db6c4-126">值</span><span class="sxs-lookup"><span data-stu-id="db6c4-126">Value</span></span>          | <span data-ttu-id="db6c4-127">说明</span><span class="sxs-lookup"><span data-stu-id="db6c4-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="db6c4-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="db6c4-128">**automatic**</span></span>  | <span data-ttu-id="db6c4-129">默认值。</span><span class="sxs-lookup"><span data-stu-id="db6c4-129">Default.</span></span> <span data-ttu-id="db6c4-130">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="db6c4-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="db6c4-131">**none**</span><span class="sxs-lookup"><span data-stu-id="db6c4-131">**none**</span></span>       | <span data-ttu-id="db6c4-132">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="db6c4-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="db6c4-133">**one**</span><span class="sxs-lookup"><span data-stu-id="db6c4-133">**one**</span></span>        | <span data-ttu-id="db6c4-134">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="db6c4-134">Always display one decimal place.</span></span>
| <span data-ttu-id="db6c4-135">**two**</span><span class="sxs-lookup"><span data-stu-id="db6c4-135">**two**</span></span>        | <span data-ttu-id="db6c4-136">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="db6c4-136">Always display two decimal places.</span></span>
| <span data-ttu-id="db6c4-137">**three**</span><span class="sxs-lookup"><span data-stu-id="db6c4-137">**three**</span></span>      | <span data-ttu-id="db6c4-138">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="db6c4-138">Always display three decimal places.</span></span>
| <span data-ttu-id="db6c4-139">**four**</span><span class="sxs-lookup"><span data-stu-id="db6c4-139">**four**</span></span>       | <span data-ttu-id="db6c4-140">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="db6c4-140">Always display four decimal places.</span></span>
| <span data-ttu-id="db6c4-141">**five**</span><span class="sxs-lookup"><span data-stu-id="db6c4-141">**five**</span></span>       | <span data-ttu-id="db6c4-142">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="db6c4-142">Always display five decimal places.</span></span>

<span data-ttu-id="db6c4-143">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="db6c4-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="db6c4-144">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="db6c4-144">These properties may be updated.</span></span>

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
