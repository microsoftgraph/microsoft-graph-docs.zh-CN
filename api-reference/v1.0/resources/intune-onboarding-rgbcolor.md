---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4cb75dd05710fbe5ca4d61d34dfc43f07d5f8a7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066325"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="7fc0e-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="7fc0e-103">rgbColor resource type</span></span>

<span data-ttu-id="7fc0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fc0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7fc0e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7fc0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fc0e-106">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="7fc0e-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="7fc0e-107">属性</span><span class="sxs-lookup"><span data-stu-id="7fc0e-107">Properties</span></span>
|<span data-ttu-id="7fc0e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7fc0e-108">Property</span></span>|<span data-ttu-id="7fc0e-109">类型</span><span class="sxs-lookup"><span data-stu-id="7fc0e-109">Type</span></span>|<span data-ttu-id="7fc0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="7fc0e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fc0e-111">r</span><span class="sxs-lookup"><span data-stu-id="7fc0e-111">r</span></span>|<span data-ttu-id="7fc0e-112">字节</span><span class="sxs-lookup"><span data-stu-id="7fc0e-112">Byte</span></span>|<span data-ttu-id="7fc0e-113">红色值</span><span class="sxs-lookup"><span data-stu-id="7fc0e-113">Red value</span></span>|
|<span data-ttu-id="7fc0e-114">g</span><span class="sxs-lookup"><span data-stu-id="7fc0e-114">g</span></span>|<span data-ttu-id="7fc0e-115">字节</span><span class="sxs-lookup"><span data-stu-id="7fc0e-115">Byte</span></span>|<span data-ttu-id="7fc0e-116">绿色值</span><span class="sxs-lookup"><span data-stu-id="7fc0e-116">Green value</span></span>|
|<span data-ttu-id="7fc0e-117">b</span><span class="sxs-lookup"><span data-stu-id="7fc0e-117">b</span></span>|<span data-ttu-id="7fc0e-118">字节</span><span class="sxs-lookup"><span data-stu-id="7fc0e-118">Byte</span></span>|<span data-ttu-id="7fc0e-119">蓝色值</span><span class="sxs-lookup"><span data-stu-id="7fc0e-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="7fc0e-120">关系</span><span class="sxs-lookup"><span data-stu-id="7fc0e-120">Relationships</span></span>
<span data-ttu-id="7fc0e-121">无</span><span class="sxs-lookup"><span data-stu-id="7fc0e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fc0e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fc0e-122">JSON Representation</span></span>
<span data-ttu-id="7fc0e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fc0e-123">Here is a JSON representation of the resource.</span></span>
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









