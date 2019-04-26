---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5ca085d009f38a2879074d7ee95a78acddf0f4a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572932"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="b72c5-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="b72c5-103">rgbColor resource type</span></span>

> <span data-ttu-id="b72c5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b72c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b72c5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b72c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b72c5-106">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="b72c5-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="b72c5-107">属性</span><span class="sxs-lookup"><span data-stu-id="b72c5-107">Properties</span></span>
|<span data-ttu-id="b72c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="b72c5-108">Property</span></span>|<span data-ttu-id="b72c5-109">类型</span><span class="sxs-lookup"><span data-stu-id="b72c5-109">Type</span></span>|<span data-ttu-id="b72c5-110">说明</span><span class="sxs-lookup"><span data-stu-id="b72c5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b72c5-111">r</span><span class="sxs-lookup"><span data-stu-id="b72c5-111">r</span></span>|<span data-ttu-id="b72c5-112">字节</span><span class="sxs-lookup"><span data-stu-id="b72c5-112">Byte</span></span>|<span data-ttu-id="b72c5-113">红色值</span><span class="sxs-lookup"><span data-stu-id="b72c5-113">Red value</span></span>|
|<span data-ttu-id="b72c5-114">g</span><span class="sxs-lookup"><span data-stu-id="b72c5-114">g</span></span>|<span data-ttu-id="b72c5-115">字节</span><span class="sxs-lookup"><span data-stu-id="b72c5-115">Byte</span></span>|<span data-ttu-id="b72c5-116">绿色值</span><span class="sxs-lookup"><span data-stu-id="b72c5-116">Green value</span></span>|
|<span data-ttu-id="b72c5-117">b</span><span class="sxs-lookup"><span data-stu-id="b72c5-117">b</span></span>|<span data-ttu-id="b72c5-118">字节</span><span class="sxs-lookup"><span data-stu-id="b72c5-118">Byte</span></span>|<span data-ttu-id="b72c5-119">蓝色值</span><span class="sxs-lookup"><span data-stu-id="b72c5-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="b72c5-120">关系</span><span class="sxs-lookup"><span data-stu-id="b72c5-120">Relationships</span></span>
<span data-ttu-id="b72c5-121">无</span><span class="sxs-lookup"><span data-stu-id="b72c5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b72c5-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b72c5-122">JSON Representation</span></span>
<span data-ttu-id="b72c5-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b72c5-123">Here is a JSON representation of the resource.</span></span>
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





