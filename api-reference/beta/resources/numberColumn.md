---
author: JeremyKelley
description: columnDefinition 资源上的 numberColumn 指示该列的值为数字。
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c8abaca08682e4a68e8e5efbeb798a8810b20bfb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966634"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="f7b54-103">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7b54-103">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b54-104">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="f7b54-104">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7b54-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7b54-105">JSON representation</span></span>

<span data-ttu-id="f7b54-106">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7b54-106">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="f7b54-107">属性</span><span class="sxs-lookup"><span data-stu-id="f7b54-107">Properties</span></span>

| <span data-ttu-id="f7b54-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="f7b54-108">Property name</span></span>      | <span data-ttu-id="f7b54-109">类型</span><span class="sxs-lookup"><span data-stu-id="f7b54-109">Type</span></span>   | <span data-ttu-id="f7b54-110">说明</span><span class="sxs-lookup"><span data-stu-id="f7b54-110">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="f7b54-111">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="f7b54-111">**decimalPlaces**</span></span>  | <span data-ttu-id="f7b54-112">string</span><span class="sxs-lookup"><span data-stu-id="f7b54-112">string</span></span> | <span data-ttu-id="f7b54-113">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="f7b54-113">How many decimal places to display.</span></span> <span data-ttu-id="f7b54-114">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="f7b54-114">See below for information about the possible values.</span></span>
| <span data-ttu-id="f7b54-115">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="f7b54-115">**displayAs**</span></span>      | <span data-ttu-id="f7b54-116">string</span><span class="sxs-lookup"><span data-stu-id="f7b54-116">string</span></span> | <span data-ttu-id="f7b54-117">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="f7b54-117">How the value should be presented in the UX.</span></span> <span data-ttu-id="f7b54-118">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="f7b54-118">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="f7b54-119">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="f7b54-119">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="f7b54-120">**maximum**</span><span class="sxs-lookup"><span data-stu-id="f7b54-120">**maximum**</span></span>        | <span data-ttu-id="f7b54-121">double</span><span class="sxs-lookup"><span data-stu-id="f7b54-121">double</span></span> | <span data-ttu-id="f7b54-122">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="f7b54-122">The maximum permitted value.</span></span>
| <span data-ttu-id="f7b54-123">**minimum**</span><span class="sxs-lookup"><span data-stu-id="f7b54-123">**minimum**</span></span>        | <span data-ttu-id="f7b54-124">double</span><span class="sxs-lookup"><span data-stu-id="f7b54-124">double</span></span> | <span data-ttu-id="f7b54-125">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="f7b54-125">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="f7b54-126">DecimalPlaces 值</span><span class="sxs-lookup"><span data-stu-id="f7b54-126">DecimalPlaces values</span></span>

| <span data-ttu-id="f7b54-127">值</span><span class="sxs-lookup"><span data-stu-id="f7b54-127">Value</span></span>          | <span data-ttu-id="f7b54-128">说明</span><span class="sxs-lookup"><span data-stu-id="f7b54-128">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="f7b54-129">**automatic**</span><span class="sxs-lookup"><span data-stu-id="f7b54-129">**automatic**</span></span>  | <span data-ttu-id="f7b54-130">默认值。</span><span class="sxs-lookup"><span data-stu-id="f7b54-130">Default.</span></span> <span data-ttu-id="f7b54-131">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="f7b54-131">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="f7b54-132">**none**</span><span class="sxs-lookup"><span data-stu-id="f7b54-132">**none**</span></span>       | <span data-ttu-id="f7b54-133">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="f7b54-133">Do not display any decimal places.</span></span>
| <span data-ttu-id="f7b54-134">**one**</span><span class="sxs-lookup"><span data-stu-id="f7b54-134">**one**</span></span>        | <span data-ttu-id="f7b54-135">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="f7b54-135">Always display one decimal place.</span></span>
| <span data-ttu-id="f7b54-136">**two**</span><span class="sxs-lookup"><span data-stu-id="f7b54-136">**two**</span></span>        | <span data-ttu-id="f7b54-137">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="f7b54-137">Always display two decimal places.</span></span>
| <span data-ttu-id="f7b54-138">**three**</span><span class="sxs-lookup"><span data-stu-id="f7b54-138">**three**</span></span>      | <span data-ttu-id="f7b54-139">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="f7b54-139">Always display three decimal places.</span></span>
| <span data-ttu-id="f7b54-140">**four**</span><span class="sxs-lookup"><span data-stu-id="f7b54-140">**four**</span></span>       | <span data-ttu-id="f7b54-141">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="f7b54-141">Always display four decimal places.</span></span>
| <span data-ttu-id="f7b54-142">**five**</span><span class="sxs-lookup"><span data-stu-id="f7b54-142">**five**</span></span>       | <span data-ttu-id="f7b54-143">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="f7b54-143">Always display five decimal places.</span></span>

<span data-ttu-id="f7b54-144">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="f7b54-144">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="f7b54-145">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="f7b54-145">These properties may be updated.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": []
}
-->
