---
title: workbookRangeFormat 资源类型
description: 一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 3ee55e1a398dab1727dfdc24d9ebd5c66b7440d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348628"
---
# <a name="workbookrangeformat-resource-type"></a><span data-ttu-id="b1894-103">workbookRangeFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1894-103">workbookRangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1894-104">一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。</span><span class="sxs-lookup"><span data-stu-id="b1894-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="b1894-105">方法</span><span class="sxs-lookup"><span data-stu-id="b1894-105">Methods</span></span>

| <span data-ttu-id="b1894-106">方法</span><span class="sxs-lookup"><span data-stu-id="b1894-106">Method</span></span>           | <span data-ttu-id="b1894-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1894-107">Return Type</span></span>    |<span data-ttu-id="b1894-108">说明</span><span class="sxs-lookup"><span data-stu-id="b1894-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1894-109">获取 workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="b1894-109">Get workbookRangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="b1894-110">workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="b1894-110">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="b1894-111">读取 rangeFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b1894-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="b1894-112">创建 workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="b1894-112">Create workbookRangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="b1894-113">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="b1894-113">workbookRangeBorder</span></span>](workbookrangeborder.md)| <span data-ttu-id="b1894-114">通过发布到边框集合创建新的 RangeBorder。</span><span class="sxs-lookup"><span data-stu-id="b1894-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="b1894-115">列出边框</span><span class="sxs-lookup"><span data-stu-id="b1894-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="b1894-116">[workbookRangeBorder](workbookrangeborder.md)集合</span><span class="sxs-lookup"><span data-stu-id="b1894-116">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>| <span data-ttu-id="b1894-117">获取 RangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b1894-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="b1894-118">更新</span><span class="sxs-lookup"><span data-stu-id="b1894-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="b1894-119">workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="b1894-119">workbookRangeFormat</span></span>](workbookrangeformat.md) |<span data-ttu-id="b1894-120">更新 RangeFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="b1894-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="b1894-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="b1894-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="b1894-122">无</span><span class="sxs-lookup"><span data-stu-id="b1894-122">None</span></span>|<span data-ttu-id="b1894-123">根据列中的当前数据更改当前区域的列宽，以达到最佳宽度。</span><span class="sxs-lookup"><span data-stu-id="b1894-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="b1894-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="b1894-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="b1894-125">无</span><span class="sxs-lookup"><span data-stu-id="b1894-125">None</span></span>|<span data-ttu-id="b1894-126">根据列中的当前数据更改当前区域的行高，以达到最佳高度。</span><span class="sxs-lookup"><span data-stu-id="b1894-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1894-127">属性</span><span class="sxs-lookup"><span data-stu-id="b1894-127">Properties</span></span>
| <span data-ttu-id="b1894-128">属性</span><span class="sxs-lookup"><span data-stu-id="b1894-128">Property</span></span>     | <span data-ttu-id="b1894-129">类型</span><span class="sxs-lookup"><span data-stu-id="b1894-129">Type</span></span>   |<span data-ttu-id="b1894-130">说明</span><span class="sxs-lookup"><span data-stu-id="b1894-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1894-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="b1894-131">columnWidth</span></span>|<span data-ttu-id="b1894-132">double</span><span class="sxs-lookup"><span data-stu-id="b1894-132">double</span></span>|<span data-ttu-id="b1894-p101">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="b1894-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="b1894-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="b1894-135">horizontalAlignment</span></span>|<span data-ttu-id="b1894-136">string</span><span class="sxs-lookup"><span data-stu-id="b1894-136">string</span></span>|<span data-ttu-id="b1894-p102">表示指定对象的水平对齐方式。可能的值是：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="b1894-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="b1894-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="b1894-139">rowHeight</span></span>|<span data-ttu-id="b1894-140">double</span><span class="sxs-lookup"><span data-stu-id="b1894-140">double</span></span>|<span data-ttu-id="b1894-p103">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="b1894-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="b1894-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="b1894-143">verticalAlignment</span></span>|<span data-ttu-id="b1894-144">string</span><span class="sxs-lookup"><span data-stu-id="b1894-144">string</span></span>|<span data-ttu-id="b1894-p104">表示指定对象的垂直对齐方式。可能的值是：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="b1894-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="b1894-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="b1894-147">wrapText</span></span>|<span data-ttu-id="b1894-148">boolean</span><span class="sxs-lookup"><span data-stu-id="b1894-148">boolean</span></span>|<span data-ttu-id="b1894-p105">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="b1894-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1894-151">关系</span><span class="sxs-lookup"><span data-stu-id="b1894-151">Relationships</span></span>
| <span data-ttu-id="b1894-152">关系</span><span class="sxs-lookup"><span data-stu-id="b1894-152">Relationship</span></span> | <span data-ttu-id="b1894-153">类型</span><span class="sxs-lookup"><span data-stu-id="b1894-153">Type</span></span>   |<span data-ttu-id="b1894-154">说明</span><span class="sxs-lookup"><span data-stu-id="b1894-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1894-155">borders</span><span class="sxs-lookup"><span data-stu-id="b1894-155">borders</span></span>|<span data-ttu-id="b1894-156">[workbookRangeBorder](workbookrangeborder.md)集合</span><span class="sxs-lookup"><span data-stu-id="b1894-156">[workbookRangeBorder](workbookrangeborder.md) collection</span></span>|<span data-ttu-id="b1894-157">应用于所选的整个区域的 border 对象的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="b1894-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="b1894-158">fill</span><span class="sxs-lookup"><span data-stu-id="b1894-158">fill</span></span>|[<span data-ttu-id="b1894-159">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="b1894-159">workbookRangeFill</span></span>](workbookrangefill.md)|<span data-ttu-id="b1894-p106">返回在整个区域内定义的 fill 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="b1894-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="b1894-162">font</span><span class="sxs-lookup"><span data-stu-id="b1894-162">font</span></span>|[<span data-ttu-id="b1894-163">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="b1894-163">workbookRangeFont</span></span>](workbookrangefont.md)|<span data-ttu-id="b1894-164">返回在所选的整个区域内定义的 font 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="b1894-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="b1894-165">protection</span><span class="sxs-lookup"><span data-stu-id="b1894-165">protection</span></span>|[<span data-ttu-id="b1894-166">formatProtection</span><span class="sxs-lookup"><span data-stu-id="b1894-166">formatProtection</span></span>](formatprotection.md)|<span data-ttu-id="b1894-167">返回某一区域的格式 protection 对象。</span><span class="sxs-lookup"><span data-stu-id="b1894-167">Returns the format protection object for a range.</span></span> <span data-ttu-id="b1894-168">只读。</span><span class="sxs-lookup"><span data-stu-id="b1894-168">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1894-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1894-169">JSON representation</span></span>

<span data-ttu-id="b1894-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1894-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
