---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7243b337a53cca31054f99ae807e5c17cdd3e372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876264"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="1cb7b-103">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="1cb7b-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="1cb7b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1cb7b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cb7b-105">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="1cb7b-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="1cb7b-106">属性</span><span class="sxs-lookup"><span data-stu-id="1cb7b-106">Properties</span></span>
|<span data-ttu-id="1cb7b-107">属性</span><span class="sxs-lookup"><span data-stu-id="1cb7b-107">Property</span></span>|<span data-ttu-id="1cb7b-108">类型</span><span class="sxs-lookup"><span data-stu-id="1cb7b-108">Type</span></span>|<span data-ttu-id="1cb7b-109">说明</span><span class="sxs-lookup"><span data-stu-id="1cb7b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cb7b-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="1cb7b-110">v8_0</span></span>|<span data-ttu-id="1cb7b-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="1cb7b-111">Boolean</span></span>|<span data-ttu-id="1cb7b-112">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="1cb7b-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="1cb7b-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="1cb7b-113">v9_0</span></span>|<span data-ttu-id="1cb7b-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="1cb7b-114">Boolean</span></span>|<span data-ttu-id="1cb7b-115">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="1cb7b-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="1cb7b-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="1cb7b-116">v10_0</span></span>|<span data-ttu-id="1cb7b-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="1cb7b-117">Boolean</span></span>|<span data-ttu-id="1cb7b-118">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="1cb7b-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="1cb7b-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="1cb7b-119">v11_0</span></span>|<span data-ttu-id="1cb7b-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="1cb7b-120">Boolean</span></span>|<span data-ttu-id="1cb7b-121">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="1cb7b-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="1cb7b-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="1cb7b-122">v12_0</span></span>|<span data-ttu-id="1cb7b-123">布尔</span><span class="sxs-lookup"><span data-stu-id="1cb7b-123">Boolean</span></span>|<span data-ttu-id="1cb7b-124">12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="1cb7b-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cb7b-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="1cb7b-125">Relationships</span></span>
<span data-ttu-id="1cb7b-126">无</span><span class="sxs-lookup"><span data-stu-id="1cb7b-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1cb7b-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cb7b-127">JSON Representation</span></span>
<span data-ttu-id="1cb7b-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cb7b-128">Here is a JSON representation of the resource.</span></span>
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



