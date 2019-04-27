---
title: workbookChartAxis 资源类型
description: 代表图表中的单个坐标轴。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ce18f029e3e5e48597ac5074d683e6a8cdb64674
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348561"
---
# <a name="workbookchartaxis-resource-type"></a><span data-ttu-id="84404-103">workbookChartAxis 资源类型</span><span class="sxs-lookup"><span data-stu-id="84404-103">workbookChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84404-104">代表图表中的单个坐标轴。</span><span class="sxs-lookup"><span data-stu-id="84404-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="84404-105">方法</span><span class="sxs-lookup"><span data-stu-id="84404-105">Methods</span></span>

| <span data-ttu-id="84404-106">方法</span><span class="sxs-lookup"><span data-stu-id="84404-106">Method</span></span>           | <span data-ttu-id="84404-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="84404-107">Return Type</span></span>    |<span data-ttu-id="84404-108">说明</span><span class="sxs-lookup"><span data-stu-id="84404-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84404-109">获取 ChartAxis</span><span class="sxs-lookup"><span data-stu-id="84404-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="84404-110">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="84404-110">workbookChartAxis</span></span>](workbookchartaxis.md) |<span data-ttu-id="84404-111">读取 chartaxis 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84404-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="84404-112">更新</span><span class="sxs-lookup"><span data-stu-id="84404-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="84404-113">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="84404-113">workbookChartAxis</span></span>](workbookchartaxis.md)   |<span data-ttu-id="84404-114">更新 ChartAxis 对象</span><span class="sxs-lookup"><span data-stu-id="84404-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="84404-115">属性</span><span class="sxs-lookup"><span data-stu-id="84404-115">Properties</span></span>
| <span data-ttu-id="84404-116">属性</span><span class="sxs-lookup"><span data-stu-id="84404-116">Property</span></span>     | <span data-ttu-id="84404-117">类型</span><span class="sxs-lookup"><span data-stu-id="84404-117">Type</span></span>   |<span data-ttu-id="84404-118">说明</span><span class="sxs-lookup"><span data-stu-id="84404-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="84404-119">id</span><span class="sxs-lookup"><span data-stu-id="84404-119">id</span></span>       |<span data-ttu-id="84404-120">string</span><span class="sxs-lookup"><span data-stu-id="84404-120">string</span></span>   | <span data-ttu-id="84404-121">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="84404-121">Unique identifier.</span></span> <span data-ttu-id="84404-122">只读。</span><span class="sxs-lookup"><span data-stu-id="84404-122">Read-only.</span></span>|
|<span data-ttu-id="84404-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="84404-123">majorUnit</span></span>|<span data-ttu-id="84404-124">Json</span><span class="sxs-lookup"><span data-stu-id="84404-124">Json</span></span>|<span data-ttu-id="84404-p102">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="84404-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="84404-128">maximum</span><span class="sxs-lookup"><span data-stu-id="84404-128">maximum</span></span>|<span data-ttu-id="84404-129">Json</span><span class="sxs-lookup"><span data-stu-id="84404-129">Json</span></span>|<span data-ttu-id="84404-p103">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="84404-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="84404-133">minimum</span><span class="sxs-lookup"><span data-stu-id="84404-133">minimum</span></span>|<span data-ttu-id="84404-134">Json</span><span class="sxs-lookup"><span data-stu-id="84404-134">Json</span></span>|<span data-ttu-id="84404-p104">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="84404-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="84404-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="84404-138">minorUnit</span></span>|<span data-ttu-id="84404-139">Json</span><span class="sxs-lookup"><span data-stu-id="84404-139">Json</span></span>|<span data-ttu-id="84404-p105">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="84404-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84404-143">关系</span><span class="sxs-lookup"><span data-stu-id="84404-143">Relationships</span></span>
| <span data-ttu-id="84404-144">关系</span><span class="sxs-lookup"><span data-stu-id="84404-144">Relationship</span></span> | <span data-ttu-id="84404-145">类型</span><span class="sxs-lookup"><span data-stu-id="84404-145">Type</span></span>   |<span data-ttu-id="84404-146">说明</span><span class="sxs-lookup"><span data-stu-id="84404-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84404-147">format</span><span class="sxs-lookup"><span data-stu-id="84404-147">format</span></span>|[<span data-ttu-id="84404-148">workbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="84404-148">workbookChartAxisFormat</span></span>](workbookchartaxisformat.md)|<span data-ttu-id="84404-p106">表示 chart 对象的格式，包括线条和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="84404-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="84404-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="84404-151">majorGridlines</span></span>|[<span data-ttu-id="84404-152">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="84404-152">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="84404-p107">返回一个表示指定坐标轴的主要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="84404-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="84404-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="84404-155">minorGridlines</span></span>|[<span data-ttu-id="84404-156">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="84404-156">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="84404-p108">返回一个表示指定坐标轴的次要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="84404-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="84404-159">title</span><span class="sxs-lookup"><span data-stu-id="84404-159">title</span></span>|[<span data-ttu-id="84404-160">workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="84404-160">workbookChartAxisTitle</span></span>](workbookchartaxistitle.md)|<span data-ttu-id="84404-161">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="84404-161">Represents the axis title.</span></span> <span data-ttu-id="84404-162">只读。</span><span class="sxs-lookup"><span data-stu-id="84404-162">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84404-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84404-163">JSON representation</span></span>

<span data-ttu-id="84404-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84404-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "title",
    "minorGridlines",
    "majorGridlines",
    "format"
   ],
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
