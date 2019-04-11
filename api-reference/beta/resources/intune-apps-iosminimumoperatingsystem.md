---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3775a9bbc9eee6bfef5dd1bef8235bf6fc770603
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795174"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="2bec9-103">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bec9-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="2bec9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2bec9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bec9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2bec9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bec9-106">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="2bec9-106">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="2bec9-107">属性</span><span class="sxs-lookup"><span data-stu-id="2bec9-107">Properties</span></span>
|<span data-ttu-id="2bec9-108">属性</span><span class="sxs-lookup"><span data-stu-id="2bec9-108">Property</span></span>|<span data-ttu-id="2bec9-109">类型</span><span class="sxs-lookup"><span data-stu-id="2bec9-109">Type</span></span>|<span data-ttu-id="2bec9-110">说明</span><span class="sxs-lookup"><span data-stu-id="2bec9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bec9-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="2bec9-111">v8_0</span></span>|<span data-ttu-id="2bec9-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="2bec9-112">Boolean</span></span>|<span data-ttu-id="2bec9-113">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="2bec9-113">Version 8.0 or later.</span></span>|
|<span data-ttu-id="2bec9-114">v9_0</span><span class="sxs-lookup"><span data-stu-id="2bec9-114">v9_0</span></span>|<span data-ttu-id="2bec9-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="2bec9-115">Boolean</span></span>|<span data-ttu-id="2bec9-116">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="2bec9-116">Version 9.0 or later.</span></span>|
|<span data-ttu-id="2bec9-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="2bec9-117">v10_0</span></span>|<span data-ttu-id="2bec9-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="2bec9-118">Boolean</span></span>|<span data-ttu-id="2bec9-119">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="2bec9-119">Version 10.0 or later.</span></span>|
|<span data-ttu-id="2bec9-120">v11_0</span><span class="sxs-lookup"><span data-stu-id="2bec9-120">v11_0</span></span>|<span data-ttu-id="2bec9-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="2bec9-121">Boolean</span></span>|<span data-ttu-id="2bec9-122">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="2bec9-122">Version 11.0 or later.</span></span>|
|<span data-ttu-id="2bec9-123">v12_0</span><span class="sxs-lookup"><span data-stu-id="2bec9-123">v12_0</span></span>|<span data-ttu-id="2bec9-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="2bec9-124">Boolean</span></span>|<span data-ttu-id="2bec9-125">版本12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="2bec9-125">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bec9-126">关系</span><span class="sxs-lookup"><span data-stu-id="2bec9-126">Relationships</span></span>
<span data-ttu-id="2bec9-127">无</span><span class="sxs-lookup"><span data-stu-id="2bec9-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bec9-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bec9-128">JSON Representation</span></span>
<span data-ttu-id="2bec9-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bec9-129">Here is a JSON representation of the resource.</span></span>
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





