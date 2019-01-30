---
title: ChartFont 资源类型
description: 此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c507a966dc6b29e46935c5c77a85b557a84cc69c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641167"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="c61a1-103">ChartFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="c61a1-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c61a1-104">此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="c61a1-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="c61a1-105">方法</span><span class="sxs-lookup"><span data-stu-id="c61a1-105">Methods</span></span>

| <span data-ttu-id="c61a1-106">方法</span><span class="sxs-lookup"><span data-stu-id="c61a1-106">Method</span></span>           | <span data-ttu-id="c61a1-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c61a1-107">Return Type</span></span>    |<span data-ttu-id="c61a1-108">说明</span><span class="sxs-lookup"><span data-stu-id="c61a1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c61a1-109">获取 ChartFont</span><span class="sxs-lookup"><span data-stu-id="c61a1-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="c61a1-110">ChartFont</span><span class="sxs-lookup"><span data-stu-id="c61a1-110">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="c61a1-111">读取 chartFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c61a1-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="c61a1-112">更新</span><span class="sxs-lookup"><span data-stu-id="c61a1-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="c61a1-113">ChartFont</span><span class="sxs-lookup"><span data-stu-id="c61a1-113">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="c61a1-114">更新 ChartFont 对象。</span><span class="sxs-lookup"><span data-stu-id="c61a1-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c61a1-115">属性</span><span class="sxs-lookup"><span data-stu-id="c61a1-115">Properties</span></span>
| <span data-ttu-id="c61a1-116">属性</span><span class="sxs-lookup"><span data-stu-id="c61a1-116">Property</span></span>     | <span data-ttu-id="c61a1-117">类型</span><span class="sxs-lookup"><span data-stu-id="c61a1-117">Type</span></span>   |<span data-ttu-id="c61a1-118">说明</span><span class="sxs-lookup"><span data-stu-id="c61a1-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c61a1-119">bold</span><span class="sxs-lookup"><span data-stu-id="c61a1-119">bold</span></span>|<span data-ttu-id="c61a1-120">boolean</span><span class="sxs-lookup"><span data-stu-id="c61a1-120">boolean</span></span>|<span data-ttu-id="c61a1-121">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="c61a1-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="c61a1-122">color</span><span class="sxs-lookup"><span data-stu-id="c61a1-122">color</span></span>|<span data-ttu-id="c61a1-123">string</span><span class="sxs-lookup"><span data-stu-id="c61a1-123">string</span></span>|<span data-ttu-id="c61a1-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="c61a1-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="c61a1-127">italic</span><span class="sxs-lookup"><span data-stu-id="c61a1-127">italic</span></span>|<span data-ttu-id="c61a1-128">boolean</span><span class="sxs-lookup"><span data-stu-id="c61a1-128">boolean</span></span>|<span data-ttu-id="c61a1-129">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="c61a1-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="c61a1-130">name</span><span class="sxs-lookup"><span data-stu-id="c61a1-130">name</span></span>|<span data-ttu-id="c61a1-131">string</span><span class="sxs-lookup"><span data-stu-id="c61a1-131">string</span></span>|<span data-ttu-id="c61a1-132">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="c61a1-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="c61a1-133">大小</span><span class="sxs-lookup"><span data-stu-id="c61a1-133">size</span></span>|<span data-ttu-id="c61a1-134">double</span><span class="sxs-lookup"><span data-stu-id="c61a1-134">double</span></span>|<span data-ttu-id="c61a1-135">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="c61a1-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="c61a1-136">underline</span><span class="sxs-lookup"><span data-stu-id="c61a1-136">underline</span></span>|<span data-ttu-id="c61a1-137">string</span><span class="sxs-lookup"><span data-stu-id="c61a1-137">string</span></span>|<span data-ttu-id="c61a1-p102">应用于字体的下划线类型。可能的值是：`None`、`Single`。</span><span class="sxs-lookup"><span data-stu-id="c61a1-p102">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c61a1-140">关系</span><span class="sxs-lookup"><span data-stu-id="c61a1-140">Relationships</span></span>
<span data-ttu-id="c61a1-141">无</span><span class="sxs-lookup"><span data-stu-id="c61a1-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c61a1-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c61a1-142">JSON representation</span></span>

<span data-ttu-id="c61a1-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c61a1-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartfont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
