---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 27d17d3e9b9d3d1debcd20f2beb916222801ebe9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049097"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="3d4ce-102">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d4ce-102">NumberColumn resource type</span></span>

> <span data-ttu-id="3d4ce-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d4ce-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d4ce-105">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-105">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d4ce-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d4ce-106">JSON representation</span></span>

<span data-ttu-id="3d4ce-107">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-107">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="3d4ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="3d4ce-108">Properties</span></span>

| <span data-ttu-id="3d4ce-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="3d4ce-109">Property name</span></span>      | <span data-ttu-id="3d4ce-110">类型</span><span class="sxs-lookup"><span data-stu-id="3d4ce-110">Type</span></span>   | <span data-ttu-id="3d4ce-111">说明</span><span class="sxs-lookup"><span data-stu-id="3d4ce-111">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="3d4ce-112">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-112">**decimalPlaces**</span></span>  | <span data-ttu-id="3d4ce-113">string</span><span class="sxs-lookup"><span data-stu-id="3d4ce-113">string</span></span> | <span data-ttu-id="3d4ce-114">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-114">How many decimal places to display.</span></span> <span data-ttu-id="3d4ce-115">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-115">See below for information about the possible values.</span></span>
| <span data-ttu-id="3d4ce-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-116">**displayAs**</span></span>      | <span data-ttu-id="3d4ce-117">string</span><span class="sxs-lookup"><span data-stu-id="3d4ce-117">string</span></span> | <span data-ttu-id="3d4ce-118">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-118">How the value should be presented in the UX.</span></span> <span data-ttu-id="3d4ce-119">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-119">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="3d4ce-120">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-120">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="3d4ce-121">**maximum**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-121">**maximum**</span></span>        | <span data-ttu-id="3d4ce-122">double</span><span class="sxs-lookup"><span data-stu-id="3d4ce-122">double</span></span> | <span data-ttu-id="3d4ce-123">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-123">The maximum permitted value.</span></span>
| <span data-ttu-id="3d4ce-124">**minimum**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-124">**minimum**</span></span>        | <span data-ttu-id="3d4ce-125">double</span><span class="sxs-lookup"><span data-stu-id="3d4ce-125">double</span></span> | <span data-ttu-id="3d4ce-126">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-126">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="3d4ce-127">DecimalPlaces 值</span><span class="sxs-lookup"><span data-stu-id="3d4ce-127">DecimalPlaces values</span></span>

| <span data-ttu-id="3d4ce-128">值</span><span class="sxs-lookup"><span data-stu-id="3d4ce-128">Value</span></span>          | <span data-ttu-id="3d4ce-129">说明</span><span class="sxs-lookup"><span data-stu-id="3d4ce-129">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="3d4ce-130">**automatic**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-130">**automatic**</span></span>  | <span data-ttu-id="3d4ce-131">默认值。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-131">Default.</span></span> <span data-ttu-id="3d4ce-132">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-132">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="3d4ce-133">**none**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-133">**none**</span></span>       | <span data-ttu-id="3d4ce-134">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-134">Do not display any decimal places.</span></span>
| <span data-ttu-id="3d4ce-135">**one**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-135">**one**</span></span>        | <span data-ttu-id="3d4ce-136">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-136">Always display one decimal place.</span></span>
| <span data-ttu-id="3d4ce-137">**two**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-137">**two**</span></span>        | <span data-ttu-id="3d4ce-138">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-138">Always display two decimal places.</span></span>
| <span data-ttu-id="3d4ce-139">**three**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-139">**three**</span></span>      | <span data-ttu-id="3d4ce-140">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-140">Always display three decimal places.</span></span>
| <span data-ttu-id="3d4ce-141">**four**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-141">**four**</span></span>       | <span data-ttu-id="3d4ce-142">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-142">Always display four decimal places.</span></span>
| <span data-ttu-id="3d4ce-143">**five**</span><span class="sxs-lookup"><span data-stu-id="3d4ce-143">**five**</span></span>       | <span data-ttu-id="3d4ce-144">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-144">Always display five decimal places.</span></span>

<span data-ttu-id="3d4ce-145">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-145">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="3d4ce-146">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="3d4ce-146">These properties may be updated.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
