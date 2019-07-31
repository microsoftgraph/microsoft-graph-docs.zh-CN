---
title: workbookRangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: cb61352964323b0ded8733aa52ddd19854e028d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007093"
---
# <a name="workbookrangefill-resource-type"></a><span data-ttu-id="65f52-103">workbookRangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="65f52-103">workbookRangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65f52-104">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="65f52-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="65f52-105">方法</span><span class="sxs-lookup"><span data-stu-id="65f52-105">Methods</span></span>

| <span data-ttu-id="65f52-106">方法</span><span class="sxs-lookup"><span data-stu-id="65f52-106">Method</span></span>           | <span data-ttu-id="65f52-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="65f52-107">Return Type</span></span>    |<span data-ttu-id="65f52-108">说明</span><span class="sxs-lookup"><span data-stu-id="65f52-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65f52-109">获取 workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="65f52-109">Get workbookRangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="65f52-110">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="65f52-110">workbookRangeFill</span></span>](workbookrangefill.md) |<span data-ttu-id="65f52-111">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="65f52-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="65f52-112">更新</span><span class="sxs-lookup"><span data-stu-id="65f52-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="65f52-113">workbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="65f52-113">workbookRangeFill</span></span>](workbookrangefill.md)   |<span data-ttu-id="65f52-114">更新 RangeFill 对象</span><span class="sxs-lookup"><span data-stu-id="65f52-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="65f52-115">清除</span><span class="sxs-lookup"><span data-stu-id="65f52-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="65f52-116">None</span><span class="sxs-lookup"><span data-stu-id="65f52-116">None</span></span>|<span data-ttu-id="65f52-117">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="65f52-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="65f52-118">属性</span><span class="sxs-lookup"><span data-stu-id="65f52-118">Properties</span></span>
| <span data-ttu-id="65f52-119">属性</span><span class="sxs-lookup"><span data-stu-id="65f52-119">Property</span></span>     | <span data-ttu-id="65f52-120">类型</span><span class="sxs-lookup"><span data-stu-id="65f52-120">Type</span></span>   |<span data-ttu-id="65f52-121">说明</span><span class="sxs-lookup"><span data-stu-id="65f52-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65f52-122">color</span><span class="sxs-lookup"><span data-stu-id="65f52-122">color</span></span>|<span data-ttu-id="65f52-123">string</span><span class="sxs-lookup"><span data-stu-id="65f52-123">string</span></span>|<span data-ttu-id="65f52-124">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="65f52-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="65f52-125">关系</span><span class="sxs-lookup"><span data-stu-id="65f52-125">Relationships</span></span>
<span data-ttu-id="65f52-126">无</span><span class="sxs-lookup"><span data-stu-id="65f52-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="65f52-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65f52-127">JSON representation</span></span>

<span data-ttu-id="65f52-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65f52-128">Here is a JSON representation of the resource.</span></span>

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
