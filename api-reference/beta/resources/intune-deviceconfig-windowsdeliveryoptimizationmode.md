---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c24689f5690d3bd6d507c1ebb4fae36d010ee26d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268333"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="f04fd-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f04fd-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="f04fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f04fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f04fd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f04fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f04fd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f04fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f04fd-107">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="f04fd-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="f04fd-108">成员</span><span class="sxs-lookup"><span data-stu-id="f04fd-108">Members</span></span>
|<span data-ttu-id="f04fd-109">成员</span><span class="sxs-lookup"><span data-stu-id="f04fd-109">Member</span></span>|<span data-ttu-id="f04fd-110">值</span><span class="sxs-lookup"><span data-stu-id="f04fd-110">Value</span></span>|<span data-ttu-id="f04fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="f04fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f04fd-112">定制</span><span class="sxs-lookup"><span data-stu-id="f04fd-112">userDefined</span></span>|<span data-ttu-id="f04fd-113">0</span><span class="sxs-lookup"><span data-stu-id="f04fd-113">0</span></span>|<span data-ttu-id="f04fd-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="f04fd-114">Allow the user to set.</span></span>|
|<span data-ttu-id="f04fd-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="f04fd-115">httpOnly</span></span>|<span data-ttu-id="f04fd-116">1</span><span class="sxs-lookup"><span data-stu-id="f04fd-116">1</span></span>|<span data-ttu-id="f04fd-117">仅限 HTTP，无对等</span><span class="sxs-lookup"><span data-stu-id="f04fd-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="f04fd-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="f04fd-118">httpWithPeeringNat</span></span>|<span data-ttu-id="f04fd-119">双面</span><span class="sxs-lookup"><span data-stu-id="f04fd-119">2</span></span>|<span data-ttu-id="f04fd-120">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="f04fd-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="f04fd-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="f04fd-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="f04fd-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f04fd-122">3</span></span>|<span data-ttu-id="f04fd-123">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="f04fd-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="f04fd-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="f04fd-124">httpWithInternetPeering</span></span>|<span data-ttu-id="f04fd-125">4 </span><span class="sxs-lookup"><span data-stu-id="f04fd-125">4</span></span>|<span data-ttu-id="f04fd-126">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="f04fd-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="f04fd-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="f04fd-127">simpleDownload</span></span>|<span data-ttu-id="f04fd-128">99</span><span class="sxs-lookup"><span data-stu-id="f04fd-128">99</span></span>|<span data-ttu-id="f04fd-129">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="f04fd-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="f04fd-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="f04fd-130">bypassMode</span></span>|<span data-ttu-id="f04fd-131">100</span><span class="sxs-lookup"><span data-stu-id="f04fd-131">100</span></span>|<span data-ttu-id="f04fd-132">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="f04fd-132">Bypass mode.</span></span> <span data-ttu-id="f04fd-133">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="f04fd-133">Do not use Delivery Optimization and use BITS instead</span></span>|




