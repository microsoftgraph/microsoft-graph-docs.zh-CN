---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 4aaff6539fc9c7ce77029463562c0f8fca57cac6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266504"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="0225d-102">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="0225d-102">NumberColumn resource type</span></span>

<span data-ttu-id="0225d-103">[columnDefinition](columnDefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="0225d-103">The **numberColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0225d-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0225d-104">JSON representation</span></span>

<span data-ttu-id="0225d-105">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0225d-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="0225d-106">属性</span><span class="sxs-lookup"><span data-stu-id="0225d-106">Properties</span></span>

| <span data-ttu-id="0225d-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="0225d-107">Property name</span></span>      | <span data-ttu-id="0225d-108">类型</span><span class="sxs-lookup"><span data-stu-id="0225d-108">Type</span></span>   | <span data-ttu-id="0225d-109">说明</span><span class="sxs-lookup"><span data-stu-id="0225d-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="0225d-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="0225d-110">**decimalPlaces**</span></span>  | <span data-ttu-id="0225d-111">字符串</span><span class="sxs-lookup"><span data-stu-id="0225d-111">string</span></span> | <span data-ttu-id="0225d-112">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="0225d-112">How many decimal places to display.</span></span> <span data-ttu-id="0225d-113">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="0225d-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="0225d-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="0225d-114">**displayAs**</span></span>      | <span data-ttu-id="0225d-115">字符串</span><span class="sxs-lookup"><span data-stu-id="0225d-115">string</span></span> | <span data-ttu-id="0225d-116">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="0225d-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="0225d-117">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="0225d-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="0225d-118">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="0225d-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="0225d-119">**最大值**</span><span class="sxs-lookup"><span data-stu-id="0225d-119">**maximum**</span></span>        | <span data-ttu-id="0225d-120">翻倍</span><span class="sxs-lookup"><span data-stu-id="0225d-120">double</span></span> | <span data-ttu-id="0225d-121">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="0225d-121">The maximum permitted value.</span></span>
| <span data-ttu-id="0225d-122">**最小值**</span><span class="sxs-lookup"><span data-stu-id="0225d-122">**minimum**</span></span>        | <span data-ttu-id="0225d-123">翻倍</span><span class="sxs-lookup"><span data-stu-id="0225d-123">double</span></span> | <span data-ttu-id="0225d-124">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="0225d-124">The minimum permitted value.</span></span>

## <a name="decimalplaces"></a><span data-ttu-id="0225d-125">DecimalPlaces</span><span class="sxs-lookup"><span data-stu-id="0225d-125">decimalPlaces</span></span>

| <span data-ttu-id="0225d-126">值</span><span class="sxs-lookup"><span data-stu-id="0225d-126">Value</span></span>          | <span data-ttu-id="0225d-127">说明</span><span class="sxs-lookup"><span data-stu-id="0225d-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="0225d-128">**自动的**</span><span class="sxs-lookup"><span data-stu-id="0225d-128">**automatic**</span></span>  | <span data-ttu-id="0225d-129">默认值。</span><span class="sxs-lookup"><span data-stu-id="0225d-129">Default.</span></span> <span data-ttu-id="0225d-130">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="0225d-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="0225d-131">**无**</span><span class="sxs-lookup"><span data-stu-id="0225d-131">**none**</span></span>       | <span data-ttu-id="0225d-132">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="0225d-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="0225d-133">**一**</span><span class="sxs-lookup"><span data-stu-id="0225d-133">**one**</span></span>        | <span data-ttu-id="0225d-134">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="0225d-134">Always display one decimal place.</span></span>
| <span data-ttu-id="0225d-135">**二**</span><span class="sxs-lookup"><span data-stu-id="0225d-135">**two**</span></span>        | <span data-ttu-id="0225d-136">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="0225d-136">Always display two decimal places.</span></span>
| <span data-ttu-id="0225d-137">**三**</span><span class="sxs-lookup"><span data-stu-id="0225d-137">**three**</span></span>      | <span data-ttu-id="0225d-138">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="0225d-138">Always display three decimal places.</span></span>
| <span data-ttu-id="0225d-139">**四**</span><span class="sxs-lookup"><span data-stu-id="0225d-139">**four**</span></span>       | <span data-ttu-id="0225d-140">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="0225d-140">Always display four decimal places.</span></span>
| <span data-ttu-id="0225d-141">**五**</span><span class="sxs-lookup"><span data-stu-id="0225d-141">**five**</span></span>       | <span data-ttu-id="0225d-142">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="0225d-142">Always display five decimal places.</span></span>

<span data-ttu-id="0225d-143">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="0225d-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="0225d-144">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="0225d-144">These properties may be updated.</span></span>

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
