---
title: ChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3c57c68e7d9dfcd26741d15e302dd5dddeaae378
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572533"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="56993-103">ChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="56993-103">ChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56993-104">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="56993-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="56993-105">方法</span><span class="sxs-lookup"><span data-stu-id="56993-105">Methods</span></span>

| <span data-ttu-id="56993-106">方法</span><span class="sxs-lookup"><span data-stu-id="56993-106">Method</span></span>           | <span data-ttu-id="56993-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="56993-107">Return Type</span></span>    |<span data-ttu-id="56993-108">说明</span><span class="sxs-lookup"><span data-stu-id="56993-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56993-109">获取 ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="56993-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="56993-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="56993-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="56993-111">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56993-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="56993-112">Update</span><span class="sxs-lookup"><span data-stu-id="56993-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="56993-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="56993-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="56993-114">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="56993-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="56993-115">属性</span><span class="sxs-lookup"><span data-stu-id="56993-115">Properties</span></span>
| <span data-ttu-id="56993-116">属性</span><span class="sxs-lookup"><span data-stu-id="56993-116">Property</span></span>     | <span data-ttu-id="56993-117">类型</span><span class="sxs-lookup"><span data-stu-id="56993-117">Type</span></span>   |<span data-ttu-id="56993-118">说明</span><span class="sxs-lookup"><span data-stu-id="56993-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56993-119">visible</span><span class="sxs-lookup"><span data-stu-id="56993-119">visible</span></span>|<span data-ttu-id="56993-120">布尔</span><span class="sxs-lookup"><span data-stu-id="56993-120">boolean</span></span>|<span data-ttu-id="56993-121">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="56993-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56993-122">关系</span><span class="sxs-lookup"><span data-stu-id="56993-122">Relationships</span></span>
| <span data-ttu-id="56993-123">关系</span><span class="sxs-lookup"><span data-stu-id="56993-123">Relationship</span></span> | <span data-ttu-id="56993-124">类型</span><span class="sxs-lookup"><span data-stu-id="56993-124">Type</span></span>   |<span data-ttu-id="56993-125">说明</span><span class="sxs-lookup"><span data-stu-id="56993-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56993-126">format</span><span class="sxs-lookup"><span data-stu-id="56993-126">format</span></span>|[<span data-ttu-id="56993-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="56993-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="56993-p101">表示图表网格线的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="56993-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56993-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56993-130">JSON representation</span></span>

<span data-ttu-id="56993-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56993-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlines.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
