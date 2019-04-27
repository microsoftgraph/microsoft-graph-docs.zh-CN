---
title: workbookRangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eea7337fa4aefb1bde607740b9a2fc78264dae91
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348593"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="55e78-103">workbookRangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="55e78-103">workbookRangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55e78-104">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="55e78-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="55e78-105">方法</span><span class="sxs-lookup"><span data-stu-id="55e78-105">Methods</span></span>

| <span data-ttu-id="55e78-106">方法</span><span class="sxs-lookup"><span data-stu-id="55e78-106">Method</span></span>           | <span data-ttu-id="55e78-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="55e78-107">Return Type</span></span>    |<span data-ttu-id="55e78-108">说明</span><span class="sxs-lookup"><span data-stu-id="55e78-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55e78-109">获取 workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="55e78-109">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="55e78-110">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="55e78-110">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="55e78-111">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="55e78-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="55e78-112">更新</span><span class="sxs-lookup"><span data-stu-id="55e78-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="55e78-113">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="55e78-113">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="55e78-114">更新 RangeFill 对象</span><span class="sxs-lookup"><span data-stu-id="55e78-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="55e78-115">清除</span><span class="sxs-lookup"><span data-stu-id="55e78-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="55e78-116">None</span><span class="sxs-lookup"><span data-stu-id="55e78-116">None</span></span>|<span data-ttu-id="55e78-117">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="55e78-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="55e78-118">属性</span><span class="sxs-lookup"><span data-stu-id="55e78-118">Properties</span></span>
| <span data-ttu-id="55e78-119">属性</span><span class="sxs-lookup"><span data-stu-id="55e78-119">Property</span></span>     | <span data-ttu-id="55e78-120">类型</span><span class="sxs-lookup"><span data-stu-id="55e78-120">Type</span></span>   |<span data-ttu-id="55e78-121">说明</span><span class="sxs-lookup"><span data-stu-id="55e78-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55e78-122">color</span><span class="sxs-lookup"><span data-stu-id="55e78-122">color</span></span>|<span data-ttu-id="55e78-123">string</span><span class="sxs-lookup"><span data-stu-id="55e78-123">string</span></span>|<span data-ttu-id="55e78-124">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="55e78-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="55e78-125">关系</span><span class="sxs-lookup"><span data-stu-id="55e78-125">Relationships</span></span>
<span data-ttu-id="55e78-126">无</span><span class="sxs-lookup"><span data-stu-id="55e78-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="55e78-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55e78-127">JSON representation</span></span>

<span data-ttu-id="55e78-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55e78-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
