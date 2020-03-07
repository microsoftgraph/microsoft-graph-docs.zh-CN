---
title: RangeFormat 资源类型
description: 一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: edf239d5e14ca65ee4ae15f846182e5678f89f46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447015"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="94061-103">RangeFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="94061-103">RangeFormat resource type</span></span>

<span data-ttu-id="94061-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94061-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94061-105">一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。</span><span class="sxs-lookup"><span data-stu-id="94061-105">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="94061-106">Methods</span><span class="sxs-lookup"><span data-stu-id="94061-106">Methods</span></span>

| <span data-ttu-id="94061-107">方法</span><span class="sxs-lookup"><span data-stu-id="94061-107">Method</span></span>           | <span data-ttu-id="94061-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="94061-108">Return Type</span></span>    |<span data-ttu-id="94061-109">说明</span><span class="sxs-lookup"><span data-stu-id="94061-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94061-110">获取 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="94061-110">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="94061-111">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="94061-111">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="94061-112">读取 rangeFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94061-112">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="94061-113">创建 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="94061-113">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="94061-114">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="94061-114">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="94061-115">通过发布到边框集合创建新的 RangeBorder。</span><span class="sxs-lookup"><span data-stu-id="94061-115">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="94061-116">列出边框</span><span class="sxs-lookup"><span data-stu-id="94061-116">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="94061-117">[WorkbookRangeBorder](rangeborder.md)集合</span><span class="sxs-lookup"><span data-stu-id="94061-117">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="94061-118">获取 RangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="94061-118">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="94061-119">更新</span><span class="sxs-lookup"><span data-stu-id="94061-119">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="94061-120">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="94061-120">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="94061-121">更新 RangeFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="94061-121">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="94061-122">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="94061-122">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="94061-123">无</span><span class="sxs-lookup"><span data-stu-id="94061-123">None</span></span>|<span data-ttu-id="94061-124">根据列中的当前数据更改当前区域的列宽，以达到最佳宽度。</span><span class="sxs-lookup"><span data-stu-id="94061-124">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="94061-125">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="94061-125">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="94061-126">无</span><span class="sxs-lookup"><span data-stu-id="94061-126">None</span></span>|<span data-ttu-id="94061-127">根据列中的当前数据更改当前区域的行高，以达到最佳高度。</span><span class="sxs-lookup"><span data-stu-id="94061-127">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="94061-128">属性</span><span class="sxs-lookup"><span data-stu-id="94061-128">Properties</span></span>
| <span data-ttu-id="94061-129">属性</span><span class="sxs-lookup"><span data-stu-id="94061-129">Property</span></span>     | <span data-ttu-id="94061-130">类型</span><span class="sxs-lookup"><span data-stu-id="94061-130">Type</span></span>   |<span data-ttu-id="94061-131">说明</span><span class="sxs-lookup"><span data-stu-id="94061-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94061-132">columnWidth</span><span class="sxs-lookup"><span data-stu-id="94061-132">columnWidth</span></span>|<span data-ttu-id="94061-133">double</span><span class="sxs-lookup"><span data-stu-id="94061-133">double</span></span>|<span data-ttu-id="94061-p101">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="94061-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="94061-136">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="94061-136">horizontalAlignment</span></span>|<span data-ttu-id="94061-137">string</span><span class="sxs-lookup"><span data-stu-id="94061-137">string</span></span>|<span data-ttu-id="94061-138">表示指定对象的水平对齐方式。</span><span class="sxs-lookup"><span data-stu-id="94061-138">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="94061-139">可能的值为： `General`、 `Left`、 `Center` `Right` `Fill` `Justify` `CenterAcrossSelection`、、、、 `Distributed`。</span><span class="sxs-lookup"><span data-stu-id="94061-139">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="94061-140">rowHeight</span><span class="sxs-lookup"><span data-stu-id="94061-140">rowHeight</span></span>|<span data-ttu-id="94061-141">double</span><span class="sxs-lookup"><span data-stu-id="94061-141">double</span></span>|<span data-ttu-id="94061-p103">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="94061-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="94061-144">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="94061-144">verticalAlignment</span></span>|<span data-ttu-id="94061-145">string</span><span class="sxs-lookup"><span data-stu-id="94061-145">string</span></span>|<span data-ttu-id="94061-146">表示指定对象的垂直对齐方式。</span><span class="sxs-lookup"><span data-stu-id="94061-146">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="94061-147">可能的值包括 `Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="94061-147">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="94061-148">wrapText</span><span class="sxs-lookup"><span data-stu-id="94061-148">wrapText</span></span>|<span data-ttu-id="94061-149">boolean</span><span class="sxs-lookup"><span data-stu-id="94061-149">boolean</span></span>|<span data-ttu-id="94061-p105">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="94061-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="94061-152">关系</span><span class="sxs-lookup"><span data-stu-id="94061-152">Relationships</span></span>
| <span data-ttu-id="94061-153">关系</span><span class="sxs-lookup"><span data-stu-id="94061-153">Relationship</span></span> | <span data-ttu-id="94061-154">类型</span><span class="sxs-lookup"><span data-stu-id="94061-154">Type</span></span>   |<span data-ttu-id="94061-155">说明</span><span class="sxs-lookup"><span data-stu-id="94061-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94061-156">borders</span><span class="sxs-lookup"><span data-stu-id="94061-156">borders</span></span>|<span data-ttu-id="94061-157">[WorkbookRangeBorder](rangeborder.md)集合</span><span class="sxs-lookup"><span data-stu-id="94061-157">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="94061-158">应用于所选的整个区域的 border 对象的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="94061-158">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="94061-159">fill</span><span class="sxs-lookup"><span data-stu-id="94061-159">fill</span></span>|[<span data-ttu-id="94061-160">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="94061-160">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="94061-p106">返回在整个区域内定义的 fill 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="94061-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="94061-163">font</span><span class="sxs-lookup"><span data-stu-id="94061-163">font</span></span>|[<span data-ttu-id="94061-164">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="94061-164">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="94061-165">返回在所选的整个区域内定义的 font 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="94061-165">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="94061-166">protection</span><span class="sxs-lookup"><span data-stu-id="94061-166">protection</span></span>|[<span data-ttu-id="94061-167">WorkbookFormatProtection</span><span class="sxs-lookup"><span data-stu-id="94061-167">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="94061-168">返回某一区域的格式 protection 对象。</span><span class="sxs-lookup"><span data-stu-id="94061-168">Returns the format protection object for a range.</span></span> <span data-ttu-id="94061-169">只读。</span><span class="sxs-lookup"><span data-stu-id="94061-169">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94061-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94061-170">JSON representation</span></span>

<span data-ttu-id="94061-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94061-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
