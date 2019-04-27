---
title: workbookRangeFont 资源类型
description: 此对象表示对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 76b84a86c0d5796b4831fa362ee98c0b1093e830
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348610"
---
# <a name="workbookrangefont-resource-type"></a><span data-ttu-id="3e97d-103">workbookRangeFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e97d-103">workbookRangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e97d-104">此对象表示对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="3e97d-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="3e97d-105">方法</span><span class="sxs-lookup"><span data-stu-id="3e97d-105">Methods</span></span>

| <span data-ttu-id="3e97d-106">方法</span><span class="sxs-lookup"><span data-stu-id="3e97d-106">Method</span></span>           | <span data-ttu-id="3e97d-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e97d-107">Return Type</span></span>    |<span data-ttu-id="3e97d-108">说明</span><span class="sxs-lookup"><span data-stu-id="3e97d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3e97d-109">获取 workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="3e97d-109">Get workbookRangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="3e97d-110">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="3e97d-110">workbookRangeFont</span></span>](workbookrangefont.md) |<span data-ttu-id="3e97d-111">读取 rangeFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e97d-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="3e97d-112">更新</span><span class="sxs-lookup"><span data-stu-id="3e97d-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="3e97d-113">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="3e97d-113">workbookRangeFont</span></span>](workbookrangefont.md)   |<span data-ttu-id="3e97d-114">更新 RangeFont 对象。</span><span class="sxs-lookup"><span data-stu-id="3e97d-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3e97d-115">属性</span><span class="sxs-lookup"><span data-stu-id="3e97d-115">Properties</span></span>
| <span data-ttu-id="3e97d-116">属性</span><span class="sxs-lookup"><span data-stu-id="3e97d-116">Property</span></span>     | <span data-ttu-id="3e97d-117">类型</span><span class="sxs-lookup"><span data-stu-id="3e97d-117">Type</span></span>   |<span data-ttu-id="3e97d-118">说明</span><span class="sxs-lookup"><span data-stu-id="3e97d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e97d-119">bold</span><span class="sxs-lookup"><span data-stu-id="3e97d-119">bold</span></span>|<span data-ttu-id="3e97d-120">布尔</span><span class="sxs-lookup"><span data-stu-id="3e97d-120">boolean</span></span>|<span data-ttu-id="3e97d-121">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="3e97d-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="3e97d-122">color</span><span class="sxs-lookup"><span data-stu-id="3e97d-122">color</span></span>|<span data-ttu-id="3e97d-123">string</span><span class="sxs-lookup"><span data-stu-id="3e97d-123">string</span></span>|<span data-ttu-id="3e97d-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="3e97d-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="3e97d-127">italic</span><span class="sxs-lookup"><span data-stu-id="3e97d-127">italic</span></span>|<span data-ttu-id="3e97d-128">布尔</span><span class="sxs-lookup"><span data-stu-id="3e97d-128">boolean</span></span>|<span data-ttu-id="3e97d-129">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="3e97d-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="3e97d-130">name</span><span class="sxs-lookup"><span data-stu-id="3e97d-130">name</span></span>|<span data-ttu-id="3e97d-131">string</span><span class="sxs-lookup"><span data-stu-id="3e97d-131">string</span></span>|<span data-ttu-id="3e97d-132">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="3e97d-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="3e97d-133">大小</span><span class="sxs-lookup"><span data-stu-id="3e97d-133">size</span></span>|<span data-ttu-id="3e97d-134">double</span><span class="sxs-lookup"><span data-stu-id="3e97d-134">double</span></span>|<span data-ttu-id="3e97d-135">字号</span><span class="sxs-lookup"><span data-stu-id="3e97d-135">Font size.</span></span>|
|<span data-ttu-id="3e97d-136">underline</span><span class="sxs-lookup"><span data-stu-id="3e97d-136">underline</span></span>| <span data-ttu-id="3e97d-137">String</span><span class="sxs-lookup"><span data-stu-id="3e97d-137">String</span></span> |<span data-ttu-id="3e97d-138">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="3e97d-138">Type of underline applied to the font.</span></span> <span data-ttu-id="3e97d-139">可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="3e97d-139">Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e97d-140">关系</span><span class="sxs-lookup"><span data-stu-id="3e97d-140">Relationships</span></span>
<span data-ttu-id="3e97d-141">无</span><span class="sxs-lookup"><span data-stu-id="3e97d-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3e97d-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e97d-142">JSON representation</span></span>

<span data-ttu-id="3e97d-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e97d-143">Here is a JSON representation of the resource.</span></span>

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
