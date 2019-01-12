---
title: RangeFormat 资源类型
description: 一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b4018995e37ff40ae014b54d08b77bbed73d6fe2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937346"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="8d34b-103">RangeFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d34b-103">RangeFormat resource type</span></span>

> <span data-ttu-id="8d34b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8d34b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d34b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d34b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d34b-106">一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。</span><span class="sxs-lookup"><span data-stu-id="8d34b-106">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="8d34b-107">方法</span><span class="sxs-lookup"><span data-stu-id="8d34b-107">Methods</span></span>

| <span data-ttu-id="8d34b-108">方法</span><span class="sxs-lookup"><span data-stu-id="8d34b-108">Method</span></span>           | <span data-ttu-id="8d34b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d34b-109">Return Type</span></span>    |<span data-ttu-id="8d34b-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d34b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d34b-111">获取 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="8d34b-111">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="8d34b-112">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="8d34b-112">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="8d34b-113">读取 rangeFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d34b-113">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="8d34b-114">创建 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="8d34b-114">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="8d34b-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="8d34b-115">RangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="8d34b-116">通过发布到边框集合创建新的 RangeBorder。</span><span class="sxs-lookup"><span data-stu-id="8d34b-116">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="8d34b-117">列出边框</span><span class="sxs-lookup"><span data-stu-id="8d34b-117">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="8d34b-118">[RangeBorder](rangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d34b-118">[RangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="8d34b-119">获取 RangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d34b-119">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="8d34b-120">更新</span><span class="sxs-lookup"><span data-stu-id="8d34b-120">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="8d34b-121">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="8d34b-121">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="8d34b-122">更新 RangeFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="8d34b-122">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="8d34b-123">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="8d34b-123">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="8d34b-124">无</span><span class="sxs-lookup"><span data-stu-id="8d34b-124">None</span></span>|<span data-ttu-id="8d34b-125">根据列中的当前数据更改当前区域的列宽，以达到最佳宽度。</span><span class="sxs-lookup"><span data-stu-id="8d34b-125">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="8d34b-126">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="8d34b-126">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="8d34b-127">无</span><span class="sxs-lookup"><span data-stu-id="8d34b-127">None</span></span>|<span data-ttu-id="8d34b-128">根据列中的当前数据更改当前区域的行高，以达到最佳高度。</span><span class="sxs-lookup"><span data-stu-id="8d34b-128">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d34b-129">属性</span><span class="sxs-lookup"><span data-stu-id="8d34b-129">Properties</span></span>
| <span data-ttu-id="8d34b-130">属性</span><span class="sxs-lookup"><span data-stu-id="8d34b-130">Property</span></span>     | <span data-ttu-id="8d34b-131">类型</span><span class="sxs-lookup"><span data-stu-id="8d34b-131">Type</span></span>   |<span data-ttu-id="8d34b-132">说明</span><span class="sxs-lookup"><span data-stu-id="8d34b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d34b-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="8d34b-133">columnWidth</span></span>|<span data-ttu-id="8d34b-134">double</span><span class="sxs-lookup"><span data-stu-id="8d34b-134">double</span></span>|<span data-ttu-id="8d34b-p102">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="8d34b-p102">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="8d34b-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="8d34b-137">horizontalAlignment</span></span>|<span data-ttu-id="8d34b-138">string</span><span class="sxs-lookup"><span data-stu-id="8d34b-138">string</span></span>|<span data-ttu-id="8d34b-p103">表示指定对象的水平对齐方式。可能的值是：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="8d34b-p103">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="8d34b-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="8d34b-141">rowHeight</span></span>|<span data-ttu-id="8d34b-142">double</span><span class="sxs-lookup"><span data-stu-id="8d34b-142">double</span></span>|<span data-ttu-id="8d34b-p104">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="8d34b-p104">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="8d34b-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="8d34b-145">verticalAlignment</span></span>|<span data-ttu-id="8d34b-146">string</span><span class="sxs-lookup"><span data-stu-id="8d34b-146">string</span></span>|<span data-ttu-id="8d34b-p105">表示指定对象的垂直对齐方式。可能的值是：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="8d34b-p105">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="8d34b-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="8d34b-149">wrapText</span></span>|<span data-ttu-id="8d34b-150">boolean</span><span class="sxs-lookup"><span data-stu-id="8d34b-150">boolean</span></span>|<span data-ttu-id="8d34b-p106">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="8d34b-p106">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d34b-153">Relationships</span><span class="sxs-lookup"><span data-stu-id="8d34b-153">Relationships</span></span>
| <span data-ttu-id="8d34b-154">关系</span><span class="sxs-lookup"><span data-stu-id="8d34b-154">Relationship</span></span> | <span data-ttu-id="8d34b-155">类型</span><span class="sxs-lookup"><span data-stu-id="8d34b-155">Type</span></span>   |<span data-ttu-id="8d34b-156">说明</span><span class="sxs-lookup"><span data-stu-id="8d34b-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d34b-157">边框</span><span class="sxs-lookup"><span data-stu-id="8d34b-157">borders</span></span>|<span data-ttu-id="8d34b-158">[RangeBorder](rangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8d34b-158">[RangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="8d34b-159">应用于所选的整个区域的 border 对象的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="8d34b-159">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="8d34b-160">fill</span><span class="sxs-lookup"><span data-stu-id="8d34b-160">fill</span></span>|[<span data-ttu-id="8d34b-161">RangeFill</span><span class="sxs-lookup"><span data-stu-id="8d34b-161">RangeFill</span></span>](rangefill.md)|<span data-ttu-id="8d34b-p107">返回在整个区域内定义的 fill 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="8d34b-p107">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="8d34b-164">font</span><span class="sxs-lookup"><span data-stu-id="8d34b-164">font</span></span>|[<span data-ttu-id="8d34b-165">RangeFont</span><span class="sxs-lookup"><span data-stu-id="8d34b-165">RangeFont</span></span>](rangefont.md)|<span data-ttu-id="8d34b-166">返回在所选的整个区域内定义的 font 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="8d34b-166">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="8d34b-167">protection</span><span class="sxs-lookup"><span data-stu-id="8d34b-167">protection</span></span>|[<span data-ttu-id="8d34b-168">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="8d34b-168">FormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="8d34b-p108">返回某一区域的格式 protection 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="8d34b-p108">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d34b-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d34b-171">JSON representation</span></span>

<span data-ttu-id="8d34b-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d34b-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFormat"
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
