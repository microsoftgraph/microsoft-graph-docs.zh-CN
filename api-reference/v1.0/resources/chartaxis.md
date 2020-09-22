---
title: ChartAxis 资源类型
description: 代表图表中的单个坐标轴。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 76bbc5f2696f966be017b798ceb065afccf3b61e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991948"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="4d564-103">ChartAxis 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d564-103">ChartAxis resource type</span></span>

<span data-ttu-id="4d564-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d564-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4d564-105">代表图表中的单个坐标轴。</span><span class="sxs-lookup"><span data-stu-id="4d564-105">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="4d564-106">方法</span><span class="sxs-lookup"><span data-stu-id="4d564-106">Methods</span></span>

| <span data-ttu-id="4d564-107">方法</span><span class="sxs-lookup"><span data-stu-id="4d564-107">Method</span></span>           | <span data-ttu-id="4d564-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4d564-108">Return Type</span></span>    |<span data-ttu-id="4d564-109">说明</span><span class="sxs-lookup"><span data-stu-id="4d564-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4d564-110">获取 ChartAxis</span><span class="sxs-lookup"><span data-stu-id="4d564-110">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="4d564-111">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="4d564-111">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="4d564-112">读取 chartaxis 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4d564-112">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="4d564-113">更新</span><span class="sxs-lookup"><span data-stu-id="4d564-113">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="4d564-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="4d564-114">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="4d564-115">更新 ChartAxis 对象</span><span class="sxs-lookup"><span data-stu-id="4d564-115">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4d564-116">属性</span><span class="sxs-lookup"><span data-stu-id="4d564-116">Properties</span></span>
| <span data-ttu-id="4d564-117">属性</span><span class="sxs-lookup"><span data-stu-id="4d564-117">Property</span></span>     | <span data-ttu-id="4d564-118">类型</span><span class="sxs-lookup"><span data-stu-id="4d564-118">Type</span></span>   |<span data-ttu-id="4d564-119">说明</span><span class="sxs-lookup"><span data-stu-id="4d564-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d564-120">id</span><span class="sxs-lookup"><span data-stu-id="4d564-120">id</span></span>       |<span data-ttu-id="4d564-121">string</span><span class="sxs-lookup"><span data-stu-id="4d564-121">string</span></span>   | <span data-ttu-id="4d564-122">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4d564-122">Unique identifier.</span></span> <span data-ttu-id="4d564-123">只读。</span><span class="sxs-lookup"><span data-stu-id="4d564-123">Read-only.</span></span>|
|<span data-ttu-id="4d564-124">majorUnit</span><span class="sxs-lookup"><span data-stu-id="4d564-124">majorUnit</span></span>|<span data-ttu-id="4d564-125">Json</span><span class="sxs-lookup"><span data-stu-id="4d564-125">Json</span></span>|<span data-ttu-id="4d564-p102">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="4d564-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="4d564-129">maximum</span><span class="sxs-lookup"><span data-stu-id="4d564-129">maximum</span></span>|<span data-ttu-id="4d564-130">Json</span><span class="sxs-lookup"><span data-stu-id="4d564-130">Json</span></span>|<span data-ttu-id="4d564-p103">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="4d564-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="4d564-134">minimum</span><span class="sxs-lookup"><span data-stu-id="4d564-134">minimum</span></span>|<span data-ttu-id="4d564-135">Json</span><span class="sxs-lookup"><span data-stu-id="4d564-135">Json</span></span>|<span data-ttu-id="4d564-p104">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="4d564-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="4d564-139">minorUnit</span><span class="sxs-lookup"><span data-stu-id="4d564-139">minorUnit</span></span>|<span data-ttu-id="4d564-140">Json</span><span class="sxs-lookup"><span data-stu-id="4d564-140">Json</span></span>|<span data-ttu-id="4d564-p105">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="4d564-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d564-144">关系</span><span class="sxs-lookup"><span data-stu-id="4d564-144">Relationships</span></span>
| <span data-ttu-id="4d564-145">关系</span><span class="sxs-lookup"><span data-stu-id="4d564-145">Relationship</span></span> | <span data-ttu-id="4d564-146">类型</span><span class="sxs-lookup"><span data-stu-id="4d564-146">Type</span></span>   |<span data-ttu-id="4d564-147">说明</span><span class="sxs-lookup"><span data-stu-id="4d564-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d564-148">format</span><span class="sxs-lookup"><span data-stu-id="4d564-148">format</span></span>|[<span data-ttu-id="4d564-149">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="4d564-149">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="4d564-p106">表示 chart 对象的格式，包括线条和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="4d564-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="4d564-152">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="4d564-152">majorGridlines</span></span>|[<span data-ttu-id="4d564-153">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="4d564-153">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="4d564-p107">返回一个表示指定坐标轴的主要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="4d564-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="4d564-156">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="4d564-156">minorGridlines</span></span>|[<span data-ttu-id="4d564-157">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="4d564-157">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="4d564-p108">返回一个表示指定坐标轴的次要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="4d564-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="4d564-160">title</span><span class="sxs-lookup"><span data-stu-id="4d564-160">title</span></span>|[<span data-ttu-id="4d564-161">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="4d564-161">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="4d564-162">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="4d564-162">Represents the axis title.</span></span> <span data-ttu-id="4d564-163">只读。</span><span class="sxs-lookup"><span data-stu-id="4d564-163">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d564-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d564-164">JSON representation</span></span>

<span data-ttu-id="4d564-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d564-165">Here is a JSON representation of the resource.</span></span>

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

