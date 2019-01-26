---
title: ChartTitle 资源类型
description: 表示图表的 chart title 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0b669593bd9ca0768ad977ace8d54f5531301a4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573093"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="40791-103">ChartTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="40791-103">ChartTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40791-104">表示图表的 chart title 对象。</span><span class="sxs-lookup"><span data-stu-id="40791-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="40791-105">方法</span><span class="sxs-lookup"><span data-stu-id="40791-105">Methods</span></span>

| <span data-ttu-id="40791-106">方法</span><span class="sxs-lookup"><span data-stu-id="40791-106">Method</span></span>           | <span data-ttu-id="40791-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="40791-107">Return Type</span></span>    |<span data-ttu-id="40791-108">说明</span><span class="sxs-lookup"><span data-stu-id="40791-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40791-109">获取 ChartTitle</span><span class="sxs-lookup"><span data-stu-id="40791-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="40791-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="40791-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="40791-111">读取 chartTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="40791-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="40791-112">Update</span><span class="sxs-lookup"><span data-stu-id="40791-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="40791-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="40791-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="40791-114">更新 ChartTitle 对象。</span><span class="sxs-lookup"><span data-stu-id="40791-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="40791-115">属性</span><span class="sxs-lookup"><span data-stu-id="40791-115">Properties</span></span>
| <span data-ttu-id="40791-116">属性</span><span class="sxs-lookup"><span data-stu-id="40791-116">Property</span></span>     | <span data-ttu-id="40791-117">类型</span><span class="sxs-lookup"><span data-stu-id="40791-117">Type</span></span>   |<span data-ttu-id="40791-118">说明</span><span class="sxs-lookup"><span data-stu-id="40791-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40791-119">overlay</span><span class="sxs-lookup"><span data-stu-id="40791-119">overlay</span></span>|<span data-ttu-id="40791-120">布尔</span><span class="sxs-lookup"><span data-stu-id="40791-120">boolean</span></span>|<span data-ttu-id="40791-121">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="40791-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="40791-122">text</span><span class="sxs-lookup"><span data-stu-id="40791-122">text</span></span>|<span data-ttu-id="40791-123">string</span><span class="sxs-lookup"><span data-stu-id="40791-123">string</span></span>|<span data-ttu-id="40791-124">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="40791-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="40791-125">visible</span><span class="sxs-lookup"><span data-stu-id="40791-125">visible</span></span>|<span data-ttu-id="40791-126">布尔</span><span class="sxs-lookup"><span data-stu-id="40791-126">boolean</span></span>|<span data-ttu-id="40791-127">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="40791-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40791-128">关系</span><span class="sxs-lookup"><span data-stu-id="40791-128">Relationships</span></span>
| <span data-ttu-id="40791-129">关系</span><span class="sxs-lookup"><span data-stu-id="40791-129">Relationship</span></span> | <span data-ttu-id="40791-130">类型</span><span class="sxs-lookup"><span data-stu-id="40791-130">Type</span></span>   |<span data-ttu-id="40791-131">说明</span><span class="sxs-lookup"><span data-stu-id="40791-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40791-132">format</span><span class="sxs-lookup"><span data-stu-id="40791-132">format</span></span>|[<span data-ttu-id="40791-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="40791-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="40791-p101">表示图表标题的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="40791-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40791-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40791-136">JSON representation</span></span>

<span data-ttu-id="40791-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40791-137">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
