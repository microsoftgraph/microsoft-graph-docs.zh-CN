---
title: workbookRangeFont 资源类型
description: 此对象表示对象的字体属性（字体名称、字体大小、颜色等）。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9ddbb607a243f4571d53dcf887f80a171b230748
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519174"
---
# <a name="workbookrangefont-resource-type"></a><span data-ttu-id="72f86-103">workbookRangeFont 资源类型</span><span class="sxs-lookup"><span data-stu-id="72f86-103">workbookRangeFont resource type</span></span>

<span data-ttu-id="72f86-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="72f86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72f86-105">此对象表示对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="72f86-105">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="72f86-106">方法</span><span class="sxs-lookup"><span data-stu-id="72f86-106">Methods</span></span>

| <span data-ttu-id="72f86-107">方法</span><span class="sxs-lookup"><span data-stu-id="72f86-107">Method</span></span>           | <span data-ttu-id="72f86-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="72f86-108">Return Type</span></span>    |<span data-ttu-id="72f86-109">说明</span><span class="sxs-lookup"><span data-stu-id="72f86-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72f86-110">获取 workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="72f86-110">Get workbookRangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="72f86-111">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="72f86-111">workbookRangeFont</span></span>](workbookrangefont.md) |<span data-ttu-id="72f86-112">读取 rangeFont 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72f86-112">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="72f86-113">更新</span><span class="sxs-lookup"><span data-stu-id="72f86-113">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="72f86-114">workbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="72f86-114">workbookRangeFont</span></span>](workbookrangefont.md)   |<span data-ttu-id="72f86-115">更新 RangeFont 对象。</span><span class="sxs-lookup"><span data-stu-id="72f86-115">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="72f86-116">属性</span><span class="sxs-lookup"><span data-stu-id="72f86-116">Properties</span></span>
| <span data-ttu-id="72f86-117">属性</span><span class="sxs-lookup"><span data-stu-id="72f86-117">Property</span></span>     | <span data-ttu-id="72f86-118">类型</span><span class="sxs-lookup"><span data-stu-id="72f86-118">Type</span></span>   |<span data-ttu-id="72f86-119">说明</span><span class="sxs-lookup"><span data-stu-id="72f86-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72f86-120">bold</span><span class="sxs-lookup"><span data-stu-id="72f86-120">bold</span></span>|<span data-ttu-id="72f86-121">boolean</span><span class="sxs-lookup"><span data-stu-id="72f86-121">boolean</span></span>|<span data-ttu-id="72f86-122">表示字体的加粗状态。</span><span class="sxs-lookup"><span data-stu-id="72f86-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="72f86-123">color</span><span class="sxs-lookup"><span data-stu-id="72f86-123">color</span></span>|<span data-ttu-id="72f86-124">string</span><span class="sxs-lookup"><span data-stu-id="72f86-124">string</span></span>|<span data-ttu-id="72f86-p101">文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。</span><span class="sxs-lookup"><span data-stu-id="72f86-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="72f86-128">italic</span><span class="sxs-lookup"><span data-stu-id="72f86-128">italic</span></span>|<span data-ttu-id="72f86-129">布尔</span><span class="sxs-lookup"><span data-stu-id="72f86-129">boolean</span></span>|<span data-ttu-id="72f86-130">表示字体的斜体状态。</span><span class="sxs-lookup"><span data-stu-id="72f86-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="72f86-131">name</span><span class="sxs-lookup"><span data-stu-id="72f86-131">name</span></span>|<span data-ttu-id="72f86-132">string</span><span class="sxs-lookup"><span data-stu-id="72f86-132">string</span></span>|<span data-ttu-id="72f86-133">字体名称（例如"Calibri"）</span><span class="sxs-lookup"><span data-stu-id="72f86-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="72f86-134">大小</span><span class="sxs-lookup"><span data-stu-id="72f86-134">size</span></span>|<span data-ttu-id="72f86-135">double</span><span class="sxs-lookup"><span data-stu-id="72f86-135">double</span></span>|<span data-ttu-id="72f86-136">字号</span><span class="sxs-lookup"><span data-stu-id="72f86-136">Font size.</span></span>|
|<span data-ttu-id="72f86-137">underline</span><span class="sxs-lookup"><span data-stu-id="72f86-137">underline</span></span>| <span data-ttu-id="72f86-138">String</span><span class="sxs-lookup"><span data-stu-id="72f86-138">String</span></span> |<span data-ttu-id="72f86-139">应用于字体的下划线类型。</span><span class="sxs-lookup"><span data-stu-id="72f86-139">Type of underline applied to the font.</span></span> <span data-ttu-id="72f86-140">可能的值是：`None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。</span><span class="sxs-lookup"><span data-stu-id="72f86-140">Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72f86-141">关系</span><span class="sxs-lookup"><span data-stu-id="72f86-141">Relationships</span></span>
<span data-ttu-id="72f86-142">无</span><span class="sxs-lookup"><span data-stu-id="72f86-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="72f86-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72f86-143">JSON representation</span></span>

<span data-ttu-id="72f86-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72f86-144">Here is a JSON representation of the resource.</span></span>

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
