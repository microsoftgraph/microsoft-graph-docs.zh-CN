---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a4b0860e05d20ea480f9c91264033f7a9eb41a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149166"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="05692-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="05692-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="05692-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05692-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05692-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05692-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05692-106">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="05692-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="05692-107">成员</span><span class="sxs-lookup"><span data-stu-id="05692-107">Members</span></span>
|<span data-ttu-id="05692-108">成员</span><span class="sxs-lookup"><span data-stu-id="05692-108">Member</span></span>|<span data-ttu-id="05692-109">值</span><span class="sxs-lookup"><span data-stu-id="05692-109">Value</span></span>|<span data-ttu-id="05692-110">说明</span><span class="sxs-lookup"><span data-stu-id="05692-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05692-111">定制</span><span class="sxs-lookup"><span data-stu-id="05692-111">userDefined</span></span>|<span data-ttu-id="05692-112">0</span><span class="sxs-lookup"><span data-stu-id="05692-112">0</span></span>|<span data-ttu-id="05692-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="05692-113">Allow the user to set.</span></span>|
|<span data-ttu-id="05692-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="05692-114">httpOnly</span></span>|<span data-ttu-id="05692-115">1</span><span class="sxs-lookup"><span data-stu-id="05692-115">1</span></span>|<span data-ttu-id="05692-116">仅限 HTTP, 无对等</span><span class="sxs-lookup"><span data-stu-id="05692-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="05692-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="05692-117">httpWithPeeringNat</span></span>|<span data-ttu-id="05692-118">双面</span><span class="sxs-lookup"><span data-stu-id="05692-118">2</span></span>|<span data-ttu-id="05692-119">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="05692-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="05692-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="05692-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="05692-121">第三章</span><span class="sxs-lookup"><span data-stu-id="05692-121">3</span></span>|<span data-ttu-id="05692-122">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="05692-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="05692-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="05692-123">httpWithInternetPeering</span></span>|<span data-ttu-id="05692-124">4</span><span class="sxs-lookup"><span data-stu-id="05692-124">4</span></span>|<span data-ttu-id="05692-125">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="05692-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="05692-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="05692-126">simpleDownload</span></span>|<span data-ttu-id="05692-127">99</span><span class="sxs-lookup"><span data-stu-id="05692-127">99</span></span>|<span data-ttu-id="05692-128">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="05692-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="05692-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="05692-129">bypassMode</span></span>|<span data-ttu-id="05692-130">100</span><span class="sxs-lookup"><span data-stu-id="05692-130">100</span></span>|<span data-ttu-id="05692-131">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="05692-131">Bypass mode.</span></span> <span data-ttu-id="05692-132">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="05692-132">Do not use Delivery Optimization and use BITS instead</span></span>|




