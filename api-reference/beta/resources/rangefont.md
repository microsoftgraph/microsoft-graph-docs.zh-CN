---
title: RangeFont 资源类型
description: 此对象表示对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: e6f448df142ffdc0c20e39045b4cd77a6c224a6f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912776"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="29bd3-103">RangeFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="29bd3-103">RangeFont resource type</span></span>

> <span data-ttu-id="29bd3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="29bd3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29bd3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="29bd3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29bd3-106">此对象表示对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="29bd3-106">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="29bd3-107">方法</span><span class="sxs-lookup"><span data-stu-id="29bd3-107">Methods</span></span>

| <span data-ttu-id="29bd3-108">方法</span><span class="sxs-lookup"><span data-stu-id="29bd3-108">Method</span></span>           | <span data-ttu-id="29bd3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="29bd3-109">Return Type</span></span>    |<span data-ttu-id="29bd3-110">说明</span><span class="sxs-lookup"><span data-stu-id="29bd3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29bd3-111">获取 RangeFont</span><span class="sxs-lookup"><span data-stu-id="29bd3-111">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="29bd3-112">RangeFont</span><span class="sxs-lookup"><span data-stu-id="29bd3-112">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="29bd3-113">读取 rangeFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29bd3-113">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="29bd3-114">Update</span><span class="sxs-lookup"><span data-stu-id="29bd3-114">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="29bd3-115">RangeFont</span><span class="sxs-lookup"><span data-stu-id="29bd3-115">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="29bd3-116">更新 RangeFont 对象。</span><span class="sxs-lookup"><span data-stu-id="29bd3-116">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="29bd3-117">属性</span><span class="sxs-lookup"><span data-stu-id="29bd3-117">Properties</span></span>
| <span data-ttu-id="29bd3-118">属性</span><span class="sxs-lookup"><span data-stu-id="29bd3-118">Property</span></span>     | <span data-ttu-id="29bd3-119">类型</span><span class="sxs-lookup"><span data-stu-id="29bd3-119">Type</span></span>   |<span data-ttu-id="29bd3-120">说明</span><span class="sxs-lookup"><span data-stu-id="29bd3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29bd3-121">bold</span><span class="sxs-lookup"><span data-stu-id="29bd3-121">bold</span></span>|<span data-ttu-id="29bd3-122">boolean</span><span class="sxs-lookup"><span data-stu-id="29bd3-122">boolean</span></span>|<span data-ttu-id="29bd3-123">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="29bd3-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="29bd3-124">color</span><span class="sxs-lookup"><span data-stu-id="29bd3-124">color</span></span>|<span data-ttu-id="29bd3-125">string</span><span class="sxs-lookup"><span data-stu-id="29bd3-125">string</span></span>|<span data-ttu-id="29bd3-p102">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="29bd3-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="29bd3-129">italic</span><span class="sxs-lookup"><span data-stu-id="29bd3-129">italic</span></span>|<span data-ttu-id="29bd3-130">boolean</span><span class="sxs-lookup"><span data-stu-id="29bd3-130">boolean</span></span>|<span data-ttu-id="29bd3-131">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="29bd3-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="29bd3-132">name</span><span class="sxs-lookup"><span data-stu-id="29bd3-132">name</span></span>|<span data-ttu-id="29bd3-133">string</span><span class="sxs-lookup"><span data-stu-id="29bd3-133">string</span></span>|<span data-ttu-id="29bd3-134">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="29bd3-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="29bd3-135">大小</span><span class="sxs-lookup"><span data-stu-id="29bd3-135">size</span></span>|<span data-ttu-id="29bd3-136">double</span><span class="sxs-lookup"><span data-stu-id="29bd3-136">double</span></span>|<span data-ttu-id="29bd3-137">字号</span><span class="sxs-lookup"><span data-stu-id="29bd3-137">Font size.</span></span>|
|<span data-ttu-id="29bd3-138">underline</span><span class="sxs-lookup"><span data-stu-id="29bd3-138">underline</span></span>|<span data-ttu-id="29bd3-139">string</span><span class="sxs-lookup"><span data-stu-id="29bd3-139">string</span></span>|<span data-ttu-id="29bd3-p103">应用于字体的下划线类型。可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="29bd3-p103">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29bd3-142">Relationships</span><span class="sxs-lookup"><span data-stu-id="29bd3-142">Relationships</span></span>
<span data-ttu-id="29bd3-143">无</span><span class="sxs-lookup"><span data-stu-id="29bd3-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="29bd3-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29bd3-144">JSON representation</span></span>

<span data-ttu-id="29bd3-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29bd3-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
