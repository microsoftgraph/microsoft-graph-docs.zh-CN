---
title: rgbColor 资源类型
description: 以 RGB 表示的颜色。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e58d4dfe1e75b4b37333e29858ce93d1383f75a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155676"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="23c10-103">rgbColor 资源类型</span><span class="sxs-lookup"><span data-stu-id="23c10-103">rgbColor resource type</span></span>

> <span data-ttu-id="23c10-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23c10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23c10-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23c10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23c10-106">以 RGB 表示的颜色。</span><span class="sxs-lookup"><span data-stu-id="23c10-106">Color in RGB.</span></span>

## <a name="properties"></a><span data-ttu-id="23c10-107">属性</span><span class="sxs-lookup"><span data-stu-id="23c10-107">Properties</span></span>
|<span data-ttu-id="23c10-108">属性</span><span class="sxs-lookup"><span data-stu-id="23c10-108">Property</span></span>|<span data-ttu-id="23c10-109">类型</span><span class="sxs-lookup"><span data-stu-id="23c10-109">Type</span></span>|<span data-ttu-id="23c10-110">说明</span><span class="sxs-lookup"><span data-stu-id="23c10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23c10-111">r</span><span class="sxs-lookup"><span data-stu-id="23c10-111">r</span></span>|<span data-ttu-id="23c10-112">字节</span><span class="sxs-lookup"><span data-stu-id="23c10-112">Byte</span></span>|<span data-ttu-id="23c10-113">红色值</span><span class="sxs-lookup"><span data-stu-id="23c10-113">Red value</span></span>|
|<span data-ttu-id="23c10-114">g</span><span class="sxs-lookup"><span data-stu-id="23c10-114">g</span></span>|<span data-ttu-id="23c10-115">字节</span><span class="sxs-lookup"><span data-stu-id="23c10-115">Byte</span></span>|<span data-ttu-id="23c10-116">绿色值</span><span class="sxs-lookup"><span data-stu-id="23c10-116">Green value</span></span>|
|<span data-ttu-id="23c10-117">b</span><span class="sxs-lookup"><span data-stu-id="23c10-117">b</span></span>|<span data-ttu-id="23c10-118">字节</span><span class="sxs-lookup"><span data-stu-id="23c10-118">Byte</span></span>|<span data-ttu-id="23c10-119">蓝色值</span><span class="sxs-lookup"><span data-stu-id="23c10-119">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="23c10-120">关系</span><span class="sxs-lookup"><span data-stu-id="23c10-120">Relationships</span></span>
<span data-ttu-id="23c10-121">无</span><span class="sxs-lookup"><span data-stu-id="23c10-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23c10-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23c10-122">JSON Representation</span></span>
<span data-ttu-id="23c10-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23c10-123">Here is a JSON representation of the resource.</span></span>
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




