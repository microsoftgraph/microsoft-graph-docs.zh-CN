---
title: RangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
ms.openlocfilehash: 21d40b1ec65ad49241af30912c3c05e114c7008d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323707"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="16ae3-103">RangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="16ae3-103">RangeFill resource type</span></span>

> <span data-ttu-id="16ae3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="16ae3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16ae3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="16ae3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16ae3-106">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="16ae3-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="16ae3-107">方法</span><span class="sxs-lookup"><span data-stu-id="16ae3-107">Methods</span></span>

| <span data-ttu-id="16ae3-108">方法</span><span class="sxs-lookup"><span data-stu-id="16ae3-108">Method</span></span>           | <span data-ttu-id="16ae3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="16ae3-109">Return Type</span></span>    |<span data-ttu-id="16ae3-110">说明</span><span class="sxs-lookup"><span data-stu-id="16ae3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16ae3-111">获取 RangeFill</span><span class="sxs-lookup"><span data-stu-id="16ae3-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="16ae3-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="16ae3-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="16ae3-113">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16ae3-113">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="16ae3-114">Update</span><span class="sxs-lookup"><span data-stu-id="16ae3-114">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="16ae3-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="16ae3-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="16ae3-116">更新 RangeFill 对象</span><span class="sxs-lookup"><span data-stu-id="16ae3-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="16ae3-117">Clear</span><span class="sxs-lookup"><span data-stu-id="16ae3-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="16ae3-118">无</span><span class="sxs-lookup"><span data-stu-id="16ae3-118">None</span></span>|<span data-ttu-id="16ae3-119">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="16ae3-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="16ae3-120">属性</span><span class="sxs-lookup"><span data-stu-id="16ae3-120">Properties</span></span>
| <span data-ttu-id="16ae3-121">属性</span><span class="sxs-lookup"><span data-stu-id="16ae3-121">Property</span></span>     | <span data-ttu-id="16ae3-122">类型</span><span class="sxs-lookup"><span data-stu-id="16ae3-122">Type</span></span>   |<span data-ttu-id="16ae3-123">说明</span><span class="sxs-lookup"><span data-stu-id="16ae3-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16ae3-124">color</span><span class="sxs-lookup"><span data-stu-id="16ae3-124">color</span></span>|<span data-ttu-id="16ae3-125">string</span><span class="sxs-lookup"><span data-stu-id="16ae3-125">string</span></span>|<span data-ttu-id="16ae3-126">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="16ae3-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="16ae3-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="16ae3-127">Relationships</span></span>
<span data-ttu-id="16ae3-128">无</span><span class="sxs-lookup"><span data-stu-id="16ae3-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="16ae3-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16ae3-129">JSON representation</span></span>

<span data-ttu-id="16ae3-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16ae3-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
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