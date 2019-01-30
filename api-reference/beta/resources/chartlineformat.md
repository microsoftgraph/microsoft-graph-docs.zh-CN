---
title: ChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b4409eb18dab41d43adc038b702a65fa8d63e4de
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640579"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="38763-103">ChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="38763-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38763-104">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="38763-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="38763-105">方法</span><span class="sxs-lookup"><span data-stu-id="38763-105">Methods</span></span>

| <span data-ttu-id="38763-106">方法</span><span class="sxs-lookup"><span data-stu-id="38763-106">Method</span></span>           | <span data-ttu-id="38763-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="38763-107">Return Type</span></span>    |<span data-ttu-id="38763-108">说明</span><span class="sxs-lookup"><span data-stu-id="38763-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38763-109">获取 ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="38763-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="38763-110">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="38763-110">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="38763-111">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38763-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="38763-112">更新</span><span class="sxs-lookup"><span data-stu-id="38763-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="38763-113">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="38763-113">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="38763-114">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="38763-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="38763-115">清除</span><span class="sxs-lookup"><span data-stu-id="38763-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="38763-116">无</span><span class="sxs-lookup"><span data-stu-id="38763-116">None</span></span>|<span data-ttu-id="38763-117">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="38763-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="38763-118">属性</span><span class="sxs-lookup"><span data-stu-id="38763-118">Properties</span></span>
| <span data-ttu-id="38763-119">属性</span><span class="sxs-lookup"><span data-stu-id="38763-119">Property</span></span>     | <span data-ttu-id="38763-120">类型</span><span class="sxs-lookup"><span data-stu-id="38763-120">Type</span></span>   |<span data-ttu-id="38763-121">说明</span><span class="sxs-lookup"><span data-stu-id="38763-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38763-122">color</span><span class="sxs-lookup"><span data-stu-id="38763-122">color</span></span>|<span data-ttu-id="38763-123">string</span><span class="sxs-lookup"><span data-stu-id="38763-123">string</span></span>|<span data-ttu-id="38763-124">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="38763-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38763-125">关系</span><span class="sxs-lookup"><span data-stu-id="38763-125">Relationships</span></span>
<span data-ttu-id="38763-126">无</span><span class="sxs-lookup"><span data-stu-id="38763-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="38763-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38763-127">JSON representation</span></span>

<span data-ttu-id="38763-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38763-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
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
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlineformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
