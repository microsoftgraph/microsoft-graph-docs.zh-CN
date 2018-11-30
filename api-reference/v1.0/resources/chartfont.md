---
title: ChartFont 资源类型
description: 此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。
ms.openlocfilehash: dc4b1f8cd0653d89c3486a61604dd09c0e23cb2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008780"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="3f087-103">ChartFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f087-103">ChartFont resource type</span></span>

<span data-ttu-id="3f087-104">此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="3f087-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="3f087-105">方法</span><span class="sxs-lookup"><span data-stu-id="3f087-105">Methods</span></span>

| <span data-ttu-id="3f087-106">方法</span><span class="sxs-lookup"><span data-stu-id="3f087-106">Method</span></span>           | <span data-ttu-id="3f087-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f087-107">Return Type</span></span>    |<span data-ttu-id="3f087-108">说明</span><span class="sxs-lookup"><span data-stu-id="3f087-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f087-109">获取 ChartFont</span><span class="sxs-lookup"><span data-stu-id="3f087-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="3f087-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="3f087-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="3f087-111">读取 chartFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f087-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="3f087-112">Update</span><span class="sxs-lookup"><span data-stu-id="3f087-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="3f087-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="3f087-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="3f087-114">更新 ChartFont 对象。</span><span class="sxs-lookup"><span data-stu-id="3f087-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3f087-115">属性</span><span class="sxs-lookup"><span data-stu-id="3f087-115">Properties</span></span>
| <span data-ttu-id="3f087-116">属性</span><span class="sxs-lookup"><span data-stu-id="3f087-116">Property</span></span>     | <span data-ttu-id="3f087-117">类型</span><span class="sxs-lookup"><span data-stu-id="3f087-117">Type</span></span>   |<span data-ttu-id="3f087-118">说明</span><span class="sxs-lookup"><span data-stu-id="3f087-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f087-119">bold</span><span class="sxs-lookup"><span data-stu-id="3f087-119">bold</span></span>|<span data-ttu-id="3f087-120">boolean</span><span class="sxs-lookup"><span data-stu-id="3f087-120">boolean</span></span>|<span data-ttu-id="3f087-121">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="3f087-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="3f087-122">color</span><span class="sxs-lookup"><span data-stu-id="3f087-122">color</span></span>|<span data-ttu-id="3f087-123">string</span><span class="sxs-lookup"><span data-stu-id="3f087-123">string</span></span>|<span data-ttu-id="3f087-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="3f087-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="3f087-127">italic</span><span class="sxs-lookup"><span data-stu-id="3f087-127">italic</span></span>|<span data-ttu-id="3f087-128">boolean</span><span class="sxs-lookup"><span data-stu-id="3f087-128">boolean</span></span>|<span data-ttu-id="3f087-129">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="3f087-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="3f087-130">name</span><span class="sxs-lookup"><span data-stu-id="3f087-130">name</span></span>|<span data-ttu-id="3f087-131">string</span><span class="sxs-lookup"><span data-stu-id="3f087-131">string</span></span>|<span data-ttu-id="3f087-132">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="3f087-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="3f087-133">大小</span><span class="sxs-lookup"><span data-stu-id="3f087-133">size</span></span>|<span data-ttu-id="3f087-134">double</span><span class="sxs-lookup"><span data-stu-id="3f087-134">double</span></span>|<span data-ttu-id="3f087-135">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="3f087-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="3f087-136">underline</span><span class="sxs-lookup"><span data-stu-id="3f087-136">underline</span></span>|<span data-ttu-id="3f087-137">string</span><span class="sxs-lookup"><span data-stu-id="3f087-137">string</span></span>|<span data-ttu-id="3f087-138">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="3f087-138">Type of underline applied to the font.</span></span> <span data-ttu-id="3f087-139">可能的值为： `None`， `Single`。</span><span class="sxs-lookup"><span data-stu-id="3f087-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f087-140">Relationships</span><span class="sxs-lookup"><span data-stu-id="3f087-140">Relationships</span></span>
<span data-ttu-id="3f087-141">无</span><span class="sxs-lookup"><span data-stu-id="3f087-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3f087-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f087-142">JSON representation</span></span>

<span data-ttu-id="3f087-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f087-143">Here is a JSON representation of the resource.</span></span>

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