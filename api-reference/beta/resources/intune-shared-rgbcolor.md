---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0295339c031b110a3203bc5b81a3b800f8f0b896
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084049"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="e95f8-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="e95f8-103">rgbColor resource type</span></span>

<span data-ttu-id="e95f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e95f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e95f8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e95f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e95f8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e95f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e95f8-107">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="e95f8-107">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="e95f8-108">属性</span><span class="sxs-lookup"><span data-stu-id="e95f8-108">Properties</span></span>
|<span data-ttu-id="e95f8-109">属性</span><span class="sxs-lookup"><span data-stu-id="e95f8-109">Property</span></span>|<span data-ttu-id="e95f8-110">类型</span><span class="sxs-lookup"><span data-stu-id="e95f8-110">Type</span></span>|<span data-ttu-id="e95f8-111">说明</span><span class="sxs-lookup"><span data-stu-id="e95f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e95f8-112">r</span><span class="sxs-lookup"><span data-stu-id="e95f8-112">r</span></span>|<span data-ttu-id="e95f8-113">字节</span><span class="sxs-lookup"><span data-stu-id="e95f8-113">Byte</span></span>|<span data-ttu-id="e95f8-114">红色值</span><span class="sxs-lookup"><span data-stu-id="e95f8-114">Red value</span></span>|
|<span data-ttu-id="e95f8-115">g</span><span class="sxs-lookup"><span data-stu-id="e95f8-115">g</span></span>|<span data-ttu-id="e95f8-116">字节</span><span class="sxs-lookup"><span data-stu-id="e95f8-116">Byte</span></span>|<span data-ttu-id="e95f8-117">绿色值</span><span class="sxs-lookup"><span data-stu-id="e95f8-117">Green value</span></span>|
|<span data-ttu-id="e95f8-118">b</span><span class="sxs-lookup"><span data-stu-id="e95f8-118">b</span></span>|<span data-ttu-id="e95f8-119">字节</span><span class="sxs-lookup"><span data-stu-id="e95f8-119">Byte</span></span>|<span data-ttu-id="e95f8-120">蓝色值</span><span class="sxs-lookup"><span data-stu-id="e95f8-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="e95f8-121">关系</span><span class="sxs-lookup"><span data-stu-id="e95f8-121">Relationships</span></span>
<span data-ttu-id="e95f8-122">无</span><span class="sxs-lookup"><span data-stu-id="e95f8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e95f8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e95f8-123">JSON Representation</span></span>
<span data-ttu-id="e95f8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e95f8-124">Here is a JSON representation of the resource.</span></span>
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






