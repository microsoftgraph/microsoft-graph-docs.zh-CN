---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e62416328e596737c36d920d6877773c905680c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807719"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="d3af4-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d3af4-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="d3af4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d3af4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3af4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d3af4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3af4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d3af4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3af4-107">对等方通讯组的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="d3af4-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="d3af4-108">成员</span><span class="sxs-lookup"><span data-stu-id="d3af4-108">Members</span></span>
|<span data-ttu-id="d3af4-109">成员</span><span class="sxs-lookup"><span data-stu-id="d3af4-109">Member</span></span>|<span data-ttu-id="d3af4-110">值</span><span class="sxs-lookup"><span data-stu-id="d3af4-110">Value</span></span>|<span data-ttu-id="d3af4-111">Description</span><span class="sxs-lookup"><span data-stu-id="d3af4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3af4-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="d3af4-112">userDefined</span></span>|<span data-ttu-id="d3af4-113">0</span><span class="sxs-lookup"><span data-stu-id="d3af4-113">0</span></span>|<span data-ttu-id="d3af4-114">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="d3af4-114">Allow the user to set.</span></span>|
|<span data-ttu-id="d3af4-115">为 httpOnly</span><span class="sxs-lookup"><span data-stu-id="d3af4-115">httpOnly</span></span>|<span data-ttu-id="d3af4-116">1</span><span class="sxs-lookup"><span data-stu-id="d3af4-116">1</span></span>|<span data-ttu-id="d3af4-117">HTTP 仅，没有对等</span><span class="sxs-lookup"><span data-stu-id="d3af4-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="d3af4-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="d3af4-118">httpWithPeeringNat</span></span>|<span data-ttu-id="d3af4-119">2</span><span class="sxs-lookup"><span data-stu-id="d3af4-119">2</span></span>|<span data-ttu-id="d3af4-120">与同一个网络地址转换器后面对等的 OS 默认 – Http 混合</span><span class="sxs-lookup"><span data-stu-id="d3af4-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="d3af4-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="d3af4-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="d3af4-122">3</span><span class="sxs-lookup"><span data-stu-id="d3af4-122">3</span></span>|<span data-ttu-id="d3af4-123">HTTP 与跨专用组对等混合</span><span class="sxs-lookup"><span data-stu-id="d3af4-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="d3af4-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="d3af4-124">httpWithInternetPeering</span></span>|<span data-ttu-id="d3af4-125">4</span><span class="sxs-lookup"><span data-stu-id="d3af4-125">4</span></span>|<span data-ttu-id="d3af4-126">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="d3af4-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="d3af4-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="d3af4-127">simpleDownload</span></span>|<span data-ttu-id="d3af4-128">99</span><span class="sxs-lookup"><span data-stu-id="d3af4-128">99</span></span>|<span data-ttu-id="d3af4-129">与没有对等的简单 download 模式</span><span class="sxs-lookup"><span data-stu-id="d3af4-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="d3af4-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="d3af4-130">bypassMode</span></span>|<span data-ttu-id="d3af4-131">100</span><span class="sxs-lookup"><span data-stu-id="d3af4-131">100</span></span>|<span data-ttu-id="d3af4-132">绕过模式。</span><span class="sxs-lookup"><span data-stu-id="d3af4-132">Bypass mode.</span></span> <span data-ttu-id="d3af4-133">不使用传递优化并改用位</span><span class="sxs-lookup"><span data-stu-id="d3af4-133">Do not use Delivery Optimization and use BITS instead</span></span>|





