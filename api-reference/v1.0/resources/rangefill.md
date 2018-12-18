---
title: RangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
ms.openlocfilehash: 6ddd039190af0e86067dfda651b2bc387b4cf74f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303561"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="50d21-103">RangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="50d21-103">RangeFill resource type</span></span>

<span data-ttu-id="50d21-104">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="50d21-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="50d21-105">方法</span><span class="sxs-lookup"><span data-stu-id="50d21-105">Methods</span></span>

| <span data-ttu-id="50d21-106">方法</span><span class="sxs-lookup"><span data-stu-id="50d21-106">Method</span></span>           | <span data-ttu-id="50d21-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="50d21-107">Return Type</span></span>    |<span data-ttu-id="50d21-108">说明</span><span class="sxs-lookup"><span data-stu-id="50d21-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50d21-109">获取 RangeFill</span><span class="sxs-lookup"><span data-stu-id="50d21-109">Get RangeFill</span></span>](../api/rangefill-get.md) | [<span data-ttu-id="50d21-110">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="50d21-110">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="50d21-111">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="50d21-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="50d21-112">Update</span><span class="sxs-lookup"><span data-stu-id="50d21-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="50d21-113">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="50d21-113">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="50d21-114">更新 RangeFill 对象</span><span class="sxs-lookup"><span data-stu-id="50d21-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="50d21-115">Clear</span><span class="sxs-lookup"><span data-stu-id="50d21-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="50d21-116">无</span><span class="sxs-lookup"><span data-stu-id="50d21-116">None</span></span>|<span data-ttu-id="50d21-117">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="50d21-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="50d21-118">属性</span><span class="sxs-lookup"><span data-stu-id="50d21-118">Properties</span></span>
| <span data-ttu-id="50d21-119">属性</span><span class="sxs-lookup"><span data-stu-id="50d21-119">Property</span></span>     | <span data-ttu-id="50d21-120">类型</span><span class="sxs-lookup"><span data-stu-id="50d21-120">Type</span></span>   |<span data-ttu-id="50d21-121">说明</span><span class="sxs-lookup"><span data-stu-id="50d21-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50d21-122">color</span><span class="sxs-lookup"><span data-stu-id="50d21-122">color</span></span>|<span data-ttu-id="50d21-123">string</span><span class="sxs-lookup"><span data-stu-id="50d21-123">string</span></span>|<span data-ttu-id="50d21-124">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="50d21-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="50d21-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="50d21-125">Relationships</span></span>
<span data-ttu-id="50d21-126">无</span><span class="sxs-lookup"><span data-stu-id="50d21-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="50d21-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50d21-127">JSON representation</span></span>

<span data-ttu-id="50d21-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50d21-128">Here is a JSON representation of the resource.</span></span>

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