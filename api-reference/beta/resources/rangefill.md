---
title: RangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8ceab66373331b6e144b69119d521a3e5ddccdc7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817757"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="2474e-103">RangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="2474e-103">RangeFill resource type</span></span>

> <span data-ttu-id="2474e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2474e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2474e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2474e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2474e-106">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="2474e-106">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="2474e-107">方法</span><span class="sxs-lookup"><span data-stu-id="2474e-107">Methods</span></span>

| <span data-ttu-id="2474e-108">方法</span><span class="sxs-lookup"><span data-stu-id="2474e-108">Method</span></span>           | <span data-ttu-id="2474e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2474e-109">Return Type</span></span>    |<span data-ttu-id="2474e-110">说明</span><span class="sxs-lookup"><span data-stu-id="2474e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2474e-111">获取 RangeFill</span><span class="sxs-lookup"><span data-stu-id="2474e-111">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="2474e-112">RangeFill</span><span class="sxs-lookup"><span data-stu-id="2474e-112">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="2474e-113">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2474e-113">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="2474e-114">Update</span><span class="sxs-lookup"><span data-stu-id="2474e-114">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="2474e-115">RangeFill</span><span class="sxs-lookup"><span data-stu-id="2474e-115">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="2474e-116">更新 RangeFill 对象</span><span class="sxs-lookup"><span data-stu-id="2474e-116">Update RangeFill object.</span></span> |
|[<span data-ttu-id="2474e-117">Clear</span><span class="sxs-lookup"><span data-stu-id="2474e-117">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="2474e-118">无</span><span class="sxs-lookup"><span data-stu-id="2474e-118">None</span></span>|<span data-ttu-id="2474e-119">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="2474e-119">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="2474e-120">属性</span><span class="sxs-lookup"><span data-stu-id="2474e-120">Properties</span></span>
| <span data-ttu-id="2474e-121">属性</span><span class="sxs-lookup"><span data-stu-id="2474e-121">Property</span></span>     | <span data-ttu-id="2474e-122">类型</span><span class="sxs-lookup"><span data-stu-id="2474e-122">Type</span></span>   |<span data-ttu-id="2474e-123">说明</span><span class="sxs-lookup"><span data-stu-id="2474e-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2474e-124">color</span><span class="sxs-lookup"><span data-stu-id="2474e-124">color</span></span>|<span data-ttu-id="2474e-125">string</span><span class="sxs-lookup"><span data-stu-id="2474e-125">string</span></span>|<span data-ttu-id="2474e-126">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="2474e-126">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="2474e-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="2474e-127">Relationships</span></span>
<span data-ttu-id="2474e-128">无</span><span class="sxs-lookup"><span data-stu-id="2474e-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2474e-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2474e-129">JSON representation</span></span>

<span data-ttu-id="2474e-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2474e-130">Here is a JSON representation of the resource.</span></span>

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
