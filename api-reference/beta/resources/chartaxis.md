---
title: ChartAxis 资源类型
description: 表示图表中的单个坐标轴。
ms.openlocfilehash: f92e8dd12dc2d7036d5022e2b293cfc290faf910
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045926"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="fb7a9-103">ChartAxis 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb7a9-103">ChartAxis resource type</span></span>

> <span data-ttu-id="fb7a9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb7a9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb7a9-106">代表图表中的单个坐标轴。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-106">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="fb7a9-107">方法</span><span class="sxs-lookup"><span data-stu-id="fb7a9-107">Methods</span></span>

| <span data-ttu-id="fb7a9-108">方法</span><span class="sxs-lookup"><span data-stu-id="fb7a9-108">Method</span></span>           | <span data-ttu-id="fb7a9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fb7a9-109">Return Type</span></span>    |<span data-ttu-id="fb7a9-110">说明</span><span class="sxs-lookup"><span data-stu-id="fb7a9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb7a9-111">获取 ChartAxis</span><span class="sxs-lookup"><span data-stu-id="fb7a9-111">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="fb7a9-112">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="fb7a9-112">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="fb7a9-113">读取 chartaxis 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-113">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="fb7a9-114">Update</span><span class="sxs-lookup"><span data-stu-id="fb7a9-114">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="fb7a9-115">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="fb7a9-115">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="fb7a9-116">更新 ChartAxis 对象</span><span class="sxs-lookup"><span data-stu-id="fb7a9-116">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fb7a9-117">属性</span><span class="sxs-lookup"><span data-stu-id="fb7a9-117">Properties</span></span>
| <span data-ttu-id="fb7a9-118">属性</span><span class="sxs-lookup"><span data-stu-id="fb7a9-118">Property</span></span>     | <span data-ttu-id="fb7a9-119">类型</span><span class="sxs-lookup"><span data-stu-id="fb7a9-119">Type</span></span>   |<span data-ttu-id="fb7a9-120">说明</span><span class="sxs-lookup"><span data-stu-id="fb7a9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb7a9-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="fb7a9-121">majorUnit</span></span>|<span data-ttu-id="fb7a9-122">对象</span><span class="sxs-lookup"><span data-stu-id="fb7a9-122">object</span></span>|<span data-ttu-id="fb7a9-p102">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="fb7a9-126">maximum</span><span class="sxs-lookup"><span data-stu-id="fb7a9-126">maximum</span></span>|<span data-ttu-id="fb7a9-127">对象</span><span class="sxs-lookup"><span data-stu-id="fb7a9-127">object</span></span>|<span data-ttu-id="fb7a9-p103">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="fb7a9-131">minimum</span><span class="sxs-lookup"><span data-stu-id="fb7a9-131">minimum</span></span>|<span data-ttu-id="fb7a9-132">对象</span><span class="sxs-lookup"><span data-stu-id="fb7a9-132">object</span></span>|<span data-ttu-id="fb7a9-p104">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="fb7a9-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="fb7a9-136">minorUnit</span></span>|<span data-ttu-id="fb7a9-137">对象</span><span class="sxs-lookup"><span data-stu-id="fb7a9-137">object</span></span>|<span data-ttu-id="fb7a9-p105">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb7a9-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="fb7a9-141">Relationships</span></span>
| <span data-ttu-id="fb7a9-142">关系</span><span class="sxs-lookup"><span data-stu-id="fb7a9-142">Relationship</span></span> | <span data-ttu-id="fb7a9-143">类型</span><span class="sxs-lookup"><span data-stu-id="fb7a9-143">Type</span></span>   |<span data-ttu-id="fb7a9-144">说明</span><span class="sxs-lookup"><span data-stu-id="fb7a9-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb7a9-145">format</span><span class="sxs-lookup"><span data-stu-id="fb7a9-145">format</span></span>|[<span data-ttu-id="fb7a9-146">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="fb7a9-146">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="fb7a9-p106">表示 chart 对象的格式，包括线条和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="fb7a9-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="fb7a9-149">majorGridlines</span></span>|[<span data-ttu-id="fb7a9-150">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="fb7a9-150">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="fb7a9-p107">返回一个表示指定坐标轴的主要网格线的 gridline 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="fb7a9-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="fb7a9-153">minorGridlines</span></span>|[<span data-ttu-id="fb7a9-154">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="fb7a9-154">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="fb7a9-p108">返回一个表示指定坐标轴的次要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="fb7a9-157">title</span><span class="sxs-lookup"><span data-stu-id="fb7a9-157">title</span></span>|[<span data-ttu-id="fb7a9-158">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="fb7a9-158">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="fb7a9-p109">表示坐标轴标题。只读。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb7a9-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb7a9-161">JSON representation</span></span>

<span data-ttu-id="fb7a9-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb7a9-162">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->