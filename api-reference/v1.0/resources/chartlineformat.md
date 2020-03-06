---
title: ChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7224f7d5d0b41814c17081eefab79de47ca89ebb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533116"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="8f65f-103">ChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f65f-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="8f65f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f65f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f65f-105">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="8f65f-105">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="8f65f-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8f65f-106">Methods</span></span>

| <span data-ttu-id="8f65f-107">方法</span><span class="sxs-lookup"><span data-stu-id="8f65f-107">Method</span></span>           | <span data-ttu-id="8f65f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f65f-108">Return Type</span></span>    |<span data-ttu-id="8f65f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8f65f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f65f-110">获取 ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8f65f-110">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="8f65f-111">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8f65f-111">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="8f65f-112">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8f65f-112">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="8f65f-113">更新</span><span class="sxs-lookup"><span data-stu-id="8f65f-113">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="8f65f-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8f65f-114">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="8f65f-115">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="8f65f-115">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="8f65f-116">清除</span><span class="sxs-lookup"><span data-stu-id="8f65f-116">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="8f65f-117">None</span><span class="sxs-lookup"><span data-stu-id="8f65f-117">None</span></span>|<span data-ttu-id="8f65f-118">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="8f65f-118">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f65f-119">属性</span><span class="sxs-lookup"><span data-stu-id="8f65f-119">Properties</span></span>
| <span data-ttu-id="8f65f-120">属性</span><span class="sxs-lookup"><span data-stu-id="8f65f-120">Property</span></span>     | <span data-ttu-id="8f65f-121">类型</span><span class="sxs-lookup"><span data-stu-id="8f65f-121">Type</span></span>   |<span data-ttu-id="8f65f-122">说明</span><span class="sxs-lookup"><span data-stu-id="8f65f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f65f-123">color</span><span class="sxs-lookup"><span data-stu-id="8f65f-123">color</span></span>|<span data-ttu-id="8f65f-124">string</span><span class="sxs-lookup"><span data-stu-id="8f65f-124">string</span></span>|<span data-ttu-id="8f65f-125">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="8f65f-125">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f65f-126">关系</span><span class="sxs-lookup"><span data-stu-id="8f65f-126">Relationships</span></span>
<span data-ttu-id="8f65f-127">无</span><span class="sxs-lookup"><span data-stu-id="8f65f-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f65f-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f65f-128">JSON representation</span></span>

<span data-ttu-id="8f65f-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f65f-129">Here is a JSON representation of the resource.</span></span>

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
