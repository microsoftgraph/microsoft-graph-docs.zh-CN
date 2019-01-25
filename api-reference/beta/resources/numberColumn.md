---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: cf1f6c6cafd23a5503d645d13e597a8941019fee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512876"
---
# <a name="numbercolumn-resource-type"></a><span data-ttu-id="e3039-102">NumberColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3039-102">NumberColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3039-103">[columnDefinition](columndefinition.md) 资源上的 **numberColumn** 指示该列的值为数字。</span><span class="sxs-lookup"><span data-stu-id="e3039-103">The **numberColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are numbers.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3039-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3039-104">JSON representation</span></span>

<span data-ttu-id="e3039-105">下面是 **numberColumn** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3039-105">Here is a JSON representation of a **numberColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a><span data-ttu-id="e3039-106">属性</span><span class="sxs-lookup"><span data-stu-id="e3039-106">Properties</span></span>

| <span data-ttu-id="e3039-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="e3039-107">Property name</span></span>      | <span data-ttu-id="e3039-108">类型</span><span class="sxs-lookup"><span data-stu-id="e3039-108">Type</span></span>   | <span data-ttu-id="e3039-109">说明</span><span class="sxs-lookup"><span data-stu-id="e3039-109">Description</span></span>
|:-------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="e3039-110">**decimalPlaces**</span><span class="sxs-lookup"><span data-stu-id="e3039-110">**decimalPlaces**</span></span>  | <span data-ttu-id="e3039-111">string</span><span class="sxs-lookup"><span data-stu-id="e3039-111">string</span></span> | <span data-ttu-id="e3039-112">要显示的小数位数。</span><span class="sxs-lookup"><span data-stu-id="e3039-112">How many decimal places to display.</span></span> <span data-ttu-id="e3039-113">有关可能的值的信息，请参阅以下信息。</span><span class="sxs-lookup"><span data-stu-id="e3039-113">See below for information about the possible values.</span></span>
| <span data-ttu-id="e3039-114">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="e3039-114">**displayAs**</span></span>      | <span data-ttu-id="e3039-115">string</span><span class="sxs-lookup"><span data-stu-id="e3039-115">string</span></span> | <span data-ttu-id="e3039-116">值在用户体验中的显示方式。</span><span class="sxs-lookup"><span data-stu-id="e3039-116">How the value should be presented in the UX.</span></span> <span data-ttu-id="e3039-117">必须为 `number` 或 `percentage` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="e3039-117">Must be one of `number` or `percentage`.</span></span> <span data-ttu-id="e3039-118">如果未指定，则视为 `number`。</span><span class="sxs-lookup"><span data-stu-id="e3039-118">If unspecified, treated as `number`.</span></span>
| <span data-ttu-id="e3039-119">**maximum**</span><span class="sxs-lookup"><span data-stu-id="e3039-119">**maximum**</span></span>        | <span data-ttu-id="e3039-120">double</span><span class="sxs-lookup"><span data-stu-id="e3039-120">double</span></span> | <span data-ttu-id="e3039-121">最大允许值。</span><span class="sxs-lookup"><span data-stu-id="e3039-121">The maximum permitted value.</span></span>
| <span data-ttu-id="e3039-122">**minimum**</span><span class="sxs-lookup"><span data-stu-id="e3039-122">**minimum**</span></span>        | <span data-ttu-id="e3039-123">double</span><span class="sxs-lookup"><span data-stu-id="e3039-123">double</span></span> | <span data-ttu-id="e3039-124">最小允许值。</span><span class="sxs-lookup"><span data-stu-id="e3039-124">The minimum permitted value.</span></span>

## <a name="decimalplaces-values"></a><span data-ttu-id="e3039-125">DecimalPlaces 值</span><span class="sxs-lookup"><span data-stu-id="e3039-125">DecimalPlaces values</span></span>

| <span data-ttu-id="e3039-126">值</span><span class="sxs-lookup"><span data-stu-id="e3039-126">Value</span></span>          | <span data-ttu-id="e3039-127">说明</span><span class="sxs-lookup"><span data-stu-id="e3039-127">Description</span></span>
|:---------------|:--------------------------------------------------------------
| <span data-ttu-id="e3039-128">**automatic**</span><span class="sxs-lookup"><span data-stu-id="e3039-128">**automatic**</span></span>  | <span data-ttu-id="e3039-129">默认值。</span><span class="sxs-lookup"><span data-stu-id="e3039-129">Default.</span></span> <span data-ttu-id="e3039-130">根据需要自动显示小数位数。</span><span class="sxs-lookup"><span data-stu-id="e3039-130">Automatically display decimal places as needed.</span></span>
| <span data-ttu-id="e3039-131">**none**</span><span class="sxs-lookup"><span data-stu-id="e3039-131">**none**</span></span>       | <span data-ttu-id="e3039-132">不显示任何小数位数。</span><span class="sxs-lookup"><span data-stu-id="e3039-132">Do not display any decimal places.</span></span>
| <span data-ttu-id="e3039-133">**one**</span><span class="sxs-lookup"><span data-stu-id="e3039-133">**one**</span></span>        | <span data-ttu-id="e3039-134">显示一位小数位数。</span><span class="sxs-lookup"><span data-stu-id="e3039-134">Always display one decimal place.</span></span>
| <span data-ttu-id="e3039-135">**two**</span><span class="sxs-lookup"><span data-stu-id="e3039-135">**two**</span></span>        | <span data-ttu-id="e3039-136">显示两位小数位数。</span><span class="sxs-lookup"><span data-stu-id="e3039-136">Always display two decimal places.</span></span>
| <span data-ttu-id="e3039-137">**three**</span><span class="sxs-lookup"><span data-stu-id="e3039-137">**three**</span></span>      | <span data-ttu-id="e3039-138">显示三位小数位数。</span><span class="sxs-lookup"><span data-stu-id="e3039-138">Always display three decimal places.</span></span>
| <span data-ttu-id="e3039-139">**four**</span><span class="sxs-lookup"><span data-stu-id="e3039-139">**four**</span></span>       | <span data-ttu-id="e3039-140">显示四位小数位数。</span><span class="sxs-lookup"><span data-stu-id="e3039-140">Always display four decimal places.</span></span>
| <span data-ttu-id="e3039-141">**five**</span><span class="sxs-lookup"><span data-stu-id="e3039-141">**five**</span></span>       | <span data-ttu-id="e3039-142">显示五位小数位数。</span><span class="sxs-lookup"><span data-stu-id="e3039-142">Always display five decimal places.</span></span>

<span data-ttu-id="e3039-143">注意：**decimalPlaces** 和 **displayAs** 应用于数字的呈现方式，而不是存储方式。</span><span class="sxs-lookup"><span data-stu-id="e3039-143">Note: **decimalPlaces** and **displayAs** apply to how numbers are rendered, not stored.</span></span>
<span data-ttu-id="e3039-144">这些属性可能会更新。</span><span class="sxs-lookup"><span data-stu-id="e3039-144">These properties may be updated.</span></span>

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
