---
author: JeremyKelley
description: columnDefinition 资源上的 numberColumn 指示该列的值为数字。
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 49c3dce15297187bcda20e20ae339dba86d154db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988953"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="bbf0b-103">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="bbf0b-103">NumberColumn resource type</span></span>

<span data-ttu-id="bbf0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbf0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbf0b-105">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbf0b-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bbf0b-106">JSON representation</span></span>

<span data-ttu-id="bbf0b-107">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="bbf0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="bbf0b-108">Properties</span></span>

| <span data-ttu-id="bbf0b-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="bbf0b-109">Property name</span></span>      | <span data-ttu-id="bbf0b-110">类型</span><span class="sxs-lookup"><span data-stu-id="bbf0b-110">Type</span></span>   | <span data-ttu-id="bbf0b-111">说明</span><span class="sxs-lookup"><span data-stu-id="bbf0b-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="bbf0b-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-112">**decimalPlaces**</span></span>  | <span data-ttu-id="bbf0b-113">string</span><span class="sxs-lookup"><span data-stu-id="bbf0b-113">string</span></span> | <span data-ttu-id="bbf0b-114">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-114">How many decimal places to display.</span></span> <span data-ttu-id="bbf0b-115">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="bbf0b-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-116">**displayAs**</span></span>      | <span data-ttu-id="bbf0b-117">string</span><span class="sxs-lookup"><span data-stu-id="bbf0b-117">string</span></span> | <span data-ttu-id="bbf0b-118">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="bbf0b-119">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="bbf0b-120">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="bbf0b-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-121">**maximum**</span></span>        | <span data-ttu-id="bbf0b-122">double</span><span class="sxs-lookup"><span data-stu-id="bbf0b-122">double</span></span> | <span data-ttu-id="bbf0b-123">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-123">The maximum permitted value.</span></span>
| <span data-ttu-id="bbf0b-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-124">**minimum**</span></span>        | <span data-ttu-id="bbf0b-125">double</span><span class="sxs-lookup"><span data-stu-id="bbf0b-125">double</span></span> | <span data-ttu-id="bbf0b-126">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="bbf0b-127">DecimalPlaces 值</span><span class="sxs-lookup"><span data-stu-id="bbf0b-127">DecimalPlaces values</span></span>

| <span data-ttu-id="bbf0b-128">值</span><span class="sxs-lookup"><span data-stu-id="bbf0b-128">Value</span></span>          | <span data-ttu-id="bbf0b-129">说明</span><span class="sxs-lookup"><span data-stu-id="bbf0b-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="bbf0b-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-130">**automatic**</span></span>  | <span data-ttu-id="bbf0b-131">默认值。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-131">Default.</span></span> <span data-ttu-id="bbf0b-132">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="bbf0b-133">**none**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-133">**none**</span></span>       | <span data-ttu-id="bbf0b-134">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="bbf0b-135">**one**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-135">**one**</span></span>        | <span data-ttu-id="bbf0b-136">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-136">Always display one decimal place.</span></span>
| <span data-ttu-id="bbf0b-137">**two**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-137">**two**</span></span>        | <span data-ttu-id="bbf0b-138">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-138">Always display two decimal places.</span></span>
| <span data-ttu-id="bbf0b-139">**three**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-139">**three**</span></span>      | <span data-ttu-id="bbf0b-140">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-140">Always display three decimal places.</span></span>
| <span data-ttu-id="bbf0b-141">**four**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-141">**four**</span></span>       | <span data-ttu-id="bbf0b-142">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-142">Always display four decimal places.</span></span>
| <span data-ttu-id="bbf0b-143">**five**</span><span class="sxs-lookup"><span data-stu-id="bbf0b-143">**five**</span></span>       | <span data-ttu-id="bbf0b-144">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-144">Always display five decimal places.</span></span>

<span data-ttu-id="bbf0b-145">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="bbf0b-146">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="bbf0b-146">These properties may be updated.</span></span>

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


