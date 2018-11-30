---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
ms.openlocfilehash: 2d393a82f855f3e3a0226c8ccb450fa2dae1a95c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009017"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="14a86-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="14a86-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="14a86-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="14a86-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14a86-105">对等方通讯组的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="14a86-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="14a86-106">成员</span><span class="sxs-lookup"><span data-stu-id="14a86-106">Members</span></span>
|<span data-ttu-id="14a86-107">成员</span><span class="sxs-lookup"><span data-stu-id="14a86-107">Member</span></span>|<span data-ttu-id="14a86-108">值</span><span class="sxs-lookup"><span data-stu-id="14a86-108">Value</span></span>|<span data-ttu-id="14a86-109">说明</span><span class="sxs-lookup"><span data-stu-id="14a86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14a86-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="14a86-110">userDefined</span></span>|<span data-ttu-id="14a86-111">0</span><span class="sxs-lookup"><span data-stu-id="14a86-111">0</span></span>|<span data-ttu-id="14a86-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="14a86-112">Allow the user to set.</span></span>|
|<span data-ttu-id="14a86-113">为 httpOnly</span><span class="sxs-lookup"><span data-stu-id="14a86-113">httpOnly</span></span>|<span data-ttu-id="14a86-114">1</span><span class="sxs-lookup"><span data-stu-id="14a86-114">1</span></span>|<span data-ttu-id="14a86-115">HTTP 仅，没有对等</span><span class="sxs-lookup"><span data-stu-id="14a86-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="14a86-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="14a86-116">httpWithPeeringNat</span></span>|<span data-ttu-id="14a86-117">2</span><span class="sxs-lookup"><span data-stu-id="14a86-117">2</span></span>|<span data-ttu-id="14a86-118">与同一个网络地址转换器后面对等的 OS 默认 – Http 混合</span><span class="sxs-lookup"><span data-stu-id="14a86-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="14a86-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="14a86-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="14a86-120">3</span><span class="sxs-lookup"><span data-stu-id="14a86-120">3</span></span>|<span data-ttu-id="14a86-121">HTTP 与跨专用组对等混合</span><span class="sxs-lookup"><span data-stu-id="14a86-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="14a86-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="14a86-122">httpWithInternetPeering</span></span>|<span data-ttu-id="14a86-123">4</span><span class="sxs-lookup"><span data-stu-id="14a86-123">4</span></span>|<span data-ttu-id="14a86-124">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="14a86-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="14a86-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="14a86-125">simpleDownload</span></span>|<span data-ttu-id="14a86-126">99</span><span class="sxs-lookup"><span data-stu-id="14a86-126">99</span></span>|<span data-ttu-id="14a86-127">与没有对等的简单 download 模式</span><span class="sxs-lookup"><span data-stu-id="14a86-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="14a86-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="14a86-128">bypassMode</span></span>|<span data-ttu-id="14a86-129">100</span><span class="sxs-lookup"><span data-stu-id="14a86-129">100</span></span>|<span data-ttu-id="14a86-130">绕过模式。</span><span class="sxs-lookup"><span data-stu-id="14a86-130">Bypass mode.</span></span> <span data-ttu-id="14a86-131">不使用传递优化并改用位</span><span class="sxs-lookup"><span data-stu-id="14a86-131">Do not use Delivery Optimization and use BITS instead</span></span>|



