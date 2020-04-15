---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等分发的传递优化模式
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9be3f6861076bed1ef2e6d45336d975c07cba576
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451485"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="04456-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="04456-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="04456-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04456-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04456-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04456-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04456-106">对等分发的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="04456-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="04456-107">成员</span><span class="sxs-lookup"><span data-stu-id="04456-107">Members</span></span>
|<span data-ttu-id="04456-108">成员</span><span class="sxs-lookup"><span data-stu-id="04456-108">Member</span></span>|<span data-ttu-id="04456-109">值</span><span class="sxs-lookup"><span data-stu-id="04456-109">Value</span></span>|<span data-ttu-id="04456-110">说明</span><span class="sxs-lookup"><span data-stu-id="04456-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04456-111">定制</span><span class="sxs-lookup"><span data-stu-id="04456-111">userDefined</span></span>|<span data-ttu-id="04456-112">0</span><span class="sxs-lookup"><span data-stu-id="04456-112">0</span></span>|<span data-ttu-id="04456-113">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="04456-113">Allow the user to set.</span></span>|
|<span data-ttu-id="04456-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="04456-114">httpOnly</span></span>|<span data-ttu-id="04456-115">1</span><span class="sxs-lookup"><span data-stu-id="04456-115">1</span></span>|<span data-ttu-id="04456-116">仅限 HTTP，无对等</span><span class="sxs-lookup"><span data-stu-id="04456-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="04456-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="04456-117">httpWithPeeringNat</span></span>|<span data-ttu-id="04456-118">双面</span><span class="sxs-lookup"><span data-stu-id="04456-118">2</span></span>|<span data-ttu-id="04456-119">OS 默认值–在同一网络地址转换器后具有对等的 Http 混合</span><span class="sxs-lookup"><span data-stu-id="04456-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="04456-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="04456-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="04456-121">第三章</span><span class="sxs-lookup"><span data-stu-id="04456-121">3</span></span>|<span data-ttu-id="04456-122">通过专用组与对等互连的 HTTP 混合</span><span class="sxs-lookup"><span data-stu-id="04456-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="04456-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="04456-123">httpWithInternetPeering</span></span>|<span data-ttu-id="04456-124">4 </span><span class="sxs-lookup"><span data-stu-id="04456-124">4</span></span>|<span data-ttu-id="04456-125">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="04456-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="04456-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="04456-126">simpleDownload</span></span>|<span data-ttu-id="04456-127">99</span><span class="sxs-lookup"><span data-stu-id="04456-127">99</span></span>|<span data-ttu-id="04456-128">无对等的简单下载模式</span><span class="sxs-lookup"><span data-stu-id="04456-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="04456-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="04456-129">bypassMode</span></span>|<span data-ttu-id="04456-130">100</span><span class="sxs-lookup"><span data-stu-id="04456-130">100</span></span>|<span data-ttu-id="04456-131">旁路模式。</span><span class="sxs-lookup"><span data-stu-id="04456-131">Bypass mode.</span></span> <span data-ttu-id="04456-132">请勿使用传递优化和改用 BITS</span><span class="sxs-lookup"><span data-stu-id="04456-132">Do not use Delivery Optimization and use BITS instead</span></span>|







