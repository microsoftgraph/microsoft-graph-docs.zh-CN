---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af266b55fd58f788965d33d0d807511d263f6195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888177"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="e1380-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e1380-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="e1380-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1380-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1380-105">对等方通讯组的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="e1380-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="e1380-106">成员</span><span class="sxs-lookup"><span data-stu-id="e1380-106">Members</span></span>
|<span data-ttu-id="e1380-107">成员</span><span class="sxs-lookup"><span data-stu-id="e1380-107">Member</span></span>|<span data-ttu-id="e1380-108">值</span><span class="sxs-lookup"><span data-stu-id="e1380-108">Value</span></span>|<span data-ttu-id="e1380-109">Description</span><span class="sxs-lookup"><span data-stu-id="e1380-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1380-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="e1380-110">userDefined</span></span>|<span data-ttu-id="e1380-111">0</span><span class="sxs-lookup"><span data-stu-id="e1380-111">0</span></span>|<span data-ttu-id="e1380-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="e1380-112">Allow the user to set.</span></span>|
|<span data-ttu-id="e1380-113">为 httpOnly</span><span class="sxs-lookup"><span data-stu-id="e1380-113">httpOnly</span></span>|<span data-ttu-id="e1380-114">1</span><span class="sxs-lookup"><span data-stu-id="e1380-114">1</span></span>|<span data-ttu-id="e1380-115">HTTP 仅，没有对等</span><span class="sxs-lookup"><span data-stu-id="e1380-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="e1380-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="e1380-116">httpWithPeeringNat</span></span>|<span data-ttu-id="e1380-117">2</span><span class="sxs-lookup"><span data-stu-id="e1380-117">2</span></span>|<span data-ttu-id="e1380-118">与同一个网络地址转换器后面对等的 OS 默认 – Http 混合</span><span class="sxs-lookup"><span data-stu-id="e1380-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="e1380-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="e1380-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="e1380-120">3</span><span class="sxs-lookup"><span data-stu-id="e1380-120">3</span></span>|<span data-ttu-id="e1380-121">HTTP 与跨专用组对等混合</span><span class="sxs-lookup"><span data-stu-id="e1380-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="e1380-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="e1380-122">httpWithInternetPeering</span></span>|<span data-ttu-id="e1380-123">4</span><span class="sxs-lookup"><span data-stu-id="e1380-123">4</span></span>|<span data-ttu-id="e1380-124">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="e1380-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="e1380-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="e1380-125">simpleDownload</span></span>|<span data-ttu-id="e1380-126">99</span><span class="sxs-lookup"><span data-stu-id="e1380-126">99</span></span>|<span data-ttu-id="e1380-127">与没有对等的简单 download 模式</span><span class="sxs-lookup"><span data-stu-id="e1380-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="e1380-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="e1380-128">bypassMode</span></span>|<span data-ttu-id="e1380-129">100</span><span class="sxs-lookup"><span data-stu-id="e1380-129">100</span></span>|<span data-ttu-id="e1380-130">绕过模式。</span><span class="sxs-lookup"><span data-stu-id="e1380-130">Bypass mode.</span></span> <span data-ttu-id="e1380-131">不使用传递优化并改用位</span><span class="sxs-lookup"><span data-stu-id="e1380-131">Do not use Delivery Optimization and use BITS instead</span></span>|



