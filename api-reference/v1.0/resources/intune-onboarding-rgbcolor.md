---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 98b5ce9dc5cb2f7d5f8c3c4d81c908dd776aa75f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441733"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="83fd3-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="83fd3-103">rgbColor resource type</span></span>

<span data-ttu-id="83fd3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83fd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83fd3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83fd3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83fd3-106">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="83fd3-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="83fd3-107">属性</span><span class="sxs-lookup"><span data-stu-id="83fd3-107">Properties</span></span>
|<span data-ttu-id="83fd3-108">属性</span><span class="sxs-lookup"><span data-stu-id="83fd3-108">Property</span></span>|<span data-ttu-id="83fd3-109">类型</span><span class="sxs-lookup"><span data-stu-id="83fd3-109">Type</span></span>|<span data-ttu-id="83fd3-110">说明</span><span class="sxs-lookup"><span data-stu-id="83fd3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83fd3-111">r</span><span class="sxs-lookup"><span data-stu-id="83fd3-111">r</span></span>|<span data-ttu-id="83fd3-112">字节</span><span class="sxs-lookup"><span data-stu-id="83fd3-112">Byte</span></span>|<span data-ttu-id="83fd3-113">红色值</span><span class="sxs-lookup"><span data-stu-id="83fd3-113">Red value</span></span>|
|<span data-ttu-id="83fd3-114">g</span><span class="sxs-lookup"><span data-stu-id="83fd3-114">g</span></span>|<span data-ttu-id="83fd3-115">字节</span><span class="sxs-lookup"><span data-stu-id="83fd3-115">Byte</span></span>|<span data-ttu-id="83fd3-116">绿色值</span><span class="sxs-lookup"><span data-stu-id="83fd3-116">Green value</span></span>|
|<span data-ttu-id="83fd3-117">b</span><span class="sxs-lookup"><span data-stu-id="83fd3-117">b</span></span>|<span data-ttu-id="83fd3-118">字节</span><span class="sxs-lookup"><span data-stu-id="83fd3-118">Byte</span></span>|<span data-ttu-id="83fd3-119">蓝色值</span><span class="sxs-lookup"><span data-stu-id="83fd3-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="83fd3-120">关系</span><span class="sxs-lookup"><span data-stu-id="83fd3-120">Relationships</span></span>
<span data-ttu-id="83fd3-121">无</span><span class="sxs-lookup"><span data-stu-id="83fd3-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83fd3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83fd3-122">JSON Representation</span></span>
<span data-ttu-id="83fd3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83fd3-123">Here is a JSON representation of the resource.</span></span>
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







