---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251501"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="9cf03-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9cf03-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="9cf03-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9cf03-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf03-105">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="9cf03-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="9cf03-106">成员</span><span class="sxs-lookup"><span data-stu-id="9cf03-106">Members</span></span>
|<span data-ttu-id="9cf03-107">成员</span><span class="sxs-lookup"><span data-stu-id="9cf03-107">Member</span></span>|<span data-ttu-id="9cf03-108">值</span><span class="sxs-lookup"><span data-stu-id="9cf03-108">Value</span></span>|<span data-ttu-id="9cf03-109">说明</span><span class="sxs-lookup"><span data-stu-id="9cf03-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cf03-110">定制</span><span class="sxs-lookup"><span data-stu-id="9cf03-110">userDefined</span></span>|<span data-ttu-id="9cf03-111">0</span><span class="sxs-lookup"><span data-stu-id="9cf03-111">0</span></span>|<span data-ttu-id="9cf03-112">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="9cf03-112">Allow the user to set.</span></span>|
|<span data-ttu-id="9cf03-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="9cf03-113">httpOnly</span></span>|<span data-ttu-id="9cf03-114">1</span><span class="sxs-lookup"><span data-stu-id="9cf03-114">1</span></span>|<span data-ttu-id="9cf03-115">仅限 HTTP, 无对等</span><span class="sxs-lookup"><span data-stu-id="9cf03-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="9cf03-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="9cf03-116">httpWithPeeringNat</span></span>|<span data-ttu-id="9cf03-117">双面</span><span class="sxs-lookup"><span data-stu-id="9cf03-117">2</span></span>|<span data-ttu-id="9cf03-118">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="9cf03-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="9cf03-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="9cf03-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="9cf03-120">第三章</span><span class="sxs-lookup"><span data-stu-id="9cf03-120">3</span></span>|<span data-ttu-id="9cf03-121">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="9cf03-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="9cf03-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="9cf03-122">httpWithInternetPeering</span></span>|<span data-ttu-id="9cf03-123">4</span><span class="sxs-lookup"><span data-stu-id="9cf03-123">4</span></span>|<span data-ttu-id="9cf03-124">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="9cf03-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="9cf03-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="9cf03-125">simpleDownload</span></span>|<span data-ttu-id="9cf03-126">99</span><span class="sxs-lookup"><span data-stu-id="9cf03-126">99</span></span>|<span data-ttu-id="9cf03-127">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="9cf03-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="9cf03-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="9cf03-128">bypassMode</span></span>|<span data-ttu-id="9cf03-129">100</span><span class="sxs-lookup"><span data-stu-id="9cf03-129">100</span></span>|<span data-ttu-id="9cf03-130">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="9cf03-130">Bypass mode.</span></span> <span data-ttu-id="9cf03-131">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="9cf03-131">Do not use Delivery Optimization and use BITS instead</span></span>|



