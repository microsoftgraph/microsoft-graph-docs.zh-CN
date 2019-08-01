---
title: ChartFont 资源类型
description: 此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9241691296b93eb21e19e10b81f36e692fea0692
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032995"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="282ce-103">ChartFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="282ce-103">ChartFont resource type</span></span>

<span data-ttu-id="282ce-104">此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="282ce-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="282ce-105">方法</span><span class="sxs-lookup"><span data-stu-id="282ce-105">Methods</span></span>

| <span data-ttu-id="282ce-106">方法</span><span class="sxs-lookup"><span data-stu-id="282ce-106">Method</span></span>           | <span data-ttu-id="282ce-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="282ce-107">Return Type</span></span>    |<span data-ttu-id="282ce-108">说明</span><span class="sxs-lookup"><span data-stu-id="282ce-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="282ce-109">获取 ChartFont</span><span class="sxs-lookup"><span data-stu-id="282ce-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="282ce-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="282ce-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="282ce-111">读取 chartFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="282ce-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="282ce-112">更新</span><span class="sxs-lookup"><span data-stu-id="282ce-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="282ce-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="282ce-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="282ce-114">更新 ChartFont 对象。</span><span class="sxs-lookup"><span data-stu-id="282ce-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="282ce-115">属性</span><span class="sxs-lookup"><span data-stu-id="282ce-115">Properties</span></span>
| <span data-ttu-id="282ce-116">属性</span><span class="sxs-lookup"><span data-stu-id="282ce-116">Property</span></span>     | <span data-ttu-id="282ce-117">类型</span><span class="sxs-lookup"><span data-stu-id="282ce-117">Type</span></span>   |<span data-ttu-id="282ce-118">说明</span><span class="sxs-lookup"><span data-stu-id="282ce-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="282ce-119">bold</span><span class="sxs-lookup"><span data-stu-id="282ce-119">bold</span></span>|<span data-ttu-id="282ce-120">boolean</span><span class="sxs-lookup"><span data-stu-id="282ce-120">boolean</span></span>|<span data-ttu-id="282ce-121">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="282ce-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="282ce-122">color</span><span class="sxs-lookup"><span data-stu-id="282ce-122">color</span></span>|<span data-ttu-id="282ce-123">string</span><span class="sxs-lookup"><span data-stu-id="282ce-123">string</span></span>|<span data-ttu-id="282ce-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="282ce-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="282ce-127">italic</span><span class="sxs-lookup"><span data-stu-id="282ce-127">italic</span></span>|<span data-ttu-id="282ce-128">布尔</span><span class="sxs-lookup"><span data-stu-id="282ce-128">boolean</span></span>|<span data-ttu-id="282ce-129">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="282ce-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="282ce-130">name</span><span class="sxs-lookup"><span data-stu-id="282ce-130">name</span></span>|<span data-ttu-id="282ce-131">string</span><span class="sxs-lookup"><span data-stu-id="282ce-131">string</span></span>|<span data-ttu-id="282ce-132">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="282ce-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="282ce-133">大小</span><span class="sxs-lookup"><span data-stu-id="282ce-133">size</span></span>|<span data-ttu-id="282ce-134">double</span><span class="sxs-lookup"><span data-stu-id="282ce-134">double</span></span>|<span data-ttu-id="282ce-135">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="282ce-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="282ce-136">underline</span><span class="sxs-lookup"><span data-stu-id="282ce-136">underline</span></span>|<span data-ttu-id="282ce-137">string</span><span class="sxs-lookup"><span data-stu-id="282ce-137">string</span></span>|<span data-ttu-id="282ce-138">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="282ce-138">Type of underline applied to the font.</span></span> <span data-ttu-id="282ce-139">可能的值为: `None`、 `Single`。</span><span class="sxs-lookup"><span data-stu-id="282ce-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="282ce-140">关系</span><span class="sxs-lookup"><span data-stu-id="282ce-140">Relationships</span></span>
<span data-ttu-id="282ce-141">无</span><span class="sxs-lookup"><span data-stu-id="282ce-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="282ce-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="282ce-142">JSON representation</span></span>

<span data-ttu-id="282ce-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="282ce-143">Here is a JSON representation of the resource.</span></span>

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
