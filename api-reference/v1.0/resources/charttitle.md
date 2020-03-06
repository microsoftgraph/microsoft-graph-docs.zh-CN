---
title: ChartTitle 资源类型
description: 表示图表的图表标题对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2e3d30d1796945c7d0217a83db966a203678f938
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533093"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="d4825-103">ChartTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4825-103">ChartTitle resource type</span></span>

<span data-ttu-id="d4825-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4825-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4825-105">表示图表的图表标题对象。</span><span class="sxs-lookup"><span data-stu-id="d4825-105">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="d4825-106">Methods</span><span class="sxs-lookup"><span data-stu-id="d4825-106">Methods</span></span>

| <span data-ttu-id="d4825-107">方法</span><span class="sxs-lookup"><span data-stu-id="d4825-107">Method</span></span>           | <span data-ttu-id="d4825-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4825-108">Return Type</span></span>    |<span data-ttu-id="d4825-109">说明</span><span class="sxs-lookup"><span data-stu-id="d4825-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4825-110">获取 ChartTitle</span><span class="sxs-lookup"><span data-stu-id="d4825-110">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="d4825-111">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="d4825-111">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="d4825-112">读取 chartTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4825-112">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="d4825-113">更新</span><span class="sxs-lookup"><span data-stu-id="d4825-113">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="d4825-114">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="d4825-114">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="d4825-115">更新 ChartTitle 对象。</span><span class="sxs-lookup"><span data-stu-id="d4825-115">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4825-116">属性</span><span class="sxs-lookup"><span data-stu-id="d4825-116">Properties</span></span>
| <span data-ttu-id="d4825-117">属性</span><span class="sxs-lookup"><span data-stu-id="d4825-117">Property</span></span>     | <span data-ttu-id="d4825-118">类型</span><span class="sxs-lookup"><span data-stu-id="d4825-118">Type</span></span>   |<span data-ttu-id="d4825-119">说明</span><span class="sxs-lookup"><span data-stu-id="d4825-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4825-120">overlay</span><span class="sxs-lookup"><span data-stu-id="d4825-120">overlay</span></span>|<span data-ttu-id="d4825-121">布尔</span><span class="sxs-lookup"><span data-stu-id="d4825-121">boolean</span></span>|<span data-ttu-id="d4825-122">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d4825-122">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="d4825-123">text</span><span class="sxs-lookup"><span data-stu-id="d4825-123">text</span></span>|<span data-ttu-id="d4825-124">string</span><span class="sxs-lookup"><span data-stu-id="d4825-124">string</span></span>|<span data-ttu-id="d4825-125">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="d4825-125">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="d4825-126">visible</span><span class="sxs-lookup"><span data-stu-id="d4825-126">visible</span></span>|<span data-ttu-id="d4825-127">布尔</span><span class="sxs-lookup"><span data-stu-id="d4825-127">boolean</span></span>|<span data-ttu-id="d4825-128">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d4825-128">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4825-129">关系</span><span class="sxs-lookup"><span data-stu-id="d4825-129">Relationships</span></span>
| <span data-ttu-id="d4825-130">关系</span><span class="sxs-lookup"><span data-stu-id="d4825-130">Relationship</span></span> | <span data-ttu-id="d4825-131">类型</span><span class="sxs-lookup"><span data-stu-id="d4825-131">Type</span></span>   |<span data-ttu-id="d4825-132">说明</span><span class="sxs-lookup"><span data-stu-id="d4825-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4825-133">format</span><span class="sxs-lookup"><span data-stu-id="d4825-133">format</span></span>|[<span data-ttu-id="d4825-134">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="d4825-134">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="d4825-135">表示图表标题的格式，包括填充和字体格式。</span><span class="sxs-lookup"><span data-stu-id="d4825-135">Represents the formatting of a chart title, which includes fill and font formatting.</span></span> <span data-ttu-id="d4825-136">只读。</span><span class="sxs-lookup"><span data-stu-id="d4825-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4825-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4825-137">JSON representation</span></span>

<span data-ttu-id="d4825-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4825-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
