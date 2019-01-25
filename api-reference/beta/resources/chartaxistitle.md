---
title: ChartAxisTitle 资源类型
description: 表示图表坐标轴的标题。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 25a5daf571f7533bd1682974adecad1cfd984894
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513121"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="be82a-103">ChartAxisTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="be82a-103">ChartAxisTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be82a-104">表示图表坐标轴的标题。</span><span class="sxs-lookup"><span data-stu-id="be82a-104">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="be82a-105">方法</span><span class="sxs-lookup"><span data-stu-id="be82a-105">Methods</span></span>

| <span data-ttu-id="be82a-106">方法</span><span class="sxs-lookup"><span data-stu-id="be82a-106">Method</span></span>           | <span data-ttu-id="be82a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="be82a-107">Return Type</span></span>    |<span data-ttu-id="be82a-108">说明</span><span class="sxs-lookup"><span data-stu-id="be82a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be82a-109">获取 ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="be82a-109">[Get ChartAxisTitle](../api/chartaxistitle-get.md)</span></span> | [<span data-ttu-id="be82a-110">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="be82a-110">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="be82a-111">读取 chartAxisTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="be82a-111">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="be82a-112">Update</span><span class="sxs-lookup"><span data-stu-id="be82a-112">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="be82a-113">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="be82a-113">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="be82a-114">更新 ChartAxisTitle 对象</span><span class="sxs-lookup"><span data-stu-id="be82a-114">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="be82a-115">属性</span><span class="sxs-lookup"><span data-stu-id="be82a-115">Properties</span></span>
| <span data-ttu-id="be82a-116">属性</span><span class="sxs-lookup"><span data-stu-id="be82a-116">Property</span></span>     | <span data-ttu-id="be82a-117">类型</span><span class="sxs-lookup"><span data-stu-id="be82a-117">Type</span></span>   |<span data-ttu-id="be82a-118">说明</span><span class="sxs-lookup"><span data-stu-id="be82a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be82a-119">text</span><span class="sxs-lookup"><span data-stu-id="be82a-119">text</span></span>|<span data-ttu-id="be82a-120">string</span><span class="sxs-lookup"><span data-stu-id="be82a-120">string</span></span>|<span data-ttu-id="be82a-121">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="be82a-121">Represents the axis title.</span></span>|
|<span data-ttu-id="be82a-122">visible</span><span class="sxs-lookup"><span data-stu-id="be82a-122">visible</span></span>|<span data-ttu-id="be82a-123">布尔</span><span class="sxs-lookup"><span data-stu-id="be82a-123">boolean</span></span>|<span data-ttu-id="be82a-124">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="be82a-124">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be82a-125">关系</span><span class="sxs-lookup"><span data-stu-id="be82a-125">Relationships</span></span>
| <span data-ttu-id="be82a-126">关系</span><span class="sxs-lookup"><span data-stu-id="be82a-126">Relationship</span></span> | <span data-ttu-id="be82a-127">类型</span><span class="sxs-lookup"><span data-stu-id="be82a-127">Type</span></span>   |<span data-ttu-id="be82a-128">说明</span><span class="sxs-lookup"><span data-stu-id="be82a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be82a-129">format</span><span class="sxs-lookup"><span data-stu-id="be82a-129">format</span></span>|[<span data-ttu-id="be82a-130">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="be82a-130">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="be82a-p101">表示图表坐标轴标题的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="be82a-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be82a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be82a-133">JSON representation</span></span>

<span data-ttu-id="be82a-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be82a-134">Here is a JSON representation of the resource.</span></span>

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
