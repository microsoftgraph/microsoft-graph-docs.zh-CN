---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 419577efc7993479e8f378227d5f6c073e8e2492
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360725"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="b0972-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0972-103">rgbColor resource type</span></span>

> <span data-ttu-id="b0972-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0972-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0972-105">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="b0972-105">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="b0972-106">属性</span><span class="sxs-lookup"><span data-stu-id="b0972-106">Properties</span></span>
|<span data-ttu-id="b0972-107">属性</span><span class="sxs-lookup"><span data-stu-id="b0972-107">Property</span></span>|<span data-ttu-id="b0972-108">类型</span><span class="sxs-lookup"><span data-stu-id="b0972-108">Type</span></span>|<span data-ttu-id="b0972-109">说明</span><span class="sxs-lookup"><span data-stu-id="b0972-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0972-110">r</span><span class="sxs-lookup"><span data-stu-id="b0972-110">r</span></span>|<span data-ttu-id="b0972-111">字节</span><span class="sxs-lookup"><span data-stu-id="b0972-111">Byte</span></span>|<span data-ttu-id="b0972-112">红色值</span><span class="sxs-lookup"><span data-stu-id="b0972-112">Red value</span></span>|
|<span data-ttu-id="b0972-113">g</span><span class="sxs-lookup"><span data-stu-id="b0972-113">g</span></span>|<span data-ttu-id="b0972-114">字节</span><span class="sxs-lookup"><span data-stu-id="b0972-114">Byte</span></span>|<span data-ttu-id="b0972-115">绿色值</span><span class="sxs-lookup"><span data-stu-id="b0972-115">Green value</span></span>|
|<span data-ttu-id="b0972-116">b</span><span class="sxs-lookup"><span data-stu-id="b0972-116">b</span></span>|<span data-ttu-id="b0972-117">字节</span><span class="sxs-lookup"><span data-stu-id="b0972-117">Byte</span></span>|<span data-ttu-id="b0972-118">蓝色值</span><span class="sxs-lookup"><span data-stu-id="b0972-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0972-119">关系</span><span class="sxs-lookup"><span data-stu-id="b0972-119">Relationships</span></span>
<span data-ttu-id="b0972-120">无</span><span class="sxs-lookup"><span data-stu-id="b0972-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0972-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0972-121">JSON Representation</span></span>
<span data-ttu-id="b0972-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0972-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```




