---
title: RangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 75aa4bd91ad6f1038fdc42460c6a3c9ab928a09d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911817"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="86bad-103">RangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="86bad-103">RangeFill resource type</span></span>

<span data-ttu-id="86bad-104">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="86bad-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="86bad-105">方法</span><span class="sxs-lookup"><span data-stu-id="86bad-105">Methods</span></span>

| <span data-ttu-id="86bad-106">方法</span><span class="sxs-lookup"><span data-stu-id="86bad-106">Method</span></span>           | <span data-ttu-id="86bad-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="86bad-107">Return Type</span></span>    |<span data-ttu-id="86bad-108">说明</span><span class="sxs-lookup"><span data-stu-id="86bad-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86bad-109">获取 RangeFill</span><span class="sxs-lookup"><span data-stu-id="86bad-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="86bad-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="86bad-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="86bad-111">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86bad-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="86bad-112">Update</span><span class="sxs-lookup"><span data-stu-id="86bad-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="86bad-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="86bad-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="86bad-114">更新 RangeFill 对象</span><span class="sxs-lookup"><span data-stu-id="86bad-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="86bad-115">Clear</span><span class="sxs-lookup"><span data-stu-id="86bad-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="86bad-116">无</span><span class="sxs-lookup"><span data-stu-id="86bad-116">None</span></span>|<span data-ttu-id="86bad-117">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="86bad-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="86bad-118">属性</span><span class="sxs-lookup"><span data-stu-id="86bad-118">Properties</span></span>
| <span data-ttu-id="86bad-119">属性</span><span class="sxs-lookup"><span data-stu-id="86bad-119">Property</span></span>     | <span data-ttu-id="86bad-120">类型</span><span class="sxs-lookup"><span data-stu-id="86bad-120">Type</span></span>   |<span data-ttu-id="86bad-121">说明</span><span class="sxs-lookup"><span data-stu-id="86bad-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86bad-122">color</span><span class="sxs-lookup"><span data-stu-id="86bad-122">color</span></span>|<span data-ttu-id="86bad-123">string</span><span class="sxs-lookup"><span data-stu-id="86bad-123">string</span></span>|<span data-ttu-id="86bad-124">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="86bad-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="86bad-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="86bad-125">Relationships</span></span>
<span data-ttu-id="86bad-126">无</span><span class="sxs-lookup"><span data-stu-id="86bad-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="86bad-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86bad-127">JSON representation</span></span>

<span data-ttu-id="86bad-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86bad-128">Here is a JSON representation of the resource.</span></span>

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
