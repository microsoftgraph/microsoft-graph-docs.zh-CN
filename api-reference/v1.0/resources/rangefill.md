---
title: RangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 37bc96fdd0dad65a1f6b5b6bcec244ef96b915ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447022"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="65809-103">RangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="65809-103">RangeFill resource type</span></span>

<span data-ttu-id="65809-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="65809-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65809-105">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="65809-105">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="65809-106">方法</span><span class="sxs-lookup"><span data-stu-id="65809-106">Methods</span></span>

| <span data-ttu-id="65809-107">方法</span><span class="sxs-lookup"><span data-stu-id="65809-107">Method</span></span>           | <span data-ttu-id="65809-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="65809-108">Return Type</span></span>    |<span data-ttu-id="65809-109">说明</span><span class="sxs-lookup"><span data-stu-id="65809-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65809-110">获取 RangeFill</span><span class="sxs-lookup"><span data-stu-id="65809-110">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="65809-111">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="65809-111">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="65809-112">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="65809-112">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="65809-113">更新</span><span class="sxs-lookup"><span data-stu-id="65809-113">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="65809-114">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="65809-114">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="65809-115">更新 RangeFill 对象</span><span class="sxs-lookup"><span data-stu-id="65809-115">Update RangeFill object.</span></span> |
|[<span data-ttu-id="65809-116">清除</span><span class="sxs-lookup"><span data-stu-id="65809-116">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="65809-117">None</span><span class="sxs-lookup"><span data-stu-id="65809-117">None</span></span>|<span data-ttu-id="65809-118">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="65809-118">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="65809-119">属性</span><span class="sxs-lookup"><span data-stu-id="65809-119">Properties</span></span>
| <span data-ttu-id="65809-120">属性</span><span class="sxs-lookup"><span data-stu-id="65809-120">Property</span></span>     | <span data-ttu-id="65809-121">类型</span><span class="sxs-lookup"><span data-stu-id="65809-121">Type</span></span>   |<span data-ttu-id="65809-122">说明</span><span class="sxs-lookup"><span data-stu-id="65809-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65809-123">color</span><span class="sxs-lookup"><span data-stu-id="65809-123">color</span></span>|<span data-ttu-id="65809-124">string</span><span class="sxs-lookup"><span data-stu-id="65809-124">string</span></span>|<span data-ttu-id="65809-125">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="65809-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="65809-126">关系</span><span class="sxs-lookup"><span data-stu-id="65809-126">Relationships</span></span>
<span data-ttu-id="65809-127">无</span><span class="sxs-lookup"><span data-stu-id="65809-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="65809-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65809-128">JSON representation</span></span>

<span data-ttu-id="65809-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65809-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
