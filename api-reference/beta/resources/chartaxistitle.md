---
title: ChartAxisTitle 资源类型
description: 表示图表坐标轴的标题。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 25a5daf571f7533bd1682974adecad1cfd984894
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644082"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="30cc7-103">ChartAxisTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="30cc7-103">ChartAxisTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30cc7-104">表示图表坐标轴的标题。</span><span class="sxs-lookup"><span data-stu-id="30cc7-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="30cc7-105">方法</span><span class="sxs-lookup"><span data-stu-id="30cc7-105">Methods</span></span>

| <span data-ttu-id="30cc7-106">方法</span><span class="sxs-lookup"><span data-stu-id="30cc7-106">Method</span></span>           | <span data-ttu-id="30cc7-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="30cc7-107">Return Type</span></span>    |<span data-ttu-id="30cc7-108">说明</span><span class="sxs-lookup"><span data-stu-id="30cc7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30cc7-109">获取 ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="30cc7-109">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="30cc7-110">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="30cc7-110">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="30cc7-111">读取 chartAxisTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30cc7-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="30cc7-112">更新</span><span class="sxs-lookup"><span data-stu-id="30cc7-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="30cc7-113">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="30cc7-113">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="30cc7-114">更新 ChartAxisTitle 对象</span><span class="sxs-lookup"><span data-stu-id="30cc7-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="30cc7-115">属性</span><span class="sxs-lookup"><span data-stu-id="30cc7-115">Properties</span></span>
| <span data-ttu-id="30cc7-116">属性</span><span class="sxs-lookup"><span data-stu-id="30cc7-116">Property</span></span>     | <span data-ttu-id="30cc7-117">类型</span><span class="sxs-lookup"><span data-stu-id="30cc7-117">Type</span></span>   |<span data-ttu-id="30cc7-118">说明</span><span class="sxs-lookup"><span data-stu-id="30cc7-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30cc7-119">text</span><span class="sxs-lookup"><span data-stu-id="30cc7-119">text</span></span>|<span data-ttu-id="30cc7-120">string</span><span class="sxs-lookup"><span data-stu-id="30cc7-120">string</span></span>|<span data-ttu-id="30cc7-121">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="30cc7-121">Represents the axis title.</span></span>|
|<span data-ttu-id="30cc7-122">visible</span><span class="sxs-lookup"><span data-stu-id="30cc7-122">visible</span></span>|<span data-ttu-id="30cc7-123">boolean</span><span class="sxs-lookup"><span data-stu-id="30cc7-123">boolean</span></span>|<span data-ttu-id="30cc7-124">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="30cc7-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30cc7-125">关系</span><span class="sxs-lookup"><span data-stu-id="30cc7-125">Relationships</span></span>
| <span data-ttu-id="30cc7-126">关系</span><span class="sxs-lookup"><span data-stu-id="30cc7-126">Relationship</span></span> | <span data-ttu-id="30cc7-127">类型</span><span class="sxs-lookup"><span data-stu-id="30cc7-127">Type</span></span>   |<span data-ttu-id="30cc7-128">说明</span><span class="sxs-lookup"><span data-stu-id="30cc7-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30cc7-129">format</span><span class="sxs-lookup"><span data-stu-id="30cc7-129">format</span></span>|[<span data-ttu-id="30cc7-130">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="30cc7-130">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="30cc7-p101">表示图表坐标轴标题的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="30cc7-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30cc7-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30cc7-133">JSON representation</span></span>

<span data-ttu-id="30cc7-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30cc7-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxistitle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
