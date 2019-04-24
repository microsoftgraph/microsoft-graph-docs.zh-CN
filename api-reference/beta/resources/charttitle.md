---
title: ChartTitle 资源类型
description: 表示图表的图表标题对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a71aed2da93c2121492f1eb29826470b797768ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460987"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="516cc-103">ChartTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="516cc-103">ChartTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="516cc-104">表示图表的图表标题对象。</span><span class="sxs-lookup"><span data-stu-id="516cc-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="516cc-105">方法</span><span class="sxs-lookup"><span data-stu-id="516cc-105">Methods</span></span>

| <span data-ttu-id="516cc-106">方法</span><span class="sxs-lookup"><span data-stu-id="516cc-106">Method</span></span>           | <span data-ttu-id="516cc-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="516cc-107">Return Type</span></span>    |<span data-ttu-id="516cc-108">说明</span><span class="sxs-lookup"><span data-stu-id="516cc-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="516cc-109">获取 ChartTitle</span><span class="sxs-lookup"><span data-stu-id="516cc-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="516cc-110">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="516cc-110">ChartTitle</span></span>](charttitle.md) |<span data-ttu-id="516cc-111">读取 chartTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="516cc-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="516cc-112">更新</span><span class="sxs-lookup"><span data-stu-id="516cc-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="516cc-113">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="516cc-113">ChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="516cc-114">更新 ChartTitle 对象。</span><span class="sxs-lookup"><span data-stu-id="516cc-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="516cc-115">属性</span><span class="sxs-lookup"><span data-stu-id="516cc-115">Properties</span></span>
| <span data-ttu-id="516cc-116">属性</span><span class="sxs-lookup"><span data-stu-id="516cc-116">Property</span></span>     | <span data-ttu-id="516cc-117">类型</span><span class="sxs-lookup"><span data-stu-id="516cc-117">Type</span></span>   |<span data-ttu-id="516cc-118">说明</span><span class="sxs-lookup"><span data-stu-id="516cc-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="516cc-119">overlay</span><span class="sxs-lookup"><span data-stu-id="516cc-119">overlay</span></span>|<span data-ttu-id="516cc-120">布尔</span><span class="sxs-lookup"><span data-stu-id="516cc-120">boolean</span></span>|<span data-ttu-id="516cc-121">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="516cc-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="516cc-122">text</span><span class="sxs-lookup"><span data-stu-id="516cc-122">text</span></span>|<span data-ttu-id="516cc-123">string</span><span class="sxs-lookup"><span data-stu-id="516cc-123">string</span></span>|<span data-ttu-id="516cc-124">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="516cc-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="516cc-125">visible</span><span class="sxs-lookup"><span data-stu-id="516cc-125">visible</span></span>|<span data-ttu-id="516cc-126">布尔</span><span class="sxs-lookup"><span data-stu-id="516cc-126">boolean</span></span>|<span data-ttu-id="516cc-127">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="516cc-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="516cc-128">关系</span><span class="sxs-lookup"><span data-stu-id="516cc-128">Relationships</span></span>
| <span data-ttu-id="516cc-129">关系</span><span class="sxs-lookup"><span data-stu-id="516cc-129">Relationship</span></span> | <span data-ttu-id="516cc-130">类型</span><span class="sxs-lookup"><span data-stu-id="516cc-130">Type</span></span>   |<span data-ttu-id="516cc-131">说明</span><span class="sxs-lookup"><span data-stu-id="516cc-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="516cc-132">format</span><span class="sxs-lookup"><span data-stu-id="516cc-132">format</span></span>|[<span data-ttu-id="516cc-133">ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="516cc-133">ChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="516cc-p101">表示图表标题的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="516cc-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="516cc-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="516cc-136">JSON representation</span></span>

<span data-ttu-id="516cc-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="516cc-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartTitle"
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
