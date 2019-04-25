---
title: RangeFont 资源类型
description: 此对象表示对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 829b391d561aae63ae94972c55039acfdf4c48d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579520"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="674b5-103">RangeFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="674b5-103">RangeFont resource type</span></span>

<span data-ttu-id="674b5-104">此对象表示对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="674b5-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="674b5-105">方法</span><span class="sxs-lookup"><span data-stu-id="674b5-105">Methods</span></span>

| <span data-ttu-id="674b5-106">方法</span><span class="sxs-lookup"><span data-stu-id="674b5-106">Method</span></span>           | <span data-ttu-id="674b5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="674b5-107">Return Type</span></span>    |<span data-ttu-id="674b5-108">说明</span><span class="sxs-lookup"><span data-stu-id="674b5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="674b5-109">获取 RangeFont</span><span class="sxs-lookup"><span data-stu-id="674b5-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="674b5-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="674b5-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="674b5-111">读取 rangeFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="674b5-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="674b5-112">更新</span><span class="sxs-lookup"><span data-stu-id="674b5-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="674b5-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="674b5-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="674b5-114">更新 RangeFont 对象。</span><span class="sxs-lookup"><span data-stu-id="674b5-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="674b5-115">属性</span><span class="sxs-lookup"><span data-stu-id="674b5-115">Properties</span></span>
| <span data-ttu-id="674b5-116">属性</span><span class="sxs-lookup"><span data-stu-id="674b5-116">Property</span></span>     | <span data-ttu-id="674b5-117">类型</span><span class="sxs-lookup"><span data-stu-id="674b5-117">Type</span></span>   |<span data-ttu-id="674b5-118">说明</span><span class="sxs-lookup"><span data-stu-id="674b5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="674b5-119">bold</span><span class="sxs-lookup"><span data-stu-id="674b5-119">bold</span></span>|<span data-ttu-id="674b5-120">布尔</span><span class="sxs-lookup"><span data-stu-id="674b5-120">boolean</span></span>|<span data-ttu-id="674b5-121">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="674b5-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="674b5-122">color</span><span class="sxs-lookup"><span data-stu-id="674b5-122">color</span></span>|<span data-ttu-id="674b5-123">string</span><span class="sxs-lookup"><span data-stu-id="674b5-123">string</span></span>|<span data-ttu-id="674b5-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="674b5-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="674b5-127">italic</span><span class="sxs-lookup"><span data-stu-id="674b5-127">italic</span></span>|<span data-ttu-id="674b5-128">布尔</span><span class="sxs-lookup"><span data-stu-id="674b5-128">boolean</span></span>|<span data-ttu-id="674b5-129">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="674b5-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="674b5-130">name</span><span class="sxs-lookup"><span data-stu-id="674b5-130">name</span></span>|<span data-ttu-id="674b5-131">string</span><span class="sxs-lookup"><span data-stu-id="674b5-131">string</span></span>|<span data-ttu-id="674b5-132">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="674b5-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="674b5-133">大小</span><span class="sxs-lookup"><span data-stu-id="674b5-133">size</span></span>|<span data-ttu-id="674b5-134">double</span><span class="sxs-lookup"><span data-stu-id="674b5-134">double</span></span>|<span data-ttu-id="674b5-135">字号</span><span class="sxs-lookup"><span data-stu-id="674b5-135">Font size.</span></span>|
|<span data-ttu-id="674b5-136">underline</span><span class="sxs-lookup"><span data-stu-id="674b5-136">underline</span></span>|<span data-ttu-id="674b5-137">string</span><span class="sxs-lookup"><span data-stu-id="674b5-137">string</span></span>|<span data-ttu-id="674b5-138">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="674b5-138">Type of underline applied to the font.</span></span> <span data-ttu-id="674b5-139">可能的值包括 `None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="674b5-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="674b5-140">关系</span><span class="sxs-lookup"><span data-stu-id="674b5-140">Relationships</span></span>
<span data-ttu-id="674b5-141">无</span><span class="sxs-lookup"><span data-stu-id="674b5-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="674b5-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="674b5-142">JSON representation</span></span>

<span data-ttu-id="674b5-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="674b5-143">Here is a JSON representation of the resource.</span></span>

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
