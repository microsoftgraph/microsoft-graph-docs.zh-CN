---
title: RangeFormat 资源类型
description: 一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。
ms.openlocfilehash: 8451b1f24f7c0df3842ed390a2a182746a0a7b20
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008692"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="d9b2b-103">RangeFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9b2b-103">RangeFormat resource type</span></span>

<span data-ttu-id="d9b2b-104">一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d9b2b-105">方法</span><span class="sxs-lookup"><span data-stu-id="d9b2b-105">Methods</span></span>

| <span data-ttu-id="d9b2b-106">方法</span><span class="sxs-lookup"><span data-stu-id="d9b2b-106">Method</span></span>           | <span data-ttu-id="d9b2b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9b2b-107">Return Type</span></span>    |<span data-ttu-id="d9b2b-108">说明</span><span class="sxs-lookup"><span data-stu-id="d9b2b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9b2b-109">获取 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="d9b2b-109">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="d9b2b-110">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="d9b2b-110">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="d9b2b-111">读取 rangeFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="d9b2b-112">创建 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d9b2b-112">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="d9b2b-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="d9b2b-113">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="d9b2b-114">通过发布到边框集合创建新的 RangeBorder。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="d9b2b-115">列出边框</span><span class="sxs-lookup"><span data-stu-id="d9b2b-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="d9b2b-116">[WorkbookRangeBorder](rangeborder.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9b2b-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="d9b2b-117">获取 RangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="d9b2b-118">Update</span><span class="sxs-lookup"><span data-stu-id="d9b2b-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="d9b2b-119">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="d9b2b-119">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="d9b2b-120">更新 RangeFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="d9b2b-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="d9b2b-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="d9b2b-122">无</span><span class="sxs-lookup"><span data-stu-id="d9b2b-122">None</span></span>|<span data-ttu-id="d9b2b-123">根据列中的当前数据更改当前区域的列宽，以达到最佳宽度。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="d9b2b-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="d9b2b-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="d9b2b-125">无</span><span class="sxs-lookup"><span data-stu-id="d9b2b-125">None</span></span>|<span data-ttu-id="d9b2b-126">根据列中的当前数据更改当前区域的行高，以达到最佳高度。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9b2b-127">属性</span><span class="sxs-lookup"><span data-stu-id="d9b2b-127">Properties</span></span>
| <span data-ttu-id="d9b2b-128">属性</span><span class="sxs-lookup"><span data-stu-id="d9b2b-128">Property</span></span>     | <span data-ttu-id="d9b2b-129">类型</span><span class="sxs-lookup"><span data-stu-id="d9b2b-129">Type</span></span>   |<span data-ttu-id="d9b2b-130">说明</span><span class="sxs-lookup"><span data-stu-id="d9b2b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9b2b-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="d9b2b-131">columnWidth</span></span>|<span data-ttu-id="d9b2b-132">double</span><span class="sxs-lookup"><span data-stu-id="d9b2b-132">double</span></span>|<span data-ttu-id="d9b2b-p101">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="d9b2b-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="d9b2b-135">horizontalAlignment</span></span>|<span data-ttu-id="d9b2b-136">string</span><span class="sxs-lookup"><span data-stu-id="d9b2b-136">string</span></span>|<span data-ttu-id="d9b2b-137">代表指定对象的水平对齐方式。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-137">Represents the horizontal alignment for the specified object.</span></span> <span data-ttu-id="d9b2b-138">可能的值为： `General`， `Left`， `Center`， `Right`， `Fill`， `Justify`， `CenterAcrossSelection`， `Distributed`。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-138">The possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="d9b2b-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="d9b2b-139">rowHeight</span></span>|<span data-ttu-id="d9b2b-140">double</span><span class="sxs-lookup"><span data-stu-id="d9b2b-140">double</span></span>|<span data-ttu-id="d9b2b-p103">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="d9b2b-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="d9b2b-143">verticalAlignment</span></span>|<span data-ttu-id="d9b2b-144">string</span><span class="sxs-lookup"><span data-stu-id="d9b2b-144">string</span></span>|<span data-ttu-id="d9b2b-145">代表指定对象的垂直对齐方式。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-145">Represents the vertical alignment for the specified object.</span></span> <span data-ttu-id="d9b2b-146">可能的值为： `Top`， `Center`， `Bottom`， `Justify`， `Distributed`。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-146">The possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="d9b2b-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="d9b2b-147">wrapText</span></span>|<span data-ttu-id="d9b2b-148">boolean</span><span class="sxs-lookup"><span data-stu-id="d9b2b-148">boolean</span></span>|<span data-ttu-id="d9b2b-p105">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="d9b2b-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9b2b-151">Relationships</span><span class="sxs-lookup"><span data-stu-id="d9b2b-151">Relationships</span></span>
| <span data-ttu-id="d9b2b-152">关系</span><span class="sxs-lookup"><span data-stu-id="d9b2b-152">Relationship</span></span> | <span data-ttu-id="d9b2b-153">类型</span><span class="sxs-lookup"><span data-stu-id="d9b2b-153">Type</span></span>   |<span data-ttu-id="d9b2b-154">说明</span><span class="sxs-lookup"><span data-stu-id="d9b2b-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9b2b-155">边框</span><span class="sxs-lookup"><span data-stu-id="d9b2b-155">borders</span></span>|<span data-ttu-id="d9b2b-156">[WorkbookRangeBorder](rangeborder.md)集合</span><span class="sxs-lookup"><span data-stu-id="d9b2b-156">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="d9b2b-157">应用于所选的整个区域的 border 对象的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="d9b2b-158">fill</span><span class="sxs-lookup"><span data-stu-id="d9b2b-158">fill</span></span>|[<span data-ttu-id="d9b2b-159">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="d9b2b-159">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="d9b2b-p106">返回在整个区域内定义的 fill 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="d9b2b-162">font</span><span class="sxs-lookup"><span data-stu-id="d9b2b-162">font</span></span>|[<span data-ttu-id="d9b2b-163">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="d9b2b-163">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="d9b2b-164">返回在所选的整个区域内定义的 font 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="d9b2b-165">protection</span><span class="sxs-lookup"><span data-stu-id="d9b2b-165">protection</span></span>|[<span data-ttu-id="d9b2b-166">WorkbookFormatProtection</span><span class="sxs-lookup"><span data-stu-id="d9b2b-166">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="d9b2b-p107">返回某一区域的格式保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9b2b-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9b2b-169">JSON representation</span></span>

<span data-ttu-id="d9b2b-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9b2b-170">Here is a JSON representation of the resource.</span></span>

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