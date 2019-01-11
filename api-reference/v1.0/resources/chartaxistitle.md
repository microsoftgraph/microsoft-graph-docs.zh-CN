---
title: ChartAxisTitle 资源类型
description: 表示图表坐标轴的标题。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b1d212fd2fa55a01971c5d58026fcbe56f1c5116
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822006"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="294da-103">ChartAxisTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="294da-103">ChartAxisTitle resource type</span></span>

<span data-ttu-id="294da-104">表示图表坐标轴的标题。</span><span class="sxs-lookup"><span data-stu-id="294da-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="294da-105">方法</span><span class="sxs-lookup"><span data-stu-id="294da-105">Methods</span></span>

| <span data-ttu-id="294da-106">方法</span><span class="sxs-lookup"><span data-stu-id="294da-106">Method</span></span>           | <span data-ttu-id="294da-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="294da-107">Return Type</span></span>    |<span data-ttu-id="294da-108">说明</span><span class="sxs-lookup"><span data-stu-id="294da-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="294da-109">获取 ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="294da-109">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="294da-110">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="294da-110">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="294da-111">读取 chartAxisTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="294da-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="294da-112">Update</span><span class="sxs-lookup"><span data-stu-id="294da-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="294da-113">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="294da-113">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="294da-114">更新 ChartAxisTitle 对象</span><span class="sxs-lookup"><span data-stu-id="294da-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="294da-115">属性</span><span class="sxs-lookup"><span data-stu-id="294da-115">Properties</span></span>
| <span data-ttu-id="294da-116">属性</span><span class="sxs-lookup"><span data-stu-id="294da-116">Property</span></span>     | <span data-ttu-id="294da-117">类型</span><span class="sxs-lookup"><span data-stu-id="294da-117">Type</span></span>   |<span data-ttu-id="294da-118">说明</span><span class="sxs-lookup"><span data-stu-id="294da-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="294da-119">text</span><span class="sxs-lookup"><span data-stu-id="294da-119">text</span></span>|<span data-ttu-id="294da-120">string</span><span class="sxs-lookup"><span data-stu-id="294da-120">string</span></span>|<span data-ttu-id="294da-121">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="294da-121">Represents the axis title.</span></span>|
|<span data-ttu-id="294da-122">visible</span><span class="sxs-lookup"><span data-stu-id="294da-122">visible</span></span>|<span data-ttu-id="294da-123">boolean</span><span class="sxs-lookup"><span data-stu-id="294da-123">boolean</span></span>|<span data-ttu-id="294da-124">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="294da-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="294da-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="294da-125">Relationships</span></span>
| <span data-ttu-id="294da-126">关系</span><span class="sxs-lookup"><span data-stu-id="294da-126">Relationship</span></span> | <span data-ttu-id="294da-127">类型</span><span class="sxs-lookup"><span data-stu-id="294da-127">Type</span></span>   |<span data-ttu-id="294da-128">说明</span><span class="sxs-lookup"><span data-stu-id="294da-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="294da-129">format</span><span class="sxs-lookup"><span data-stu-id="294da-129">format</span></span>|[<span data-ttu-id="294da-130">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="294da-130">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="294da-p101">表示图表坐标轴标题的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="294da-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="294da-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="294da-133">JSON representation</span></span>

<span data-ttu-id="294da-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="294da-134">Here is a JSON representation of the resource.</span></span>

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
