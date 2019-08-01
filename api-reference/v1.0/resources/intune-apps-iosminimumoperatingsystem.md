---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da56780e66e88baaa074c3106997e3b4a3cc3b64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032345"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="98c53-103">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="98c53-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="98c53-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98c53-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98c53-105">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="98c53-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="98c53-106">属性</span><span class="sxs-lookup"><span data-stu-id="98c53-106">Properties</span></span>
|<span data-ttu-id="98c53-107">属性</span><span class="sxs-lookup"><span data-stu-id="98c53-107">Property</span></span>|<span data-ttu-id="98c53-108">类型</span><span class="sxs-lookup"><span data-stu-id="98c53-108">Type</span></span>|<span data-ttu-id="98c53-109">说明</span><span class="sxs-lookup"><span data-stu-id="98c53-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98c53-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="98c53-110">v8_0</span></span>|<span data-ttu-id="98c53-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="98c53-111">Boolean</span></span>|<span data-ttu-id="98c53-112">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="98c53-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="98c53-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="98c53-113">v9_0</span></span>|<span data-ttu-id="98c53-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="98c53-114">Boolean</span></span>|<span data-ttu-id="98c53-115">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="98c53-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="98c53-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="98c53-116">v10_0</span></span>|<span data-ttu-id="98c53-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="98c53-117">Boolean</span></span>|<span data-ttu-id="98c53-118">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="98c53-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="98c53-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="98c53-119">v11_0</span></span>|<span data-ttu-id="98c53-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="98c53-120">Boolean</span></span>|<span data-ttu-id="98c53-121">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="98c53-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="98c53-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="98c53-122">v12_0</span></span>|<span data-ttu-id="98c53-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="98c53-123">Boolean</span></span>|<span data-ttu-id="98c53-124">版本12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="98c53-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98c53-125">关系</span><span class="sxs-lookup"><span data-stu-id="98c53-125">Relationships</span></span>
<span data-ttu-id="98c53-126">无</span><span class="sxs-lookup"><span data-stu-id="98c53-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98c53-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98c53-127">JSON Representation</span></span>
<span data-ttu-id="98c53-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98c53-128">Here is a JSON representation of the resource.</span></span>
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



