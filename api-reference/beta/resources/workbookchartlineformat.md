---
title: workbookChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fe36b0448d430566b51ee836e93d02f08cdbdbd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007240"
---
# <a name="workbookchartlineformat-resource-type"></a><span data-ttu-id="41e31-103">workbookChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="41e31-103">workbookChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41e31-104">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="41e31-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="41e31-105">方法</span><span class="sxs-lookup"><span data-stu-id="41e31-105">Methods</span></span>

| <span data-ttu-id="41e31-106">方法</span><span class="sxs-lookup"><span data-stu-id="41e31-106">Method</span></span>           | <span data-ttu-id="41e31-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="41e31-107">Return Type</span></span>    |<span data-ttu-id="41e31-108">说明</span><span class="sxs-lookup"><span data-stu-id="41e31-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41e31-109">获取 workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="41e31-109">Get workbookChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="41e31-110">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="41e31-110">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="41e31-111">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41e31-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="41e31-112">更新</span><span class="sxs-lookup"><span data-stu-id="41e31-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="41e31-113">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="41e31-113">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="41e31-114">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="41e31-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="41e31-115">清除</span><span class="sxs-lookup"><span data-stu-id="41e31-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="41e31-116">None</span><span class="sxs-lookup"><span data-stu-id="41e31-116">None</span></span>|<span data-ttu-id="41e31-117">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="41e31-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="41e31-118">属性</span><span class="sxs-lookup"><span data-stu-id="41e31-118">Properties</span></span>
| <span data-ttu-id="41e31-119">属性</span><span class="sxs-lookup"><span data-stu-id="41e31-119">Property</span></span>     | <span data-ttu-id="41e31-120">类型</span><span class="sxs-lookup"><span data-stu-id="41e31-120">Type</span></span>   |<span data-ttu-id="41e31-121">说明</span><span class="sxs-lookup"><span data-stu-id="41e31-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41e31-122">color</span><span class="sxs-lookup"><span data-stu-id="41e31-122">color</span></span>|<span data-ttu-id="41e31-123">string</span><span class="sxs-lookup"><span data-stu-id="41e31-123">string</span></span>|<span data-ttu-id="41e31-124">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="41e31-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41e31-125">关系</span><span class="sxs-lookup"><span data-stu-id="41e31-125">Relationships</span></span>
<span data-ttu-id="41e31-126">无</span><span class="sxs-lookup"><span data-stu-id="41e31-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="41e31-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41e31-127">JSON representation</span></span>

<span data-ttu-id="41e31-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41e31-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
