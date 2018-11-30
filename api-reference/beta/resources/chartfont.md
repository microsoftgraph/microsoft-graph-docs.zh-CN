---
title: ChartFont 资源类型
description: 此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。
ms.openlocfilehash: a0aa3150cb6ad31b4ad635253fd6ae35647b5ff7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045392"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="849a6-103">ChartFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="849a6-103">ChartFont resource type</span></span>

> <span data-ttu-id="849a6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="849a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="849a6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="849a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="849a6-106">此对象表示 chart 对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="849a6-106">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="849a6-107">方法</span><span class="sxs-lookup"><span data-stu-id="849a6-107">Methods</span></span>

| <span data-ttu-id="849a6-108">方法</span><span class="sxs-lookup"><span data-stu-id="849a6-108">Method</span></span>           | <span data-ttu-id="849a6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="849a6-109">Return Type</span></span>    |<span data-ttu-id="849a6-110">说明</span><span class="sxs-lookup"><span data-stu-id="849a6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="849a6-111">获取 ChartFont</span><span class="sxs-lookup"><span data-stu-id="849a6-111">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="849a6-112">ChartFont</span><span class="sxs-lookup"><span data-stu-id="849a6-112">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="849a6-113">读取 chartFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="849a6-113">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="849a6-114">Update</span><span class="sxs-lookup"><span data-stu-id="849a6-114">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="849a6-115">ChartFont</span><span class="sxs-lookup"><span data-stu-id="849a6-115">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="849a6-116">更新 ChartFont 对象。</span><span class="sxs-lookup"><span data-stu-id="849a6-116">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="849a6-117">属性</span><span class="sxs-lookup"><span data-stu-id="849a6-117">Properties</span></span>
| <span data-ttu-id="849a6-118">属性</span><span class="sxs-lookup"><span data-stu-id="849a6-118">Property</span></span>     | <span data-ttu-id="849a6-119">类型</span><span class="sxs-lookup"><span data-stu-id="849a6-119">Type</span></span>   |<span data-ttu-id="849a6-120">说明</span><span class="sxs-lookup"><span data-stu-id="849a6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="849a6-121">bold</span><span class="sxs-lookup"><span data-stu-id="849a6-121">bold</span></span>|<span data-ttu-id="849a6-122">boolean</span><span class="sxs-lookup"><span data-stu-id="849a6-122">boolean</span></span>|<span data-ttu-id="849a6-123">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="849a6-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="849a6-124">color</span><span class="sxs-lookup"><span data-stu-id="849a6-124">color</span></span>|<span data-ttu-id="849a6-125">string</span><span class="sxs-lookup"><span data-stu-id="849a6-125">string</span></span>|<span data-ttu-id="849a6-p102">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="849a6-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="849a6-129">italic</span><span class="sxs-lookup"><span data-stu-id="849a6-129">italic</span></span>|<span data-ttu-id="849a6-130">boolean</span><span class="sxs-lookup"><span data-stu-id="849a6-130">boolean</span></span>|<span data-ttu-id="849a6-131">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="849a6-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="849a6-132">name</span><span class="sxs-lookup"><span data-stu-id="849a6-132">name</span></span>|<span data-ttu-id="849a6-133">string</span><span class="sxs-lookup"><span data-stu-id="849a6-133">string</span></span>|<span data-ttu-id="849a6-134">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="849a6-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="849a6-135">大小</span><span class="sxs-lookup"><span data-stu-id="849a6-135">size</span></span>|<span data-ttu-id="849a6-136">double</span><span class="sxs-lookup"><span data-stu-id="849a6-136">double</span></span>|<span data-ttu-id="849a6-137">字体大小（例如 11）</span><span class="sxs-lookup"><span data-stu-id="849a6-137">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="849a6-138">underline</span><span class="sxs-lookup"><span data-stu-id="849a6-138">underline</span></span>|<span data-ttu-id="849a6-139">string</span><span class="sxs-lookup"><span data-stu-id="849a6-139">string</span></span>|<span data-ttu-id="849a6-p103">应用于字体的下划线类型。可能的值是：`None`、`Single`。</span><span class="sxs-lookup"><span data-stu-id="849a6-p103">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="849a6-142">Relationships</span><span class="sxs-lookup"><span data-stu-id="849a6-142">Relationships</span></span>
<span data-ttu-id="849a6-143">无</span><span class="sxs-lookup"><span data-stu-id="849a6-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="849a6-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="849a6-144">JSON representation</span></span>

<span data-ttu-id="849a6-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="849a6-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->