---
title: workbookRangeFont 资源类型
description: 此对象表示对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b3982a8026cd720fe614b11405a37bed8626042d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964037"
---
# <a name="workbookrangefont-resource-type"></a><span data-ttu-id="3d8ec-103">workbookRangeFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d8ec-103">workbookRangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d8ec-104">此对象表示对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="3d8ec-105">方法</span><span class="sxs-lookup"><span data-stu-id="3d8ec-105">Methods</span></span>

| <span data-ttu-id="3d8ec-106">方法</span><span class="sxs-lookup"><span data-stu-id="3d8ec-106">Method</span></span>           | <span data-ttu-id="3d8ec-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3d8ec-107">Return Type</span></span>    |<span data-ttu-id="3d8ec-108">说明</span><span class="sxs-lookup"><span data-stu-id="3d8ec-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3d8ec-109">获取 workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="3d8ec-109">Get workbookRangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="3d8ec-110">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="3d8ec-110">workbookRangeFont</span></span>](workbookrangefont.md) |<span data-ttu-id="3d8ec-111">读取 rangeFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="3d8ec-112">更新</span><span class="sxs-lookup"><span data-stu-id="3d8ec-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="3d8ec-113">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="3d8ec-113">workbookRangeFont</span></span>](workbookrangefont.md)   |<span data-ttu-id="3d8ec-114">更新 RangeFont 对象。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3d8ec-115">属性</span><span class="sxs-lookup"><span data-stu-id="3d8ec-115">Properties</span></span>
| <span data-ttu-id="3d8ec-116">属性</span><span class="sxs-lookup"><span data-stu-id="3d8ec-116">Property</span></span>     | <span data-ttu-id="3d8ec-117">类型</span><span class="sxs-lookup"><span data-stu-id="3d8ec-117">Type</span></span>   |<span data-ttu-id="3d8ec-118">说明</span><span class="sxs-lookup"><span data-stu-id="3d8ec-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d8ec-119">bold</span><span class="sxs-lookup"><span data-stu-id="3d8ec-119">bold</span></span>|<span data-ttu-id="3d8ec-120">boolean</span><span class="sxs-lookup"><span data-stu-id="3d8ec-120">boolean</span></span>|<span data-ttu-id="3d8ec-121">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="3d8ec-122">color</span><span class="sxs-lookup"><span data-stu-id="3d8ec-122">color</span></span>|<span data-ttu-id="3d8ec-123">string</span><span class="sxs-lookup"><span data-stu-id="3d8ec-123">string</span></span>|<span data-ttu-id="3d8ec-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="3d8ec-127">italic</span><span class="sxs-lookup"><span data-stu-id="3d8ec-127">italic</span></span>|<span data-ttu-id="3d8ec-128">布尔</span><span class="sxs-lookup"><span data-stu-id="3d8ec-128">boolean</span></span>|<span data-ttu-id="3d8ec-129">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="3d8ec-130">name</span><span class="sxs-lookup"><span data-stu-id="3d8ec-130">name</span></span>|<span data-ttu-id="3d8ec-131">string</span><span class="sxs-lookup"><span data-stu-id="3d8ec-131">string</span></span>|<span data-ttu-id="3d8ec-132">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="3d8ec-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="3d8ec-133">大小</span><span class="sxs-lookup"><span data-stu-id="3d8ec-133">size</span></span>|<span data-ttu-id="3d8ec-134">double</span><span class="sxs-lookup"><span data-stu-id="3d8ec-134">double</span></span>|<span data-ttu-id="3d8ec-135">字号</span><span class="sxs-lookup"><span data-stu-id="3d8ec-135">Font size.</span></span>|
|<span data-ttu-id="3d8ec-136">underline</span><span class="sxs-lookup"><span data-stu-id="3d8ec-136">underline</span></span>| <span data-ttu-id="3d8ec-137">String</span><span class="sxs-lookup"><span data-stu-id="3d8ec-137">String</span></span> |<span data-ttu-id="3d8ec-138">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-138">Type of underline applied to the font.</span></span> <span data-ttu-id="3d8ec-139">可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-139">Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d8ec-140">关系</span><span class="sxs-lookup"><span data-stu-id="3d8ec-140">Relationships</span></span>
<span data-ttu-id="3d8ec-141">无</span><span class="sxs-lookup"><span data-stu-id="3d8ec-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3d8ec-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d8ec-142">JSON representation</span></span>

<span data-ttu-id="3d8ec-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d8ec-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
