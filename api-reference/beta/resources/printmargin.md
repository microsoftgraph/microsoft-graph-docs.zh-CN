---
title: printMargin 资源类型
description: 指定打印时使用的页边距宽度。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8f89d2d4daa45d1043e3412852cdaa480223129b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048727"
---
# <a name="printmargin-complex-type"></a><span data-ttu-id="9c3ff-103">printMargin 复杂类型</span><span class="sxs-lookup"><span data-stu-id="9c3ff-103">printMargin complex type</span></span>

<span data-ttu-id="9c3ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c3ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c3ff-105">指定打印时使用的页边距宽度。</span><span class="sxs-lookup"><span data-stu-id="9c3ff-105">Specifies the margin widths to use when printing.</span></span>

## <a name="properties"></a><span data-ttu-id="9c3ff-106">属性</span><span class="sxs-lookup"><span data-stu-id="9c3ff-106">Properties</span></span>
| <span data-ttu-id="9c3ff-107">属性</span><span class="sxs-lookup"><span data-stu-id="9c3ff-107">Property</span></span>     | <span data-ttu-id="9c3ff-108">类型</span><span class="sxs-lookup"><span data-stu-id="9c3ff-108">Type</span></span>        | <span data-ttu-id="9c3ff-109">说明</span><span class="sxs-lookup"><span data-stu-id="9c3ff-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9c3ff-110">top</span><span class="sxs-lookup"><span data-stu-id="9c3ff-110">top</span></span>|<span data-ttu-id="9c3ff-111">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3ff-111">Int32</span></span>|<span data-ttu-id="9c3ff-112">从上边缘到 microns 中的边距。</span><span class="sxs-lookup"><span data-stu-id="9c3ff-112">The margin in microns from the top edge.</span></span>|
|<span data-ttu-id="9c3ff-113">bottom</span><span class="sxs-lookup"><span data-stu-id="9c3ff-113">bottom</span></span>|<span data-ttu-id="9c3ff-114">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3ff-114">Int32</span></span>|<span data-ttu-id="9c3ff-115">从下边缘 microns 的边距。</span><span class="sxs-lookup"><span data-stu-id="9c3ff-115">The margin in microns from the bottom edge.</span></span>|
|<span data-ttu-id="9c3ff-116">左向右</span><span class="sxs-lookup"><span data-stu-id="9c3ff-116">right</span></span>|<span data-ttu-id="9c3ff-117">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3ff-117">Int32</span></span>|<span data-ttu-id="9c3ff-118">从右边缘 microns 的边距。</span><span class="sxs-lookup"><span data-stu-id="9c3ff-118">The margin in microns from the right edge.</span></span>|
|<span data-ttu-id="9c3ff-119">左边</span><span class="sxs-lookup"><span data-stu-id="9c3ff-119">left</span></span>|<span data-ttu-id="9c3ff-120">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3ff-120">Int32</span></span>|<span data-ttu-id="9c3ff-121">从左边缘的 microns 中的边距。</span><span class="sxs-lookup"><span data-stu-id="9c3ff-121">The margin in microns from the left edge.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c3ff-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c3ff-122">JSON representation</span></span>

<span data-ttu-id="9c3ff-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c3ff-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printMargin"
}-->

```json
{
  "top": 123456,
  "bottom": 123456,
  "right": 123456,
  "left": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printMargin resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


