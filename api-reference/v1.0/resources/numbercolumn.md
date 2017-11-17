---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 8aa366e3c4f59fc5d22f945c863bab4f91373b67
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="339ad-102">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="339ad-102">NumberColumn resource type</span></span>

<span data-ttu-id="339ad-103">[columnDefinition](columnDefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="339ad-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="339ad-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="339ad-104">JSON representation</span></span>

<span data-ttu-id="339ad-105">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="339ad-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="339ad-106">属性</span><span class="sxs-lookup"><span data-stu-id="339ad-106">Properties</span></span>

| <span data-ttu-id="339ad-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="339ad-107">Property name</span></span>      | <span data-ttu-id="339ad-108">类型</span><span class="sxs-lookup"><span data-stu-id="339ad-108">Type</span></span>   | <span data-ttu-id="339ad-109">说明</span><span class="sxs-lookup"><span data-stu-id="339ad-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="339ad-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="339ad-110">**decimalPlaces**</span></span>  | <span data-ttu-id="339ad-111">string</span><span class="sxs-lookup"><span data-stu-id="339ad-111">string</span></span> | <span data-ttu-id="339ad-112">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="339ad-112">How many decimal places to display.</span></span> <span data-ttu-id="339ad-113">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="339ad-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="339ad-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="339ad-114">**displayAs**</span></span>      | <span data-ttu-id="339ad-115">string</span><span class="sxs-lookup"><span data-stu-id="339ad-115">string</span></span> | <span data-ttu-id="339ad-116">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="339ad-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="339ad-117">必须是 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="339ad-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="339ad-118">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="339ad-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="339ad-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="339ad-119">**maximum**</span></span>        | <span data-ttu-id="339ad-120">double</span><span class="sxs-lookup"><span data-stu-id="339ad-120">double</span></span> | <span data-ttu-id="339ad-121">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="339ad-121">The maximum permitted value.</span></span>
| <span data-ttu-id="339ad-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="339ad-122">**minimum**</span></span>        | <span data-ttu-id="339ad-123">double</span><span class="sxs-lookup"><span data-stu-id="339ad-123">double</span></span> | <span data-ttu-id="339ad-124">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="339ad-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="339ad-125">DecimalPlaces 值</span><span class="sxs-lookup"><span data-stu-id="339ad-125">DecimalPlaces values</span></span>

| <span data-ttu-id="339ad-126">值</span><span class="sxs-lookup"><span data-stu-id="339ad-126">Value</span></span>          | <span data-ttu-id="339ad-127">说明</span><span class="sxs-lookup"><span data-stu-id="339ad-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="339ad-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="339ad-128">**Automatic**</span></span>  | <span data-ttu-id="339ad-129">默认值。</span><span class="sxs-lookup"><span data-stu-id="339ad-129">Default.</span></span> <span data-ttu-id="339ad-130">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="339ad-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="339ad-131">**none**</span><span class="sxs-lookup"><span data-stu-id="339ad-131">**None**</span></span>       | <span data-ttu-id="339ad-132">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="339ad-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="339ad-133">**one**</span><span class="sxs-lookup"><span data-stu-id="339ad-133">**One**</span></span>        | <span data-ttu-id="339ad-134">始终显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="339ad-134">Always display one decimal place.</span></span>
| <span data-ttu-id="339ad-135">**two**</span><span class="sxs-lookup"><span data-stu-id="339ad-135">**Two**</span></span>        | <span data-ttu-id="339ad-136">始终显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="339ad-136">Always display two decimal places.</span></span>
| <span data-ttu-id="339ad-137">**three**</span><span class="sxs-lookup"><span data-stu-id="339ad-137">**Three**</span></span>      | <span data-ttu-id="339ad-138">始终显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="339ad-138">Always display three decimal places.</span></span>
| <span data-ttu-id="339ad-139">**four**</span><span class="sxs-lookup"><span data-stu-id="339ad-139">**Four**</span></span>       | <span data-ttu-id="339ad-140">始终显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="339ad-140">Always display four decimal places.</span></span>
| <span data-ttu-id="339ad-141">**five**</span><span class="sxs-lookup"><span data-stu-id="339ad-141">**five**</span></span>       | <span data-ttu-id="339ad-142">始终显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="339ad-142">Always display five decimal places.</span></span>

<span data-ttu-id="339ad-143">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="339ad-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="339ad-144">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="339ad-144">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
