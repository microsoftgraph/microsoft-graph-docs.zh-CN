---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52ace73dc7735a2e9c8fe316fc7a00a26564cdca
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754942"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="51c8f-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="51c8f-103">rgbColor resource type</span></span>

<span data-ttu-id="51c8f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51c8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51c8f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51c8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51c8f-106">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="51c8f-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="51c8f-107">属性</span><span class="sxs-lookup"><span data-stu-id="51c8f-107">Properties</span></span>
|<span data-ttu-id="51c8f-108">属性</span><span class="sxs-lookup"><span data-stu-id="51c8f-108">Property</span></span>|<span data-ttu-id="51c8f-109">类型</span><span class="sxs-lookup"><span data-stu-id="51c8f-109">Type</span></span>|<span data-ttu-id="51c8f-110">Description</span><span class="sxs-lookup"><span data-stu-id="51c8f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51c8f-111">r</span><span class="sxs-lookup"><span data-stu-id="51c8f-111">r</span></span>|<span data-ttu-id="51c8f-112">字节</span><span class="sxs-lookup"><span data-stu-id="51c8f-112">Byte</span></span>|<span data-ttu-id="51c8f-113">红色值</span><span class="sxs-lookup"><span data-stu-id="51c8f-113">Red value</span></span>|
|<span data-ttu-id="51c8f-114">g</span><span class="sxs-lookup"><span data-stu-id="51c8f-114">g</span></span>|<span data-ttu-id="51c8f-115">字节</span><span class="sxs-lookup"><span data-stu-id="51c8f-115">Byte</span></span>|<span data-ttu-id="51c8f-116">绿色值</span><span class="sxs-lookup"><span data-stu-id="51c8f-116">Green value</span></span>|
|<span data-ttu-id="51c8f-117">b</span><span class="sxs-lookup"><span data-stu-id="51c8f-117">b</span></span>|<span data-ttu-id="51c8f-118">字节</span><span class="sxs-lookup"><span data-stu-id="51c8f-118">Byte</span></span>|<span data-ttu-id="51c8f-119">蓝色值</span><span class="sxs-lookup"><span data-stu-id="51c8f-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="51c8f-120">关系</span><span class="sxs-lookup"><span data-stu-id="51c8f-120">Relationships</span></span>
<span data-ttu-id="51c8f-121">无</span><span class="sxs-lookup"><span data-stu-id="51c8f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51c8f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51c8f-122">JSON Representation</span></span>
<span data-ttu-id="51c8f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51c8f-123">Here is a JSON representation of the resource.</span></span>
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




