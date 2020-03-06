---
title: ChartAxis 资源类型
description: 代表图表中的单个坐标轴。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0ae528e68aa3bf28457f2fee04beb6a8013e902d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531897"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="9a487-103">ChartAxis 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a487-103">ChartAxis resource type</span></span>

<span data-ttu-id="9a487-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a487-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a487-105">代表图表中的单个坐标轴。</span><span class="sxs-lookup"><span data-stu-id="9a487-105">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="9a487-106">Methods</span><span class="sxs-lookup"><span data-stu-id="9a487-106">Methods</span></span>

| <span data-ttu-id="9a487-107">方法</span><span class="sxs-lookup"><span data-stu-id="9a487-107">Method</span></span>           | <span data-ttu-id="9a487-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a487-108">Return Type</span></span>    |<span data-ttu-id="9a487-109">说明</span><span class="sxs-lookup"><span data-stu-id="9a487-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a487-110">获取 ChartAxis</span><span class="sxs-lookup"><span data-stu-id="9a487-110">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="9a487-111">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="9a487-111">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="9a487-112">读取 chartaxis 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9a487-112">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="9a487-113">更新</span><span class="sxs-lookup"><span data-stu-id="9a487-113">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="9a487-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="9a487-114">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="9a487-115">更新 ChartAxis 对象</span><span class="sxs-lookup"><span data-stu-id="9a487-115">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a487-116">属性</span><span class="sxs-lookup"><span data-stu-id="9a487-116">Properties</span></span>
| <span data-ttu-id="9a487-117">属性</span><span class="sxs-lookup"><span data-stu-id="9a487-117">Property</span></span>     | <span data-ttu-id="9a487-118">类型</span><span class="sxs-lookup"><span data-stu-id="9a487-118">Type</span></span>   |<span data-ttu-id="9a487-119">说明</span><span class="sxs-lookup"><span data-stu-id="9a487-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a487-120">id</span><span class="sxs-lookup"><span data-stu-id="9a487-120">id</span></span>       |<span data-ttu-id="9a487-121">string</span><span class="sxs-lookup"><span data-stu-id="9a487-121">string</span></span>   | <span data-ttu-id="9a487-122">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9a487-122">Unique identifier.</span></span> <span data-ttu-id="9a487-123">只读。</span><span class="sxs-lookup"><span data-stu-id="9a487-123">Read-only.</span></span>|
|<span data-ttu-id="9a487-124">majorUnit</span><span class="sxs-lookup"><span data-stu-id="9a487-124">majorUnit</span></span>|<span data-ttu-id="9a487-125">Json</span><span class="sxs-lookup"><span data-stu-id="9a487-125">Json</span></span>|<span data-ttu-id="9a487-p102">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="9a487-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="9a487-129">maximum</span><span class="sxs-lookup"><span data-stu-id="9a487-129">maximum</span></span>|<span data-ttu-id="9a487-130">Json</span><span class="sxs-lookup"><span data-stu-id="9a487-130">Json</span></span>|<span data-ttu-id="9a487-p103">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="9a487-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="9a487-134">minimum</span><span class="sxs-lookup"><span data-stu-id="9a487-134">minimum</span></span>|<span data-ttu-id="9a487-135">Json</span><span class="sxs-lookup"><span data-stu-id="9a487-135">Json</span></span>|<span data-ttu-id="9a487-p104">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="9a487-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="9a487-139">minorUnit</span><span class="sxs-lookup"><span data-stu-id="9a487-139">minorUnit</span></span>|<span data-ttu-id="9a487-140">Json</span><span class="sxs-lookup"><span data-stu-id="9a487-140">Json</span></span>|<span data-ttu-id="9a487-p105">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="9a487-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a487-144">关系</span><span class="sxs-lookup"><span data-stu-id="9a487-144">Relationships</span></span>
| <span data-ttu-id="9a487-145">关系</span><span class="sxs-lookup"><span data-stu-id="9a487-145">Relationship</span></span> | <span data-ttu-id="9a487-146">类型</span><span class="sxs-lookup"><span data-stu-id="9a487-146">Type</span></span>   |<span data-ttu-id="9a487-147">说明</span><span class="sxs-lookup"><span data-stu-id="9a487-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a487-148">format</span><span class="sxs-lookup"><span data-stu-id="9a487-148">format</span></span>|[<span data-ttu-id="9a487-149">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="9a487-149">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="9a487-p106">表示 chart 对象的格式，包括线条和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="9a487-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="9a487-152">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="9a487-152">majorGridlines</span></span>|[<span data-ttu-id="9a487-153">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9a487-153">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="9a487-p107">返回一个表示指定坐标轴的主要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="9a487-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="9a487-156">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="9a487-156">minorGridlines</span></span>|[<span data-ttu-id="9a487-157">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9a487-157">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="9a487-p108">返回一个表示指定坐标轴的次要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="9a487-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="9a487-160">title</span><span class="sxs-lookup"><span data-stu-id="9a487-160">title</span></span>|[<span data-ttu-id="9a487-161">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="9a487-161">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="9a487-162">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="9a487-162">Represents the axis title.</span></span> <span data-ttu-id="9a487-163">只读。</span><span class="sxs-lookup"><span data-stu-id="9a487-163">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a487-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a487-164">JSON representation</span></span>

<span data-ttu-id="9a487-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a487-165">Here is a JSON representation of the resource.</span></span>

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
