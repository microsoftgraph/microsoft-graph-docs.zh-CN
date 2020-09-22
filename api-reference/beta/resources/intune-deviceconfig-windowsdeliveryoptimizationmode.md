---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e3b32f3a6480b236297a7d0217c9aed8eefd5c44
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084455"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="b9567-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b9567-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="b9567-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9567-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9567-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9567-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9567-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9567-107">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="b9567-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="b9567-108">成员</span><span class="sxs-lookup"><span data-stu-id="b9567-108">Members</span></span>
|<span data-ttu-id="b9567-109">成员</span><span class="sxs-lookup"><span data-stu-id="b9567-109">Member</span></span>|<span data-ttu-id="b9567-110">值</span><span class="sxs-lookup"><span data-stu-id="b9567-110">Value</span></span>|<span data-ttu-id="b9567-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9567-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9567-112">定制</span><span class="sxs-lookup"><span data-stu-id="b9567-112">userDefined</span></span>|<span data-ttu-id="b9567-113">0</span><span class="sxs-lookup"><span data-stu-id="b9567-113">0</span></span>|<span data-ttu-id="b9567-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="b9567-114">Allow the user to set.</span></span>|
|<span data-ttu-id="b9567-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="b9567-115">httpOnly</span></span>|<span data-ttu-id="b9567-116">1 </span><span class="sxs-lookup"><span data-stu-id="b9567-116">1</span></span>|<span data-ttu-id="b9567-117">仅限 HTTP，无对等</span><span class="sxs-lookup"><span data-stu-id="b9567-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="b9567-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="b9567-118">httpWithPeeringNat</span></span>|<span data-ttu-id="b9567-119">2 </span><span class="sxs-lookup"><span data-stu-id="b9567-119">2</span></span>|<span data-ttu-id="b9567-120">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="b9567-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="b9567-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="b9567-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="b9567-122">第三章</span><span class="sxs-lookup"><span data-stu-id="b9567-122">3</span></span>|<span data-ttu-id="b9567-123">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="b9567-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="b9567-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="b9567-124">httpWithInternetPeering</span></span>|<span data-ttu-id="b9567-125">4 </span><span class="sxs-lookup"><span data-stu-id="b9567-125">4</span></span>|<span data-ttu-id="b9567-126">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="b9567-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="b9567-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="b9567-127">simpleDownload</span></span>|<span data-ttu-id="b9567-128">99</span><span class="sxs-lookup"><span data-stu-id="b9567-128">99</span></span>|<span data-ttu-id="b9567-129">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="b9567-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="b9567-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="b9567-130">bypassMode</span></span>|<span data-ttu-id="b9567-131">100</span><span class="sxs-lookup"><span data-stu-id="b9567-131">100</span></span>|<span data-ttu-id="b9567-132">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="b9567-132">Bypass mode.</span></span> <span data-ttu-id="b9567-133">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="b9567-133">Do not use Delivery Optimization and use BITS instead</span></span>|






