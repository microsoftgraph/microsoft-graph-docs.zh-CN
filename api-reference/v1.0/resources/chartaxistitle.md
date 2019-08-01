---
title: ChartAxisTitle 资源类型
description: 表示图表坐标轴的标题。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5c89b3e90cce7dcc064dfd7186eafcc26a37dd0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033024"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="01dab-103">ChartAxisTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="01dab-103">ChartAxisTitle resource type</span></span>

<span data-ttu-id="01dab-104">表示图表坐标轴的标题。</span><span class="sxs-lookup"><span data-stu-id="01dab-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="01dab-105">方法</span><span class="sxs-lookup"><span data-stu-id="01dab-105">Methods</span></span>

| <span data-ttu-id="01dab-106">方法</span><span class="sxs-lookup"><span data-stu-id="01dab-106">Method</span></span>           | <span data-ttu-id="01dab-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="01dab-107">Return Type</span></span>    |<span data-ttu-id="01dab-108">说明</span><span class="sxs-lookup"><span data-stu-id="01dab-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01dab-109">获取 ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="01dab-109">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="01dab-110">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="01dab-110">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="01dab-111">读取 chartAxisTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="01dab-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="01dab-112">更新</span><span class="sxs-lookup"><span data-stu-id="01dab-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="01dab-113">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="01dab-113">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="01dab-114">更新 ChartAxisTitle 对象</span><span class="sxs-lookup"><span data-stu-id="01dab-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="01dab-115">属性</span><span class="sxs-lookup"><span data-stu-id="01dab-115">Properties</span></span>
| <span data-ttu-id="01dab-116">属性</span><span class="sxs-lookup"><span data-stu-id="01dab-116">Property</span></span>     | <span data-ttu-id="01dab-117">类型</span><span class="sxs-lookup"><span data-stu-id="01dab-117">Type</span></span>   |<span data-ttu-id="01dab-118">说明</span><span class="sxs-lookup"><span data-stu-id="01dab-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01dab-119">text</span><span class="sxs-lookup"><span data-stu-id="01dab-119">text</span></span>|<span data-ttu-id="01dab-120">string</span><span class="sxs-lookup"><span data-stu-id="01dab-120">string</span></span>|<span data-ttu-id="01dab-121">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="01dab-121">Represents the axis title.</span></span>|
|<span data-ttu-id="01dab-122">visible</span><span class="sxs-lookup"><span data-stu-id="01dab-122">visible</span></span>|<span data-ttu-id="01dab-123">布尔</span><span class="sxs-lookup"><span data-stu-id="01dab-123">boolean</span></span>|<span data-ttu-id="01dab-124">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="01dab-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01dab-125">关系</span><span class="sxs-lookup"><span data-stu-id="01dab-125">Relationships</span></span>
| <span data-ttu-id="01dab-126">关系</span><span class="sxs-lookup"><span data-stu-id="01dab-126">Relationship</span></span> | <span data-ttu-id="01dab-127">类型</span><span class="sxs-lookup"><span data-stu-id="01dab-127">Type</span></span>   |<span data-ttu-id="01dab-128">说明</span><span class="sxs-lookup"><span data-stu-id="01dab-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01dab-129">format</span><span class="sxs-lookup"><span data-stu-id="01dab-129">format</span></span>|[<span data-ttu-id="01dab-130">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="01dab-130">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="01dab-131">表示图表坐标轴标题的格式。</span><span class="sxs-lookup"><span data-stu-id="01dab-131">Represents the formatting of chart axis title.</span></span> <span data-ttu-id="01dab-132">只读。</span><span class="sxs-lookup"><span data-stu-id="01dab-132">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01dab-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01dab-133">JSON representation</span></span>

<span data-ttu-id="01dab-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01dab-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
