---
title: printMargin 资源类型
description: 指定打印时使用的边距宽度。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1680cc641da02f3339dcd75977c411d3255cf037
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517291"
---
# <a name="printmargin-resource-type"></a><span data-ttu-id="84667-103">printMargin 资源类型</span><span class="sxs-lookup"><span data-stu-id="84667-103">printMargin resource type</span></span>

<span data-ttu-id="84667-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84667-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="84667-105">指定打印时使用的边距宽度。</span><span class="sxs-lookup"><span data-stu-id="84667-105">Specifies the margin widths to use when printing.</span></span>

## <a name="properties"></a><span data-ttu-id="84667-106">属性</span><span class="sxs-lookup"><span data-stu-id="84667-106">Properties</span></span>
|<span data-ttu-id="84667-107">属性</span><span class="sxs-lookup"><span data-stu-id="84667-107">Property</span></span>|<span data-ttu-id="84667-108">类型</span><span class="sxs-lookup"><span data-stu-id="84667-108">Type</span></span>|<span data-ttu-id="84667-109">Description</span><span class="sxs-lookup"><span data-stu-id="84667-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84667-110">top</span><span class="sxs-lookup"><span data-stu-id="84667-110">top</span></span>|<span data-ttu-id="84667-111">Int32</span><span class="sxs-lookup"><span data-stu-id="84667-111">Int32</span></span>|<span data-ttu-id="84667-112">上边缘的边距（以密分表示）。</span><span class="sxs-lookup"><span data-stu-id="84667-112">The margin in microns from the top edge.</span></span>|
|<span data-ttu-id="84667-113">bottom</span><span class="sxs-lookup"><span data-stu-id="84667-113">bottom</span></span>|<span data-ttu-id="84667-114">Int32</span><span class="sxs-lookup"><span data-stu-id="84667-114">Int32</span></span>|<span data-ttu-id="84667-115">下边缘的边距（以密分表示）。</span><span class="sxs-lookup"><span data-stu-id="84667-115">The margin in microns from the bottom edge.</span></span>|
|<span data-ttu-id="84667-116">right</span><span class="sxs-lookup"><span data-stu-id="84667-116">right</span></span>|<span data-ttu-id="84667-117">Int32</span><span class="sxs-lookup"><span data-stu-id="84667-117">Int32</span></span>|<span data-ttu-id="84667-118">右边缘的边距（以密分表示）。</span><span class="sxs-lookup"><span data-stu-id="84667-118">The margin in microns from the right edge.</span></span>|
|<span data-ttu-id="84667-119">左边</span><span class="sxs-lookup"><span data-stu-id="84667-119">left</span></span>|<span data-ttu-id="84667-120">Int32</span><span class="sxs-lookup"><span data-stu-id="84667-120">Int32</span></span>|<span data-ttu-id="84667-121">距左边缘的边距（以密分表示）。</span><span class="sxs-lookup"><span data-stu-id="84667-121">The margin in microns from the left edge.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84667-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84667-122">JSON representation</span></span>
<span data-ttu-id="84667-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84667-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printMargin"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printMargin",
  "top": "Integer",
  "bottom": "Integer",
  "right": "Integer",
  "left": "Integer"
}
```

