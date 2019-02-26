---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7490ad7b27d55fa6f2b7c6de12083025e7b4ac93
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254567"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="ebd54-103">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebd54-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="ebd54-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebd54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebd54-105">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="ebd54-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="ebd54-106">属性</span><span class="sxs-lookup"><span data-stu-id="ebd54-106">Properties</span></span>
|<span data-ttu-id="ebd54-107">属性</span><span class="sxs-lookup"><span data-stu-id="ebd54-107">Property</span></span>|<span data-ttu-id="ebd54-108">类型</span><span class="sxs-lookup"><span data-stu-id="ebd54-108">Type</span></span>|<span data-ttu-id="ebd54-109">说明</span><span class="sxs-lookup"><span data-stu-id="ebd54-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd54-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="ebd54-110">v8_0</span></span>|<span data-ttu-id="ebd54-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd54-111">Boolean</span></span>|<span data-ttu-id="ebd54-112">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ebd54-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="ebd54-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="ebd54-113">v9_0</span></span>|<span data-ttu-id="ebd54-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd54-114">Boolean</span></span>|<span data-ttu-id="ebd54-115">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ebd54-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="ebd54-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="ebd54-116">v10_0</span></span>|<span data-ttu-id="ebd54-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd54-117">Boolean</span></span>|<span data-ttu-id="ebd54-118">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ebd54-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="ebd54-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="ebd54-119">v11_0</span></span>|<span data-ttu-id="ebd54-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="ebd54-120">Boolean</span></span>|<span data-ttu-id="ebd54-121">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ebd54-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="ebd54-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="ebd54-122">v12_0</span></span>|<span data-ttu-id="ebd54-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="ebd54-123">Boolean</span></span>|<span data-ttu-id="ebd54-124">版本12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="ebd54-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebd54-125">关系</span><span class="sxs-lookup"><span data-stu-id="ebd54-125">Relationships</span></span>
<span data-ttu-id="ebd54-126">无</span><span class="sxs-lookup"><span data-stu-id="ebd54-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebd54-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebd54-127">JSON Representation</span></span>
<span data-ttu-id="ebd54-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebd54-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```



