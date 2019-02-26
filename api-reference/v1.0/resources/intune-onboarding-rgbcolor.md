---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2222d7142ea033a8db2c2ce263da04c3b33153
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250297"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="ce2cb-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce2cb-103">rgbColor resource type</span></span>

> <span data-ttu-id="ce2cb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce2cb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce2cb-105">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="ce2cb-105">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="ce2cb-106">属性</span><span class="sxs-lookup"><span data-stu-id="ce2cb-106">Properties</span></span>
|<span data-ttu-id="ce2cb-107">属性</span><span class="sxs-lookup"><span data-stu-id="ce2cb-107">Property</span></span>|<span data-ttu-id="ce2cb-108">类型</span><span class="sxs-lookup"><span data-stu-id="ce2cb-108">Type</span></span>|<span data-ttu-id="ce2cb-109">说明</span><span class="sxs-lookup"><span data-stu-id="ce2cb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce2cb-110">r</span><span class="sxs-lookup"><span data-stu-id="ce2cb-110">r</span></span>|<span data-ttu-id="ce2cb-111">字节</span><span class="sxs-lookup"><span data-stu-id="ce2cb-111">Byte</span></span>|<span data-ttu-id="ce2cb-112">红色值</span><span class="sxs-lookup"><span data-stu-id="ce2cb-112">Red value</span></span>|
|<span data-ttu-id="ce2cb-113">g</span><span class="sxs-lookup"><span data-stu-id="ce2cb-113">g</span></span>|<span data-ttu-id="ce2cb-114">字节</span><span class="sxs-lookup"><span data-stu-id="ce2cb-114">Byte</span></span>|<span data-ttu-id="ce2cb-115">绿色值</span><span class="sxs-lookup"><span data-stu-id="ce2cb-115">Green value</span></span>|
|<span data-ttu-id="ce2cb-116">b</span><span class="sxs-lookup"><span data-stu-id="ce2cb-116">b</span></span>|<span data-ttu-id="ce2cb-117">字节</span><span class="sxs-lookup"><span data-stu-id="ce2cb-117">Byte</span></span>|<span data-ttu-id="ce2cb-118">蓝色值</span><span class="sxs-lookup"><span data-stu-id="ce2cb-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce2cb-119">关系</span><span class="sxs-lookup"><span data-stu-id="ce2cb-119">Relationships</span></span>
<span data-ttu-id="ce2cb-120">无</span><span class="sxs-lookup"><span data-stu-id="ce2cb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce2cb-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce2cb-121">JSON Representation</span></span>
<span data-ttu-id="ce2cb-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce2cb-122">Here is a JSON representation of the resource.</span></span>
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



