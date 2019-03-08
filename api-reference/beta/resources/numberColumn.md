---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: edd495b62f0ccbd163ec31a2efca70923d0bc8ad
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480766"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="fca3e-102">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="fca3e-102">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fca3e-103">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="fca3e-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fca3e-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fca3e-104">JSON representation</span></span>

<span data-ttu-id="fca3e-105">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fca3e-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="fca3e-106">属性</span><span class="sxs-lookup"><span data-stu-id="fca3e-106">Properties</span></span>

| <span data-ttu-id="fca3e-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="fca3e-107">Property name</span></span>      | <span data-ttu-id="fca3e-108">类型</span><span class="sxs-lookup"><span data-stu-id="fca3e-108">Type</span></span>   | <span data-ttu-id="fca3e-109">说明</span><span class="sxs-lookup"><span data-stu-id="fca3e-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="fca3e-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="fca3e-110">**decimalPlaces**</span></span>  | <span data-ttu-id="fca3e-111">string</span><span class="sxs-lookup"><span data-stu-id="fca3e-111">string</span></span> | <span data-ttu-id="fca3e-112">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="fca3e-112">How many decimal places to display.</span></span> <span data-ttu-id="fca3e-113">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="fca3e-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="fca3e-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="fca3e-114">**displayAs**</span></span>      | <span data-ttu-id="fca3e-115">string</span><span class="sxs-lookup"><span data-stu-id="fca3e-115">string</span></span> | <span data-ttu-id="fca3e-116">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="fca3e-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="fca3e-117">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="fca3e-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="fca3e-118">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="fca3e-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="fca3e-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="fca3e-119">**maximum**</span></span>        | <span data-ttu-id="fca3e-120">double</span><span class="sxs-lookup"><span data-stu-id="fca3e-120">double</span></span> | <span data-ttu-id="fca3e-121">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="fca3e-121">The maximum permitted value.</span></span>
| <span data-ttu-id="fca3e-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="fca3e-122">**minimum**</span></span>        | <span data-ttu-id="fca3e-123">double</span><span class="sxs-lookup"><span data-stu-id="fca3e-123">double</span></span> | <span data-ttu-id="fca3e-124">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="fca3e-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="fca3e-125">DecimalPlaces 值</span><span class="sxs-lookup"><span data-stu-id="fca3e-125">DecimalPlaces values</span></span>

| <span data-ttu-id="fca3e-126">值</span><span class="sxs-lookup"><span data-stu-id="fca3e-126">Value</span></span>          | <span data-ttu-id="fca3e-127">说明</span><span class="sxs-lookup"><span data-stu-id="fca3e-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="fca3e-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="fca3e-128">**automatic**</span></span>  | <span data-ttu-id="fca3e-129">默认值。</span><span class="sxs-lookup"><span data-stu-id="fca3e-129">Default.</span></span> <span data-ttu-id="fca3e-130">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="fca3e-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="fca3e-131">**none**</span><span class="sxs-lookup"><span data-stu-id="fca3e-131">**none**</span></span>       | <span data-ttu-id="fca3e-132">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="fca3e-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="fca3e-133">**one**</span><span class="sxs-lookup"><span data-stu-id="fca3e-133">**one**</span></span>        | <span data-ttu-id="fca3e-134">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="fca3e-134">Always display one decimal place.</span></span>
| <span data-ttu-id="fca3e-135">**two**</span><span class="sxs-lookup"><span data-stu-id="fca3e-135">**two**</span></span>        | <span data-ttu-id="fca3e-136">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="fca3e-136">Always display two decimal places.</span></span>
| <span data-ttu-id="fca3e-137">**three**</span><span class="sxs-lookup"><span data-stu-id="fca3e-137">**three**</span></span>      | <span data-ttu-id="fca3e-138">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="fca3e-138">Always display three decimal places.</span></span>
| <span data-ttu-id="fca3e-139">**four**</span><span class="sxs-lookup"><span data-stu-id="fca3e-139">**four**</span></span>       | <span data-ttu-id="fca3e-140">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="fca3e-140">Always display four decimal places.</span></span>
| <span data-ttu-id="fca3e-141">**five**</span><span class="sxs-lookup"><span data-stu-id="fca3e-141">**five**</span></span>       | <span data-ttu-id="fca3e-142">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="fca3e-142">Always display five decimal places.</span></span>

<span data-ttu-id="fca3e-143">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="fca3e-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="fca3e-144">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="fca3e-144">These properties may be updated.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/numberColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
