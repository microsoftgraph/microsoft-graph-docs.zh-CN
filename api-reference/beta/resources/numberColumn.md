---
author: JeremyKelley
description: columnDefinition 资源上的 numberColumn 指示该列的值为数字。
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0f6ed1c8aca8909b50f47f539e0569a4b68dad89
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522545"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="edabd-103">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="edabd-103">NumberColumn resource type</span></span>

<span data-ttu-id="edabd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="edabd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edabd-105">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="edabd-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="edabd-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edabd-106">JSON representation</span></span>

<span data-ttu-id="edabd-107">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edabd-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="edabd-108">属性</span><span class="sxs-lookup"><span data-stu-id="edabd-108">Properties</span></span>

| <span data-ttu-id="edabd-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="edabd-109">Property name</span></span>      | <span data-ttu-id="edabd-110">类型</span><span class="sxs-lookup"><span data-stu-id="edabd-110">Type</span></span>   | <span data-ttu-id="edabd-111">说明</span><span class="sxs-lookup"><span data-stu-id="edabd-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="edabd-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="edabd-112">**decimalPlaces**</span></span>  | <span data-ttu-id="edabd-113">string</span><span class="sxs-lookup"><span data-stu-id="edabd-113">string</span></span> | <span data-ttu-id="edabd-114">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="edabd-114">How many decimal places to display.</span></span> <span data-ttu-id="edabd-115">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="edabd-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="edabd-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="edabd-116">**displayAs**</span></span>      | <span data-ttu-id="edabd-117">string</span><span class="sxs-lookup"><span data-stu-id="edabd-117">string</span></span> | <span data-ttu-id="edabd-118">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="edabd-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="edabd-119">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="edabd-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="edabd-120">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="edabd-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="edabd-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="edabd-121">**maximum**</span></span>        | <span data-ttu-id="edabd-122">double</span><span class="sxs-lookup"><span data-stu-id="edabd-122">double</span></span> | <span data-ttu-id="edabd-123">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="edabd-123">The maximum permitted value.</span></span>
| <span data-ttu-id="edabd-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="edabd-124">**minimum**</span></span>        | <span data-ttu-id="edabd-125">double</span><span class="sxs-lookup"><span data-stu-id="edabd-125">double</span></span> | <span data-ttu-id="edabd-126">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="edabd-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="edabd-127">DecimalPlaces 值</span><span class="sxs-lookup"><span data-stu-id="edabd-127">DecimalPlaces values</span></span>

| <span data-ttu-id="edabd-128">值</span><span class="sxs-lookup"><span data-stu-id="edabd-128">Value</span></span>          | <span data-ttu-id="edabd-129">说明</span><span class="sxs-lookup"><span data-stu-id="edabd-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="edabd-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="edabd-130">**automatic**</span></span>  | <span data-ttu-id="edabd-131">默认值。</span><span class="sxs-lookup"><span data-stu-id="edabd-131">Default.</span></span> <span data-ttu-id="edabd-132">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="edabd-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="edabd-133">**none**</span><span class="sxs-lookup"><span data-stu-id="edabd-133">**none**</span></span>       | <span data-ttu-id="edabd-134">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="edabd-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="edabd-135">**one**</span><span class="sxs-lookup"><span data-stu-id="edabd-135">**one**</span></span>        | <span data-ttu-id="edabd-136">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="edabd-136">Always display one decimal place.</span></span>
| <span data-ttu-id="edabd-137">**two**</span><span class="sxs-lookup"><span data-stu-id="edabd-137">**two**</span></span>        | <span data-ttu-id="edabd-138">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="edabd-138">Always display two decimal places.</span></span>
| <span data-ttu-id="edabd-139">**three**</span><span class="sxs-lookup"><span data-stu-id="edabd-139">**three**</span></span>      | <span data-ttu-id="edabd-140">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="edabd-140">Always display three decimal places.</span></span>
| <span data-ttu-id="edabd-141">**four**</span><span class="sxs-lookup"><span data-stu-id="edabd-141">**four**</span></span>       | <span data-ttu-id="edabd-142">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="edabd-142">Always display four decimal places.</span></span>
| <span data-ttu-id="edabd-143">**five**</span><span class="sxs-lookup"><span data-stu-id="edabd-143">**five**</span></span>       | <span data-ttu-id="edabd-144">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="edabd-144">Always display five decimal places.</span></span>

<span data-ttu-id="edabd-145">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="edabd-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="edabd-146">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="edabd-146">These properties may be updated.</span></span>

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
