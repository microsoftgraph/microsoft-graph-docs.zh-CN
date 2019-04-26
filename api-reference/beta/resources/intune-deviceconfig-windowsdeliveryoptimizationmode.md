---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3872b7c09c8934e95725565b83cc195d9b9d8da5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554147"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="603a0-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="603a0-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="603a0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="603a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="603a0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="603a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="603a0-106">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="603a0-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="603a0-107">成员</span><span class="sxs-lookup"><span data-stu-id="603a0-107">Members</span></span>
|<span data-ttu-id="603a0-108">成员</span><span class="sxs-lookup"><span data-stu-id="603a0-108">Member</span></span>|<span data-ttu-id="603a0-109">值</span><span class="sxs-lookup"><span data-stu-id="603a0-109">Value</span></span>|<span data-ttu-id="603a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="603a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="603a0-111">定制</span><span class="sxs-lookup"><span data-stu-id="603a0-111">userDefined</span></span>|<span data-ttu-id="603a0-112">0</span><span class="sxs-lookup"><span data-stu-id="603a0-112">0</span></span>|<span data-ttu-id="603a0-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="603a0-113">Allow the user to set.</span></span>|
|<span data-ttu-id="603a0-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="603a0-114">httpOnly</span></span>|<span data-ttu-id="603a0-115">1</span><span class="sxs-lookup"><span data-stu-id="603a0-115">1</span></span>|<span data-ttu-id="603a0-116">仅限 HTTP, 无对等</span><span class="sxs-lookup"><span data-stu-id="603a0-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="603a0-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="603a0-117">httpWithPeeringNat</span></span>|<span data-ttu-id="603a0-118">2 </span><span class="sxs-lookup"><span data-stu-id="603a0-118">2</span></span>|<span data-ttu-id="603a0-119">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="603a0-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="603a0-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="603a0-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="603a0-121">3 </span><span class="sxs-lookup"><span data-stu-id="603a0-121">3</span></span>|<span data-ttu-id="603a0-122">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="603a0-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="603a0-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="603a0-123">httpWithInternetPeering</span></span>|<span data-ttu-id="603a0-124">4 </span><span class="sxs-lookup"><span data-stu-id="603a0-124">4</span></span>|<span data-ttu-id="603a0-125">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="603a0-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="603a0-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="603a0-126">simpleDownload</span></span>|<span data-ttu-id="603a0-127">99</span><span class="sxs-lookup"><span data-stu-id="603a0-127">99</span></span>|<span data-ttu-id="603a0-128">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="603a0-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="603a0-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="603a0-129">bypassMode</span></span>|<span data-ttu-id="603a0-130">100</span><span class="sxs-lookup"><span data-stu-id="603a0-130">100</span></span>|<span data-ttu-id="603a0-131">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="603a0-131">Bypass mode.</span></span> <span data-ttu-id="603a0-132">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="603a0-132">Do not use Delivery Optimization and use BITS instead</span></span>|





