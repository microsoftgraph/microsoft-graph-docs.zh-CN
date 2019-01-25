---
title: RangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d1ae60c0b362ba8593f374c5edd505121cd18587
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509670"
---
# <a name="rangefill-resource-type"></a><span data-ttu-id="761f6-103">RangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="761f6-103">RangeFill resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="761f6-104">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="761f6-104">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="761f6-105">方法</span><span class="sxs-lookup"><span data-stu-id="761f6-105">Methods</span></span>

| <span data-ttu-id="761f6-106">方法</span><span class="sxs-lookup"><span data-stu-id="761f6-106">Method</span></span>           | <span data-ttu-id="761f6-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="761f6-107">Return Type</span></span>    |<span data-ttu-id="761f6-108">说明</span><span class="sxs-lookup"><span data-stu-id="761f6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="761f6-109">获取 RangeFill</span><span class="sxs-lookup"><span data-stu-id="761f6-109">[Get RangeFill](../api/rangefill-get.md)</span></span> | [<span data-ttu-id="761f6-110">RangeFill</span><span class="sxs-lookup"><span data-stu-id="761f6-110">RangeFill</span></span>](rangefill.md) |<span data-ttu-id="761f6-111">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="761f6-111">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="761f6-112">Update</span><span class="sxs-lookup"><span data-stu-id="761f6-112">Update</span></span>](../api/rangefill-update.md) | [<span data-ttu-id="761f6-113">RangeFill</span><span class="sxs-lookup"><span data-stu-id="761f6-113">RangeFill</span></span>](rangefill.md)   |<span data-ttu-id="761f6-114">更新 RangeFill 对象</span><span class="sxs-lookup"><span data-stu-id="761f6-114">Update RangeFill object.</span></span> |
|[<span data-ttu-id="761f6-115">清除</span><span class="sxs-lookup"><span data-stu-id="761f6-115">Clear</span></span>](../api/rangefill-clear.md)|<span data-ttu-id="761f6-116">无</span><span class="sxs-lookup"><span data-stu-id="761f6-116">None</span></span>|<span data-ttu-id="761f6-117">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="761f6-117">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="761f6-118">属性</span><span class="sxs-lookup"><span data-stu-id="761f6-118">Properties</span></span>
| <span data-ttu-id="761f6-119">属性</span><span class="sxs-lookup"><span data-stu-id="761f6-119">Property</span></span>     | <span data-ttu-id="761f6-120">类型</span><span class="sxs-lookup"><span data-stu-id="761f6-120">Type</span></span>   |<span data-ttu-id="761f6-121">说明</span><span class="sxs-lookup"><span data-stu-id="761f6-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="761f6-122">color</span><span class="sxs-lookup"><span data-stu-id="761f6-122">color</span></span>|<span data-ttu-id="761f6-123">string</span><span class="sxs-lookup"><span data-stu-id="761f6-123">string</span></span>|<span data-ttu-id="761f6-124">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="761f6-124">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="761f6-125">关系</span><span class="sxs-lookup"><span data-stu-id="761f6-125">Relationships</span></span>
<span data-ttu-id="761f6-126">无</span><span class="sxs-lookup"><span data-stu-id="761f6-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="761f6-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="761f6-127">JSON representation</span></span>

<span data-ttu-id="761f6-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="761f6-128">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefill.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
