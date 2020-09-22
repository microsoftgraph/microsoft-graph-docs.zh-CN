---
title: ChartFont 资源类型
description: 此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3862a6273e9dfca4df6bb412afcc061b057e617c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069195"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="8e52c-103">ChartFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e52c-103">ChartFont resource type</span></span>

<span data-ttu-id="8e52c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e52c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e52c-105">此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="8e52c-105">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="8e52c-106">方法</span><span class="sxs-lookup"><span data-stu-id="8e52c-106">Methods</span></span>

| <span data-ttu-id="8e52c-107">方法</span><span class="sxs-lookup"><span data-stu-id="8e52c-107">Method</span></span>           | <span data-ttu-id="8e52c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8e52c-108">Return Type</span></span>    |<span data-ttu-id="8e52c-109">说明</span><span class="sxs-lookup"><span data-stu-id="8e52c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e52c-110">获取 ChartFont</span><span class="sxs-lookup"><span data-stu-id="8e52c-110">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="8e52c-111">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="8e52c-111">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="8e52c-112">读取 chartFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8e52c-112">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="8e52c-113">更新</span><span class="sxs-lookup"><span data-stu-id="8e52c-113">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="8e52c-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="8e52c-114">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="8e52c-115">更新 ChartFont 对象。</span><span class="sxs-lookup"><span data-stu-id="8e52c-115">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e52c-116">属性</span><span class="sxs-lookup"><span data-stu-id="8e52c-116">Properties</span></span>
| <span data-ttu-id="8e52c-117">属性</span><span class="sxs-lookup"><span data-stu-id="8e52c-117">Property</span></span>     | <span data-ttu-id="8e52c-118">类型</span><span class="sxs-lookup"><span data-stu-id="8e52c-118">Type</span></span>   |<span data-ttu-id="8e52c-119">说明</span><span class="sxs-lookup"><span data-stu-id="8e52c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e52c-120">bold</span><span class="sxs-lookup"><span data-stu-id="8e52c-120">bold</span></span>|<span data-ttu-id="8e52c-121">布尔</span><span class="sxs-lookup"><span data-stu-id="8e52c-121">boolean</span></span>|<span data-ttu-id="8e52c-122">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="8e52c-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="8e52c-123">color</span><span class="sxs-lookup"><span data-stu-id="8e52c-123">color</span></span>|<span data-ttu-id="8e52c-124">string</span><span class="sxs-lookup"><span data-stu-id="8e52c-124">string</span></span>|<span data-ttu-id="8e52c-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="8e52c-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="8e52c-128">italic</span><span class="sxs-lookup"><span data-stu-id="8e52c-128">italic</span></span>|<span data-ttu-id="8e52c-129">布尔</span><span class="sxs-lookup"><span data-stu-id="8e52c-129">boolean</span></span>|<span data-ttu-id="8e52c-130">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="8e52c-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="8e52c-131">name</span><span class="sxs-lookup"><span data-stu-id="8e52c-131">name</span></span>|<span data-ttu-id="8e52c-132">string</span><span class="sxs-lookup"><span data-stu-id="8e52c-132">string</span></span>|<span data-ttu-id="8e52c-133">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="8e52c-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="8e52c-134">大小</span><span class="sxs-lookup"><span data-stu-id="8e52c-134">size</span></span>|<span data-ttu-id="8e52c-135">double</span><span class="sxs-lookup"><span data-stu-id="8e52c-135">double</span></span>|<span data-ttu-id="8e52c-136">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="8e52c-136">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="8e52c-137">underline</span><span class="sxs-lookup"><span data-stu-id="8e52c-137">underline</span></span>|<span data-ttu-id="8e52c-138">string</span><span class="sxs-lookup"><span data-stu-id="8e52c-138">string</span></span>|<span data-ttu-id="8e52c-139">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="8e52c-139">Type of underline applied to the font.</span></span> <span data-ttu-id="8e52c-140">可能的值为： `None` 、 `Single` 。</span><span class="sxs-lookup"><span data-stu-id="8e52c-140">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e52c-141">关系</span><span class="sxs-lookup"><span data-stu-id="8e52c-141">Relationships</span></span>
<span data-ttu-id="8e52c-142">无</span><span class="sxs-lookup"><span data-stu-id="8e52c-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8e52c-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e52c-143">JSON representation</span></span>

<span data-ttu-id="8e52c-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e52c-144">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

