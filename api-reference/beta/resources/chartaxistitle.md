---
title: ChartAxisTitle 资源类型
description: 表示图表坐标轴的标题。
ms.openlocfilehash: 83d3712367b3c56b2fe30e7e1e464491b77fbee5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046672"
---
# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="bd1ab-103">ChartAxisTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd1ab-103">ChartAxisTitle resource type</span></span>

> <span data-ttu-id="bd1ab-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bd1ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd1ab-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bd1ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd1ab-106">表示图表坐标轴的标题。</span><span class="sxs-lookup"><span data-stu-id="bd1ab-106">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="bd1ab-107">方法</span><span class="sxs-lookup"><span data-stu-id="bd1ab-107">Methods</span></span>

| <span data-ttu-id="bd1ab-108">方法</span><span class="sxs-lookup"><span data-stu-id="bd1ab-108">Method</span></span>           | <span data-ttu-id="bd1ab-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bd1ab-109">Return Type</span></span>    |<span data-ttu-id="bd1ab-110">说明</span><span class="sxs-lookup"><span data-stu-id="bd1ab-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd1ab-111">获取 ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="bd1ab-111">Get ChartAxisTitle</span></span>](../api/chartaxistitle-get.md) | [<span data-ttu-id="bd1ab-112">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="bd1ab-112">ChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="bd1ab-113">读取 chartAxisTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bd1ab-113">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="bd1ab-114">Update</span><span class="sxs-lookup"><span data-stu-id="bd1ab-114">Update</span></span>](../api/chartaxistitle-update.md) | [<span data-ttu-id="bd1ab-115">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="bd1ab-115">ChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="bd1ab-116">更新 ChartAxisTitle 对象</span><span class="sxs-lookup"><span data-stu-id="bd1ab-116">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bd1ab-117">属性</span><span class="sxs-lookup"><span data-stu-id="bd1ab-117">Properties</span></span>
| <span data-ttu-id="bd1ab-118">属性</span><span class="sxs-lookup"><span data-stu-id="bd1ab-118">Property</span></span>     | <span data-ttu-id="bd1ab-119">类型</span><span class="sxs-lookup"><span data-stu-id="bd1ab-119">Type</span></span>   |<span data-ttu-id="bd1ab-120">说明</span><span class="sxs-lookup"><span data-stu-id="bd1ab-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd1ab-121">text</span><span class="sxs-lookup"><span data-stu-id="bd1ab-121">text</span></span>|<span data-ttu-id="bd1ab-122">string</span><span class="sxs-lookup"><span data-stu-id="bd1ab-122">string</span></span>|<span data-ttu-id="bd1ab-123">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="bd1ab-123">Represents the axis title.</span></span>|
|<span data-ttu-id="bd1ab-124">visible</span><span class="sxs-lookup"><span data-stu-id="bd1ab-124">visible</span></span>|<span data-ttu-id="bd1ab-125">boolean</span><span class="sxs-lookup"><span data-stu-id="bd1ab-125">boolean</span></span>|<span data-ttu-id="bd1ab-126">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="bd1ab-126">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd1ab-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="bd1ab-127">Relationships</span></span>
| <span data-ttu-id="bd1ab-128">关系</span><span class="sxs-lookup"><span data-stu-id="bd1ab-128">Relationship</span></span> | <span data-ttu-id="bd1ab-129">类型</span><span class="sxs-lookup"><span data-stu-id="bd1ab-129">Type</span></span>   |<span data-ttu-id="bd1ab-130">说明</span><span class="sxs-lookup"><span data-stu-id="bd1ab-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd1ab-131">format</span><span class="sxs-lookup"><span data-stu-id="bd1ab-131">format</span></span>|[<span data-ttu-id="bd1ab-132">ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="bd1ab-132">ChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="bd1ab-p102">表示图表坐标轴标题的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="bd1ab-p102">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd1ab-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd1ab-135">JSON representation</span></span>

<span data-ttu-id="bd1ab-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd1ab-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->