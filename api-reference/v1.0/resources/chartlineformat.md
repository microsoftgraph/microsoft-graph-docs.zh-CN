---
title: ChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 505e6d88e0c1b19ea33d475b6d8edf3485e29cea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032961"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="d9543-103">ChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9543-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="d9543-104">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="d9543-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="d9543-105">方法</span><span class="sxs-lookup"><span data-stu-id="d9543-105">Methods</span></span>

| <span data-ttu-id="d9543-106">方法</span><span class="sxs-lookup"><span data-stu-id="d9543-106">Method</span></span>           | <span data-ttu-id="d9543-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9543-107">Return Type</span></span>    |<span data-ttu-id="d9543-108">说明</span><span class="sxs-lookup"><span data-stu-id="d9543-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9543-109">获取 ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d9543-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="d9543-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d9543-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="d9543-111">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9543-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="d9543-112">更新</span><span class="sxs-lookup"><span data-stu-id="d9543-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="d9543-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="d9543-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="d9543-114">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="d9543-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="d9543-115">清除</span><span class="sxs-lookup"><span data-stu-id="d9543-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="d9543-116">None</span><span class="sxs-lookup"><span data-stu-id="d9543-116">None</span></span>|<span data-ttu-id="d9543-117">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="d9543-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9543-118">属性</span><span class="sxs-lookup"><span data-stu-id="d9543-118">Properties</span></span>
| <span data-ttu-id="d9543-119">属性</span><span class="sxs-lookup"><span data-stu-id="d9543-119">Property</span></span>     | <span data-ttu-id="d9543-120">类型</span><span class="sxs-lookup"><span data-stu-id="d9543-120">Type</span></span>   |<span data-ttu-id="d9543-121">说明</span><span class="sxs-lookup"><span data-stu-id="d9543-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9543-122">color</span><span class="sxs-lookup"><span data-stu-id="d9543-122">color</span></span>|<span data-ttu-id="d9543-123">string</span><span class="sxs-lookup"><span data-stu-id="d9543-123">string</span></span>|<span data-ttu-id="d9543-124">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="d9543-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9543-125">关系</span><span class="sxs-lookup"><span data-stu-id="d9543-125">Relationships</span></span>
<span data-ttu-id="d9543-126">无</span><span class="sxs-lookup"><span data-stu-id="d9543-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d9543-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9543-127">JSON representation</span></span>

<span data-ttu-id="d9543-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9543-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
