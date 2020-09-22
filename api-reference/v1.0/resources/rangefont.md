---
title: RangeFont 资源类型
description: 此对象表示对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 95a58a62355c70b1f2588b83594ab5497ac3db49
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037071"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="905ed-103">RangeFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="905ed-103">RangeFont resource type</span></span>

<span data-ttu-id="905ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="905ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="905ed-105">此对象表示对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="905ed-105">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="905ed-106">方法</span><span class="sxs-lookup"><span data-stu-id="905ed-106">Methods</span></span>

| <span data-ttu-id="905ed-107">方法</span><span class="sxs-lookup"><span data-stu-id="905ed-107">Method</span></span>           | <span data-ttu-id="905ed-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="905ed-108">Return Type</span></span>    |<span data-ttu-id="905ed-109">说明</span><span class="sxs-lookup"><span data-stu-id="905ed-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="905ed-110">获取 RangeFont</span><span class="sxs-lookup"><span data-stu-id="905ed-110">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="905ed-111">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="905ed-111">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="905ed-112">读取 rangeFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="905ed-112">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="905ed-113">更新</span><span class="sxs-lookup"><span data-stu-id="905ed-113">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="905ed-114">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="905ed-114">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="905ed-115">更新 RangeFont 对象。</span><span class="sxs-lookup"><span data-stu-id="905ed-115">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="905ed-116">属性</span><span class="sxs-lookup"><span data-stu-id="905ed-116">Properties</span></span>
| <span data-ttu-id="905ed-117">属性</span><span class="sxs-lookup"><span data-stu-id="905ed-117">Property</span></span>     | <span data-ttu-id="905ed-118">类型</span><span class="sxs-lookup"><span data-stu-id="905ed-118">Type</span></span>   |<span data-ttu-id="905ed-119">说明</span><span class="sxs-lookup"><span data-stu-id="905ed-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="905ed-120">bold</span><span class="sxs-lookup"><span data-stu-id="905ed-120">bold</span></span>|<span data-ttu-id="905ed-121">布尔</span><span class="sxs-lookup"><span data-stu-id="905ed-121">boolean</span></span>|<span data-ttu-id="905ed-122">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="905ed-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="905ed-123">color</span><span class="sxs-lookup"><span data-stu-id="905ed-123">color</span></span>|<span data-ttu-id="905ed-124">string</span><span class="sxs-lookup"><span data-stu-id="905ed-124">string</span></span>|<span data-ttu-id="905ed-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="905ed-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="905ed-128">italic</span><span class="sxs-lookup"><span data-stu-id="905ed-128">italic</span></span>|<span data-ttu-id="905ed-129">布尔</span><span class="sxs-lookup"><span data-stu-id="905ed-129">boolean</span></span>|<span data-ttu-id="905ed-130">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="905ed-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="905ed-131">name</span><span class="sxs-lookup"><span data-stu-id="905ed-131">name</span></span>|<span data-ttu-id="905ed-132">string</span><span class="sxs-lookup"><span data-stu-id="905ed-132">string</span></span>|<span data-ttu-id="905ed-133">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="905ed-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="905ed-134">大小</span><span class="sxs-lookup"><span data-stu-id="905ed-134">size</span></span>|<span data-ttu-id="905ed-135">double</span><span class="sxs-lookup"><span data-stu-id="905ed-135">double</span></span>|<span data-ttu-id="905ed-136">字号</span><span class="sxs-lookup"><span data-stu-id="905ed-136">Font size.</span></span>|
|<span data-ttu-id="905ed-137">underline</span><span class="sxs-lookup"><span data-stu-id="905ed-137">underline</span></span>|<span data-ttu-id="905ed-138">string</span><span class="sxs-lookup"><span data-stu-id="905ed-138">string</span></span>|<span data-ttu-id="905ed-139">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="905ed-139">Type of underline applied to the font.</span></span> <span data-ttu-id="905ed-140">可能的值包括 `None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="905ed-140">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="905ed-141">关系</span><span class="sxs-lookup"><span data-stu-id="905ed-141">Relationships</span></span>
<span data-ttu-id="905ed-142">无</span><span class="sxs-lookup"><span data-stu-id="905ed-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="905ed-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="905ed-143">JSON representation</span></span>

<span data-ttu-id="905ed-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="905ed-144">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
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

