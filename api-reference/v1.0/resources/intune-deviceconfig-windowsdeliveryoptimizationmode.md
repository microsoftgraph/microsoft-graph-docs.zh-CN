---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5c483f00817858e7061bacf1b1e2b6ec6c00a02b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742746"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="0d17b-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0d17b-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="0d17b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d17b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d17b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d17b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d17b-106">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="0d17b-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="0d17b-107">成员</span><span class="sxs-lookup"><span data-stu-id="0d17b-107">Members</span></span>
|<span data-ttu-id="0d17b-108">成员</span><span class="sxs-lookup"><span data-stu-id="0d17b-108">Member</span></span>|<span data-ttu-id="0d17b-109">值</span><span class="sxs-lookup"><span data-stu-id="0d17b-109">Value</span></span>|<span data-ttu-id="0d17b-110">Description</span><span class="sxs-lookup"><span data-stu-id="0d17b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d17b-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="0d17b-111">userDefined</span></span>|<span data-ttu-id="0d17b-112">0</span><span class="sxs-lookup"><span data-stu-id="0d17b-112">0</span></span>|<span data-ttu-id="0d17b-113">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="0d17b-113">Allow the user to set.</span></span>|
|<span data-ttu-id="0d17b-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="0d17b-114">httpOnly</span></span>|<span data-ttu-id="0d17b-115">1</span><span class="sxs-lookup"><span data-stu-id="0d17b-115">1</span></span>|<span data-ttu-id="0d17b-116">仅 HTTP，无对等</span><span class="sxs-lookup"><span data-stu-id="0d17b-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="0d17b-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="0d17b-117">httpWithPeeringNat</span></span>|<span data-ttu-id="0d17b-118">2</span><span class="sxs-lookup"><span data-stu-id="0d17b-118">2</span></span>|<span data-ttu-id="0d17b-119">操作系统默认值 – Http 与同一网络地址转换器后的对等混合</span><span class="sxs-lookup"><span data-stu-id="0d17b-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="0d17b-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="0d17b-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="0d17b-121">3</span><span class="sxs-lookup"><span data-stu-id="0d17b-121">3</span></span>|<span data-ttu-id="0d17b-122">通过专用组对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="0d17b-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="0d17b-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="0d17b-123">httpWithInternetPeering</span></span>|<span data-ttu-id="0d17b-124">4 </span><span class="sxs-lookup"><span data-stu-id="0d17b-124">4</span></span>|<span data-ttu-id="0d17b-125">HTTP 与 Internet 对等混合</span><span class="sxs-lookup"><span data-stu-id="0d17b-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="0d17b-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="0d17b-126">simpleDownload</span></span>|<span data-ttu-id="0d17b-127">99</span><span class="sxs-lookup"><span data-stu-id="0d17b-127">99</span></span>|<span data-ttu-id="0d17b-128">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="0d17b-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="0d17b-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="0d17b-129">bypassMode</span></span>|<span data-ttu-id="0d17b-130">100</span><span class="sxs-lookup"><span data-stu-id="0d17b-130">100</span></span>|<span data-ttu-id="0d17b-131">绕过模式。</span><span class="sxs-lookup"><span data-stu-id="0d17b-131">Bypass mode.</span></span> <span data-ttu-id="0d17b-132">请勿使用传递优化并改为使用 BITS</span><span class="sxs-lookup"><span data-stu-id="0d17b-132">Do not use Delivery Optimization and use BITS instead</span></span>|




