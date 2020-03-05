---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2cb52dcf33055539af503e5d49a05ce248c5187d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448009"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="f3275-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3275-103">rgbColor resource type</span></span>

<span data-ttu-id="f3275-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f3275-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3275-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3275-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3275-106">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="f3275-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="f3275-107">属性</span><span class="sxs-lookup"><span data-stu-id="f3275-107">Properties</span></span>
|<span data-ttu-id="f3275-108">属性</span><span class="sxs-lookup"><span data-stu-id="f3275-108">Property</span></span>|<span data-ttu-id="f3275-109">类型</span><span class="sxs-lookup"><span data-stu-id="f3275-109">Type</span></span>|<span data-ttu-id="f3275-110">说明</span><span class="sxs-lookup"><span data-stu-id="f3275-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3275-111">r</span><span class="sxs-lookup"><span data-stu-id="f3275-111">r</span></span>|<span data-ttu-id="f3275-112">字节</span><span class="sxs-lookup"><span data-stu-id="f3275-112">Byte</span></span>|<span data-ttu-id="f3275-113">红色值</span><span class="sxs-lookup"><span data-stu-id="f3275-113">Red value</span></span>|
|<span data-ttu-id="f3275-114">g</span><span class="sxs-lookup"><span data-stu-id="f3275-114">g</span></span>|<span data-ttu-id="f3275-115">字节</span><span class="sxs-lookup"><span data-stu-id="f3275-115">Byte</span></span>|<span data-ttu-id="f3275-116">绿色值</span><span class="sxs-lookup"><span data-stu-id="f3275-116">Green value</span></span>|
|<span data-ttu-id="f3275-117">b</span><span class="sxs-lookup"><span data-stu-id="f3275-117">b</span></span>|<span data-ttu-id="f3275-118">字节</span><span class="sxs-lookup"><span data-stu-id="f3275-118">Byte</span></span>|<span data-ttu-id="f3275-119">蓝色值</span><span class="sxs-lookup"><span data-stu-id="f3275-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3275-120">关系</span><span class="sxs-lookup"><span data-stu-id="f3275-120">Relationships</span></span>
<span data-ttu-id="f3275-121">无</span><span class="sxs-lookup"><span data-stu-id="f3275-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3275-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3275-122">JSON Representation</span></span>
<span data-ttu-id="f3275-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3275-123">Here is a JSON representation of the resource.</span></span>
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




