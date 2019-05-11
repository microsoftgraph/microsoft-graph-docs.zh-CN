---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e020b4f32cc9075acab6c783b4e9df3eb19a438b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944122"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="9e576-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9e576-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="9e576-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e576-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e576-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e576-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e576-106">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="9e576-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="9e576-107">成员</span><span class="sxs-lookup"><span data-stu-id="9e576-107">Members</span></span>
|<span data-ttu-id="9e576-108">成员</span><span class="sxs-lookup"><span data-stu-id="9e576-108">Member</span></span>|<span data-ttu-id="9e576-109">值</span><span class="sxs-lookup"><span data-stu-id="9e576-109">Value</span></span>|<span data-ttu-id="9e576-110">说明</span><span class="sxs-lookup"><span data-stu-id="9e576-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e576-111">定制</span><span class="sxs-lookup"><span data-stu-id="9e576-111">userDefined</span></span>|<span data-ttu-id="9e576-112">0</span><span class="sxs-lookup"><span data-stu-id="9e576-112">0</span></span>|<span data-ttu-id="9e576-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="9e576-113">Allow the user to set.</span></span>|
|<span data-ttu-id="9e576-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="9e576-114">httpOnly</span></span>|<span data-ttu-id="9e576-115">1</span><span class="sxs-lookup"><span data-stu-id="9e576-115">1</span></span>|<span data-ttu-id="9e576-116">仅限 HTTP, 无对等</span><span class="sxs-lookup"><span data-stu-id="9e576-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="9e576-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="9e576-117">httpWithPeeringNat</span></span>|<span data-ttu-id="9e576-118">双面</span><span class="sxs-lookup"><span data-stu-id="9e576-118">2</span></span>|<span data-ttu-id="9e576-119">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="9e576-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="9e576-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="9e576-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="9e576-121">第三章</span><span class="sxs-lookup"><span data-stu-id="9e576-121">3</span></span>|<span data-ttu-id="9e576-122">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="9e576-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="9e576-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="9e576-123">httpWithInternetPeering</span></span>|<span data-ttu-id="9e576-124">4</span><span class="sxs-lookup"><span data-stu-id="9e576-124">4</span></span>|<span data-ttu-id="9e576-125">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="9e576-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="9e576-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="9e576-126">simpleDownload</span></span>|<span data-ttu-id="9e576-127">99</span><span class="sxs-lookup"><span data-stu-id="9e576-127">99</span></span>|<span data-ttu-id="9e576-128">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="9e576-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="9e576-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="9e576-129">bypassMode</span></span>|<span data-ttu-id="9e576-130">100</span><span class="sxs-lookup"><span data-stu-id="9e576-130">100</span></span>|<span data-ttu-id="9e576-131">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="9e576-131">Bypass mode.</span></span> <span data-ttu-id="9e576-132">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="9e576-132">Do not use Delivery Optimization and use BITS instead</span></span>|




