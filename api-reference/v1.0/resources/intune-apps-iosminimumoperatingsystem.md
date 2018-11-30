---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
ms.openlocfilehash: 1b39890faf574ab952635c11f113c90479c3ba1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008483"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="bf7b1-103">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf7b1-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="bf7b1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf7b1-105">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="bf7b1-106">属性</span><span class="sxs-lookup"><span data-stu-id="bf7b1-106">Properties</span></span>
|<span data-ttu-id="bf7b1-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf7b1-107">Property</span></span>|<span data-ttu-id="bf7b1-108">类型</span><span class="sxs-lookup"><span data-stu-id="bf7b1-108">Type</span></span>|<span data-ttu-id="bf7b1-109">说明</span><span class="sxs-lookup"><span data-stu-id="bf7b1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf7b1-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="bf7b1-110">v8_0</span></span>|<span data-ttu-id="bf7b1-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="bf7b1-111">Boolean</span></span>|<span data-ttu-id="bf7b1-112">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="bf7b1-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="bf7b1-113">v9_0</span></span>|<span data-ttu-id="bf7b1-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="bf7b1-114">Boolean</span></span>|<span data-ttu-id="bf7b1-115">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="bf7b1-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="bf7b1-116">v10_0</span></span>|<span data-ttu-id="bf7b1-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="bf7b1-117">Boolean</span></span>|<span data-ttu-id="bf7b1-118">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="bf7b1-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="bf7b1-119">v11_0</span></span>|<span data-ttu-id="bf7b1-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="bf7b1-120">Boolean</span></span>|<span data-ttu-id="bf7b1-121">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="bf7b1-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="bf7b1-122">v12_0</span></span>|<span data-ttu-id="bf7b1-123">布尔</span><span class="sxs-lookup"><span data-stu-id="bf7b1-123">Boolean</span></span>|<span data-ttu-id="bf7b1-124">12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf7b1-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="bf7b1-125">Relationships</span></span>
<span data-ttu-id="bf7b1-126">无</span><span class="sxs-lookup"><span data-stu-id="bf7b1-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf7b1-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf7b1-127">JSON Representation</span></span>
<span data-ttu-id="bf7b1-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf7b1-128">Here is a JSON representation of the resource.</span></span>
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



