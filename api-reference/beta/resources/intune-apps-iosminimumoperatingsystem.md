---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: acee063da4c37627027bce2133201943a9194376
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918936"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="b6066-103">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6066-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="b6066-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b6066-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6066-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b6066-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6066-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b6066-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6066-107">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="b6066-107">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="b6066-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6066-108">Properties</span></span>
|<span data-ttu-id="b6066-109">属性</span><span class="sxs-lookup"><span data-stu-id="b6066-109">Property</span></span>|<span data-ttu-id="b6066-110">类型</span><span class="sxs-lookup"><span data-stu-id="b6066-110">Type</span></span>|<span data-ttu-id="b6066-111">说明</span><span class="sxs-lookup"><span data-stu-id="b6066-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6066-112">v8_0</span><span class="sxs-lookup"><span data-stu-id="b6066-112">v8_0</span></span>|<span data-ttu-id="b6066-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="b6066-113">Boolean</span></span>|<span data-ttu-id="b6066-114">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="b6066-114">Version 8.0 or later.</span></span>|
|<span data-ttu-id="b6066-115">v9_0</span><span class="sxs-lookup"><span data-stu-id="b6066-115">v9_0</span></span>|<span data-ttu-id="b6066-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="b6066-116">Boolean</span></span>|<span data-ttu-id="b6066-117">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="b6066-117">Version 9.0 or later.</span></span>|
|<span data-ttu-id="b6066-118">v10_0</span><span class="sxs-lookup"><span data-stu-id="b6066-118">v10_0</span></span>|<span data-ttu-id="b6066-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="b6066-119">Boolean</span></span>|<span data-ttu-id="b6066-120">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="b6066-120">Version 10.0 or later.</span></span>|
|<span data-ttu-id="b6066-121">v11_0</span><span class="sxs-lookup"><span data-stu-id="b6066-121">v11_0</span></span>|<span data-ttu-id="b6066-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="b6066-122">Boolean</span></span>|<span data-ttu-id="b6066-123">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="b6066-123">Version 11.0 or later.</span></span>|
|<span data-ttu-id="b6066-124">v12_0</span><span class="sxs-lookup"><span data-stu-id="b6066-124">v12_0</span></span>|<span data-ttu-id="b6066-125">布尔</span><span class="sxs-lookup"><span data-stu-id="b6066-125">Boolean</span></span>|<span data-ttu-id="b6066-126">12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="b6066-126">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6066-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="b6066-127">Relationships</span></span>
<span data-ttu-id="b6066-128">无</span><span class="sxs-lookup"><span data-stu-id="b6066-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b6066-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6066-129">JSON Representation</span></span>
<span data-ttu-id="b6066-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6066-130">Here is a JSON representation of the resource.</span></span>
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





