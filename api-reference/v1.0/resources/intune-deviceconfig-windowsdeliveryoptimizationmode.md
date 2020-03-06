---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 869c902e8fc0b02fed1037d1d1273d8584ece9fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530367"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="f1d27-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f1d27-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="f1d27-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1d27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1d27-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1d27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1d27-106">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="f1d27-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="f1d27-107">成员</span><span class="sxs-lookup"><span data-stu-id="f1d27-107">Members</span></span>
|<span data-ttu-id="f1d27-108">成员</span><span class="sxs-lookup"><span data-stu-id="f1d27-108">Member</span></span>|<span data-ttu-id="f1d27-109">值</span><span class="sxs-lookup"><span data-stu-id="f1d27-109">Value</span></span>|<span data-ttu-id="f1d27-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1d27-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1d27-111">定制</span><span class="sxs-lookup"><span data-stu-id="f1d27-111">userDefined</span></span>|<span data-ttu-id="f1d27-112">0</span><span class="sxs-lookup"><span data-stu-id="f1d27-112">0</span></span>|<span data-ttu-id="f1d27-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="f1d27-113">Allow the user to set.</span></span>|
|<span data-ttu-id="f1d27-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="f1d27-114">httpOnly</span></span>|<span data-ttu-id="f1d27-115">1 </span><span class="sxs-lookup"><span data-stu-id="f1d27-115">1</span></span>|<span data-ttu-id="f1d27-116">仅限 HTTP，无对等</span><span class="sxs-lookup"><span data-stu-id="f1d27-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="f1d27-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="f1d27-117">httpWithPeeringNat</span></span>|<span data-ttu-id="f1d27-118">2 </span><span class="sxs-lookup"><span data-stu-id="f1d27-118">2</span></span>|<span data-ttu-id="f1d27-119">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="f1d27-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="f1d27-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="f1d27-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="f1d27-121">3 </span><span class="sxs-lookup"><span data-stu-id="f1d27-121">3</span></span>|<span data-ttu-id="f1d27-122">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="f1d27-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="f1d27-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="f1d27-123">httpWithInternetPeering</span></span>|<span data-ttu-id="f1d27-124">4 </span><span class="sxs-lookup"><span data-stu-id="f1d27-124">4</span></span>|<span data-ttu-id="f1d27-125">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="f1d27-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="f1d27-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="f1d27-126">simpleDownload</span></span>|<span data-ttu-id="f1d27-127">99</span><span class="sxs-lookup"><span data-stu-id="f1d27-127">99</span></span>|<span data-ttu-id="f1d27-128">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="f1d27-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="f1d27-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="f1d27-129">bypassMode</span></span>|<span data-ttu-id="f1d27-130">100</span><span class="sxs-lookup"><span data-stu-id="f1d27-130">100</span></span>|<span data-ttu-id="f1d27-131">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="f1d27-131">Bypass mode.</span></span> <span data-ttu-id="f1d27-132">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="f1d27-132">Do not use Delivery Optimization and use BITS instead</span></span>|




