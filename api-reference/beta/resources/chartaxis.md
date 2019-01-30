---
title: ChartAxis 资源类型
description: 表示图表中的单个坐标轴。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640929"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="93e57-103">ChartAxis 资源类型</span><span class="sxs-lookup"><span data-stu-id="93e57-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93e57-104">表示图表中的单个坐标轴。</span><span class="sxs-lookup"><span data-stu-id="93e57-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="93e57-105">方法</span><span class="sxs-lookup"><span data-stu-id="93e57-105">Methods</span></span>

| <span data-ttu-id="93e57-106">方法</span><span class="sxs-lookup"><span data-stu-id="93e57-106">Method</span></span>           | <span data-ttu-id="93e57-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="93e57-107">Return Type</span></span>    |<span data-ttu-id="93e57-108">说明</span><span class="sxs-lookup"><span data-stu-id="93e57-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93e57-109">获取 ChartAxis</span><span class="sxs-lookup"><span data-stu-id="93e57-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="93e57-110">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="93e57-110">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="93e57-111">读取 chartaxis 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="93e57-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="93e57-112">更新</span><span class="sxs-lookup"><span data-stu-id="93e57-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="93e57-113">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="93e57-113">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="93e57-114">更新 ChartAxis 对象</span><span class="sxs-lookup"><span data-stu-id="93e57-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="93e57-115">属性</span><span class="sxs-lookup"><span data-stu-id="93e57-115">Properties</span></span>
| <span data-ttu-id="93e57-116">属性</span><span class="sxs-lookup"><span data-stu-id="93e57-116">Property</span></span>     | <span data-ttu-id="93e57-117">类型</span><span class="sxs-lookup"><span data-stu-id="93e57-117">Type</span></span>   |<span data-ttu-id="93e57-118">说明</span><span class="sxs-lookup"><span data-stu-id="93e57-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93e57-119">majorUnit</span><span class="sxs-lookup"><span data-stu-id="93e57-119">majorUnit</span></span>|<span data-ttu-id="93e57-120">对象</span><span class="sxs-lookup"><span data-stu-id="93e57-120">object</span></span>|<span data-ttu-id="93e57-p101">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="93e57-p101">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="93e57-124">maximum</span><span class="sxs-lookup"><span data-stu-id="93e57-124">maximum</span></span>|<span data-ttu-id="93e57-125">对象</span><span class="sxs-lookup"><span data-stu-id="93e57-125">object</span></span>|<span data-ttu-id="93e57-p102">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="93e57-p102">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="93e57-129">minimum</span><span class="sxs-lookup"><span data-stu-id="93e57-129">minimum</span></span>|<span data-ttu-id="93e57-130">对象</span><span class="sxs-lookup"><span data-stu-id="93e57-130">object</span></span>|<span data-ttu-id="93e57-p103">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="93e57-p103">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="93e57-134">minorUnit</span><span class="sxs-lookup"><span data-stu-id="93e57-134">minorUnit</span></span>|<span data-ttu-id="93e57-135">对象</span><span class="sxs-lookup"><span data-stu-id="93e57-135">object</span></span>|<span data-ttu-id="93e57-p104">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="93e57-p104">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93e57-139">关系</span><span class="sxs-lookup"><span data-stu-id="93e57-139">Relationships</span></span>
| <span data-ttu-id="93e57-140">关系</span><span class="sxs-lookup"><span data-stu-id="93e57-140">Relationship</span></span> | <span data-ttu-id="93e57-141">类型</span><span class="sxs-lookup"><span data-stu-id="93e57-141">Type</span></span>   |<span data-ttu-id="93e57-142">说明</span><span class="sxs-lookup"><span data-stu-id="93e57-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93e57-143">format</span><span class="sxs-lookup"><span data-stu-id="93e57-143">format</span></span>|[<span data-ttu-id="93e57-144">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="93e57-144">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="93e57-p105">表示 chart 对象的格式，包括线条和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="93e57-p105">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="93e57-147">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="93e57-147">majorGridlines</span></span>|[<span data-ttu-id="93e57-148">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="93e57-148">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="93e57-p106">返回一个表示指定坐标轴的主要网格线的 gridline 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="93e57-p106">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="93e57-151">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="93e57-151">minorGridlines</span></span>|[<span data-ttu-id="93e57-152">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="93e57-152">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="93e57-p107">返回一个表示指定坐标轴的次要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="93e57-p107">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="93e57-155">title</span><span class="sxs-lookup"><span data-stu-id="93e57-155">title</span></span>|[<span data-ttu-id="93e57-156">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="93e57-156">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="93e57-p108">表示坐标轴标题。只读。</span><span class="sxs-lookup"><span data-stu-id="93e57-p108">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93e57-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93e57-159">JSON representation</span></span>

<span data-ttu-id="93e57-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93e57-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxis.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
