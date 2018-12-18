---
title: ChartAxis 资源类型
description: 表示图表中的单个坐标轴。
author: lumine2008
ms.openlocfilehash: 39c71e9fa832ffb967a1ef147ccd7e07d6b9aaec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344364"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="6272c-103">ChartAxis 资源类型</span><span class="sxs-lookup"><span data-stu-id="6272c-103">ChartAxis resource type</span></span>

<span data-ttu-id="6272c-104">表示图表中的单个坐标轴。</span><span class="sxs-lookup"><span data-stu-id="6272c-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="6272c-105">方法</span><span class="sxs-lookup"><span data-stu-id="6272c-105">Methods</span></span>

| <span data-ttu-id="6272c-106">方法</span><span class="sxs-lookup"><span data-stu-id="6272c-106">Method</span></span>           | <span data-ttu-id="6272c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6272c-107">Return Type</span></span>    |<span data-ttu-id="6272c-108">说明</span><span class="sxs-lookup"><span data-stu-id="6272c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6272c-109">获取 ChartAxis</span><span class="sxs-lookup"><span data-stu-id="6272c-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="6272c-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="6272c-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="6272c-111">读取 chartaxis 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6272c-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="6272c-112">Update</span><span class="sxs-lookup"><span data-stu-id="6272c-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="6272c-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="6272c-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="6272c-114">更新 ChartAxis 对象</span><span class="sxs-lookup"><span data-stu-id="6272c-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6272c-115">属性</span><span class="sxs-lookup"><span data-stu-id="6272c-115">Properties</span></span>
| <span data-ttu-id="6272c-116">属性</span><span class="sxs-lookup"><span data-stu-id="6272c-116">Property</span></span>     | <span data-ttu-id="6272c-117">类型</span><span class="sxs-lookup"><span data-stu-id="6272c-117">Type</span></span>   |<span data-ttu-id="6272c-118">说明</span><span class="sxs-lookup"><span data-stu-id="6272c-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6272c-119">ID</span><span class="sxs-lookup"><span data-stu-id="6272c-119">id</span></span>       |<span data-ttu-id="6272c-120">string</span><span class="sxs-lookup"><span data-stu-id="6272c-120">string</span></span>   | <span data-ttu-id="6272c-121">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6272c-121">Unique identifier.</span></span> <span data-ttu-id="6272c-122">只读。</span><span class="sxs-lookup"><span data-stu-id="6272c-122">Read-only.</span></span>|
|<span data-ttu-id="6272c-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="6272c-123">majorUnit</span></span>|<span data-ttu-id="6272c-124">Json</span><span class="sxs-lookup"><span data-stu-id="6272c-124">Json</span></span>|<span data-ttu-id="6272c-p102">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="6272c-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="6272c-128">maximum</span><span class="sxs-lookup"><span data-stu-id="6272c-128">maximum</span></span>|<span data-ttu-id="6272c-129">Json</span><span class="sxs-lookup"><span data-stu-id="6272c-129">Json</span></span>|<span data-ttu-id="6272c-p103">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="6272c-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="6272c-133">minimum</span><span class="sxs-lookup"><span data-stu-id="6272c-133">minimum</span></span>|<span data-ttu-id="6272c-134">Json</span><span class="sxs-lookup"><span data-stu-id="6272c-134">Json</span></span>|<span data-ttu-id="6272c-p104">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="6272c-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="6272c-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="6272c-138">minorUnit</span></span>|<span data-ttu-id="6272c-139">Json</span><span class="sxs-lookup"><span data-stu-id="6272c-139">Json</span></span>|<span data-ttu-id="6272c-p105">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="6272c-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6272c-143">Relationships</span><span class="sxs-lookup"><span data-stu-id="6272c-143">Relationships</span></span>
| <span data-ttu-id="6272c-144">关系</span><span class="sxs-lookup"><span data-stu-id="6272c-144">Relationship</span></span> | <span data-ttu-id="6272c-145">类型</span><span class="sxs-lookup"><span data-stu-id="6272c-145">Type</span></span>   |<span data-ttu-id="6272c-146">说明</span><span class="sxs-lookup"><span data-stu-id="6272c-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6272c-147">format</span><span class="sxs-lookup"><span data-stu-id="6272c-147">format</span></span>|[<span data-ttu-id="6272c-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="6272c-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="6272c-p106">表示 chart 对象的格式，包括线条和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="6272c-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="6272c-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="6272c-151">majorGridlines</span></span>|[<span data-ttu-id="6272c-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="6272c-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="6272c-p107">返回一个表示指定坐标轴的主要网格线的 gridline 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="6272c-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="6272c-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="6272c-155">minorGridlines</span></span>|[<span data-ttu-id="6272c-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="6272c-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="6272c-p108">返回一个表示指定坐标轴的次要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="6272c-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="6272c-159">title</span><span class="sxs-lookup"><span data-stu-id="6272c-159">title</span></span>|[<span data-ttu-id="6272c-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="6272c-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="6272c-p109">表示坐标轴标题。只读。</span><span class="sxs-lookup"><span data-stu-id="6272c-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6272c-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6272c-163">JSON representation</span></span>

<span data-ttu-id="6272c-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6272c-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->