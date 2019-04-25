---
title: ChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 852b52fd70e619b8720ef56fb0e857fb499f0abf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543698"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="657f8-103">ChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="657f8-103">ChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="657f8-104">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="657f8-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="657f8-105">方法</span><span class="sxs-lookup"><span data-stu-id="657f8-105">Methods</span></span>

| <span data-ttu-id="657f8-106">方法</span><span class="sxs-lookup"><span data-stu-id="657f8-106">Method</span></span>           | <span data-ttu-id="657f8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="657f8-107">Return Type</span></span>    |<span data-ttu-id="657f8-108">说明</span><span class="sxs-lookup"><span data-stu-id="657f8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="657f8-109">获取 ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="657f8-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="657f8-110">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="657f8-110">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="657f8-111">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="657f8-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="657f8-112">更新</span><span class="sxs-lookup"><span data-stu-id="657f8-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="657f8-113">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="657f8-113">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="657f8-114">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="657f8-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="657f8-115">属性</span><span class="sxs-lookup"><span data-stu-id="657f8-115">Properties</span></span>
| <span data-ttu-id="657f8-116">属性</span><span class="sxs-lookup"><span data-stu-id="657f8-116">Property</span></span>     | <span data-ttu-id="657f8-117">类型</span><span class="sxs-lookup"><span data-stu-id="657f8-117">Type</span></span>   |<span data-ttu-id="657f8-118">说明</span><span class="sxs-lookup"><span data-stu-id="657f8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="657f8-119">visible</span><span class="sxs-lookup"><span data-stu-id="657f8-119">visible</span></span>|<span data-ttu-id="657f8-120">布尔</span><span class="sxs-lookup"><span data-stu-id="657f8-120">boolean</span></span>|<span data-ttu-id="657f8-121">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="657f8-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="657f8-122">关系</span><span class="sxs-lookup"><span data-stu-id="657f8-122">Relationships</span></span>
| <span data-ttu-id="657f8-123">关系</span><span class="sxs-lookup"><span data-stu-id="657f8-123">Relationship</span></span> | <span data-ttu-id="657f8-124">类型</span><span class="sxs-lookup"><span data-stu-id="657f8-124">Type</span></span>   |<span data-ttu-id="657f8-125">说明</span><span class="sxs-lookup"><span data-stu-id="657f8-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="657f8-126">format</span><span class="sxs-lookup"><span data-stu-id="657f8-126">format</span></span>|[<span data-ttu-id="657f8-127">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="657f8-127">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="657f8-p101">表示图表网格线的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="657f8-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="657f8-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="657f8-130">JSON representation</span></span>

<span data-ttu-id="657f8-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="657f8-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
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
