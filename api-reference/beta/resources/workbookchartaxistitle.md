---
title: workbookChartAxisTitle 资源类型
description: 表示图表坐标轴的标题。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 543a13042f4245f90b799f6298a3f29c6368ea8f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519363"
---
# <a name="workbookchartaxistitle-resource-type"></a><span data-ttu-id="5ef49-103">workbookChartAxisTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ef49-103">workbookChartAxisTitle resource type</span></span>

<span data-ttu-id="5ef49-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5ef49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ef49-105">表示图表坐标轴的标题。</span><span class="sxs-lookup"><span data-stu-id="5ef49-105">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="5ef49-106">方法</span><span class="sxs-lookup"><span data-stu-id="5ef49-106">Methods</span></span>

| <span data-ttu-id="5ef49-107">方法</span><span class="sxs-lookup"><span data-stu-id="5ef49-107">Method</span></span>           | <span data-ttu-id="5ef49-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5ef49-108">Return Type</span></span>    |<span data-ttu-id="5ef49-109">说明</span><span class="sxs-lookup"><span data-stu-id="5ef49-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ef49-110">获取 ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="5ef49-110">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="5ef49-111">workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="5ef49-111">workbookChartAxisTitle</span></span>](workbookchartaxistitle.md) |<span data-ttu-id="5ef49-112">读取 chartAxisTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5ef49-112">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="5ef49-113">更新</span><span class="sxs-lookup"><span data-stu-id="5ef49-113">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="5ef49-114">workbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="5ef49-114">workbookChartAxisTitle</span></span>](workbookchartaxistitle.md)    |<span data-ttu-id="5ef49-115">更新 ChartAxisTitle 对象</span><span class="sxs-lookup"><span data-stu-id="5ef49-115">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5ef49-116">属性</span><span class="sxs-lookup"><span data-stu-id="5ef49-116">Properties</span></span>
| <span data-ttu-id="5ef49-117">属性</span><span class="sxs-lookup"><span data-stu-id="5ef49-117">Property</span></span>     | <span data-ttu-id="5ef49-118">类型</span><span class="sxs-lookup"><span data-stu-id="5ef49-118">Type</span></span>   |<span data-ttu-id="5ef49-119">说明</span><span class="sxs-lookup"><span data-stu-id="5ef49-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ef49-120">text</span><span class="sxs-lookup"><span data-stu-id="5ef49-120">text</span></span>|<span data-ttu-id="5ef49-121">string</span><span class="sxs-lookup"><span data-stu-id="5ef49-121">string</span></span>|<span data-ttu-id="5ef49-122">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="5ef49-122">Represents the axis title.</span></span>|
|<span data-ttu-id="5ef49-123">visible</span><span class="sxs-lookup"><span data-stu-id="5ef49-123">visible</span></span>|<span data-ttu-id="5ef49-124">布尔</span><span class="sxs-lookup"><span data-stu-id="5ef49-124">boolean</span></span>|<span data-ttu-id="5ef49-125">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="5ef49-125">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ef49-126">关系</span><span class="sxs-lookup"><span data-stu-id="5ef49-126">Relationships</span></span>
| <span data-ttu-id="5ef49-127">关系</span><span class="sxs-lookup"><span data-stu-id="5ef49-127">Relationship</span></span> | <span data-ttu-id="5ef49-128">类型</span><span class="sxs-lookup"><span data-stu-id="5ef49-128">Type</span></span>   |<span data-ttu-id="5ef49-129">说明</span><span class="sxs-lookup"><span data-stu-id="5ef49-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ef49-130">format</span><span class="sxs-lookup"><span data-stu-id="5ef49-130">format</span></span>|[<span data-ttu-id="5ef49-131">workbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="5ef49-131">workbookChartAxisTitleFormat</span></span>](workbookchartaxistitleformat.md)|<span data-ttu-id="5ef49-132">表示图表坐标轴标题的格式。</span><span class="sxs-lookup"><span data-stu-id="5ef49-132">Represents the formatting of chart axis title.</span></span> <span data-ttu-id="5ef49-133">只读。</span><span class="sxs-lookup"><span data-stu-id="5ef49-133">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ef49-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ef49-134">JSON representation</span></span>

<span data-ttu-id="5ef49-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ef49-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "format"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
