---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a80de09abe7e5fb513c95006f6b2c2fe719a4f39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925936"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="616be-103">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="616be-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="616be-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="616be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="616be-105">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="616be-105">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>
## <a name="properties"></a><span data-ttu-id="616be-106">属性</span><span class="sxs-lookup"><span data-stu-id="616be-106">Properties</span></span>
|<span data-ttu-id="616be-107">属性</span><span class="sxs-lookup"><span data-stu-id="616be-107">Property</span></span>|<span data-ttu-id="616be-108">类型</span><span class="sxs-lookup"><span data-stu-id="616be-108">Type</span></span>|<span data-ttu-id="616be-109">说明</span><span class="sxs-lookup"><span data-stu-id="616be-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="616be-110">v8_0</span><span class="sxs-lookup"><span data-stu-id="616be-110">v8_0</span></span>|<span data-ttu-id="616be-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="616be-111">Boolean</span></span>|<span data-ttu-id="616be-112">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="616be-112">Version 8.0 or later.</span></span>|
|<span data-ttu-id="616be-113">v9_0</span><span class="sxs-lookup"><span data-stu-id="616be-113">v9_0</span></span>|<span data-ttu-id="616be-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="616be-114">Boolean</span></span>|<span data-ttu-id="616be-115">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="616be-115">Version 9.0 or later.</span></span>|
|<span data-ttu-id="616be-116">v10_0</span><span class="sxs-lookup"><span data-stu-id="616be-116">v10_0</span></span>|<span data-ttu-id="616be-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="616be-117">Boolean</span></span>|<span data-ttu-id="616be-118">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="616be-118">Version 10.0 or later.</span></span>|
|<span data-ttu-id="616be-119">v11_0</span><span class="sxs-lookup"><span data-stu-id="616be-119">v11_0</span></span>|<span data-ttu-id="616be-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="616be-120">Boolean</span></span>|<span data-ttu-id="616be-121">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="616be-121">Version 11.0 or later.</span></span>|
|<span data-ttu-id="616be-122">v12_0</span><span class="sxs-lookup"><span data-stu-id="616be-122">v12_0</span></span>|<span data-ttu-id="616be-123">布尔</span><span class="sxs-lookup"><span data-stu-id="616be-123">Boolean</span></span>|<span data-ttu-id="616be-124">12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="616be-124">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="616be-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="616be-125">Relationships</span></span>
<span data-ttu-id="616be-126">无</span><span class="sxs-lookup"><span data-stu-id="616be-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="616be-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="616be-127">JSON Representation</span></span>
<span data-ttu-id="616be-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="616be-128">Here is a JSON representation of the resource.</span></span>
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



