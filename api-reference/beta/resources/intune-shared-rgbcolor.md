---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d397c3660852d23e0fa92cd1036f2a30cc38d293
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733145"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="ed726-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed726-103">rgbColor resource type</span></span>

<span data-ttu-id="ed726-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed726-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed726-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed726-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed726-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed726-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed726-107">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="ed726-107">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="ed726-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed726-108">Properties</span></span>
|<span data-ttu-id="ed726-109">属性</span><span class="sxs-lookup"><span data-stu-id="ed726-109">Property</span></span>|<span data-ttu-id="ed726-110">类型</span><span class="sxs-lookup"><span data-stu-id="ed726-110">Type</span></span>|<span data-ttu-id="ed726-111">说明</span><span class="sxs-lookup"><span data-stu-id="ed726-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed726-112">r</span><span class="sxs-lookup"><span data-stu-id="ed726-112">r</span></span>|<span data-ttu-id="ed726-113">字节</span><span class="sxs-lookup"><span data-stu-id="ed726-113">Byte</span></span>|<span data-ttu-id="ed726-114">红色值</span><span class="sxs-lookup"><span data-stu-id="ed726-114">Red value</span></span>|
|<span data-ttu-id="ed726-115">g</span><span class="sxs-lookup"><span data-stu-id="ed726-115">g</span></span>|<span data-ttu-id="ed726-116">字节</span><span class="sxs-lookup"><span data-stu-id="ed726-116">Byte</span></span>|<span data-ttu-id="ed726-117">绿色值</span><span class="sxs-lookup"><span data-stu-id="ed726-117">Green value</span></span>|
|<span data-ttu-id="ed726-118">b</span><span class="sxs-lookup"><span data-stu-id="ed726-118">b</span></span>|<span data-ttu-id="ed726-119">字节</span><span class="sxs-lookup"><span data-stu-id="ed726-119">Byte</span></span>|<span data-ttu-id="ed726-120">蓝色值</span><span class="sxs-lookup"><span data-stu-id="ed726-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed726-121">关系</span><span class="sxs-lookup"><span data-stu-id="ed726-121">Relationships</span></span>
<span data-ttu-id="ed726-122">无</span><span class="sxs-lookup"><span data-stu-id="ed726-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed726-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed726-123">JSON Representation</span></span>
<span data-ttu-id="ed726-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed726-124">Here is a JSON representation of the resource.</span></span>
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





