---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2222d7142ea033a8db2c2ce263da04c3b33153
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524552"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="38895-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="38895-103">rgbColor resource type</span></span>

> <span data-ttu-id="38895-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38895-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38895-105">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="38895-105">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="38895-106">属性</span><span class="sxs-lookup"><span data-stu-id="38895-106">Properties</span></span>
|<span data-ttu-id="38895-107">属性</span><span class="sxs-lookup"><span data-stu-id="38895-107">Property</span></span>|<span data-ttu-id="38895-108">类型</span><span class="sxs-lookup"><span data-stu-id="38895-108">Type</span></span>|<span data-ttu-id="38895-109">说明</span><span class="sxs-lookup"><span data-stu-id="38895-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38895-110">r</span><span class="sxs-lookup"><span data-stu-id="38895-110">r</span></span>|<span data-ttu-id="38895-111">字节</span><span class="sxs-lookup"><span data-stu-id="38895-111">Byte</span></span>|<span data-ttu-id="38895-112">红色值</span><span class="sxs-lookup"><span data-stu-id="38895-112">Red value</span></span>|
|<span data-ttu-id="38895-113">g</span><span class="sxs-lookup"><span data-stu-id="38895-113">g</span></span>|<span data-ttu-id="38895-114">字节</span><span class="sxs-lookup"><span data-stu-id="38895-114">Byte</span></span>|<span data-ttu-id="38895-115">绿色值</span><span class="sxs-lookup"><span data-stu-id="38895-115">Green value</span></span>|
|<span data-ttu-id="38895-116">b</span><span class="sxs-lookup"><span data-stu-id="38895-116">b</span></span>|<span data-ttu-id="38895-117">字节</span><span class="sxs-lookup"><span data-stu-id="38895-117">Byte</span></span>|<span data-ttu-id="38895-118">蓝色值</span><span class="sxs-lookup"><span data-stu-id="38895-118">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="38895-119">关系</span><span class="sxs-lookup"><span data-stu-id="38895-119">Relationships</span></span>
<span data-ttu-id="38895-120">无</span><span class="sxs-lookup"><span data-stu-id="38895-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38895-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38895-121">JSON Representation</span></span>
<span data-ttu-id="38895-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38895-122">Here is a JSON representation of the resource.</span></span>
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



