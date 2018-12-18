---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
author: tfitzmac
ms.openlocfilehash: b23bdc80bd8b1fb151f9e138e1a1802140455c4e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333479"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="b984c-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b984c-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="b984c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b984c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b984c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b984c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b984c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b984c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b984c-107">对等方通讯组的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="b984c-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="b984c-108">成员</span><span class="sxs-lookup"><span data-stu-id="b984c-108">Members</span></span>
|<span data-ttu-id="b984c-109">成员</span><span class="sxs-lookup"><span data-stu-id="b984c-109">Member</span></span>|<span data-ttu-id="b984c-110">值</span><span class="sxs-lookup"><span data-stu-id="b984c-110">Value</span></span>|<span data-ttu-id="b984c-111">说明</span><span class="sxs-lookup"><span data-stu-id="b984c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b984c-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="b984c-112">userDefined</span></span>|<span data-ttu-id="b984c-113">0</span><span class="sxs-lookup"><span data-stu-id="b984c-113">0</span></span>|<span data-ttu-id="b984c-114">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="b984c-114">Allow the user to set.</span></span>|
|<span data-ttu-id="b984c-115">为 httpOnly</span><span class="sxs-lookup"><span data-stu-id="b984c-115">httpOnly</span></span>|<span data-ttu-id="b984c-116">1</span><span class="sxs-lookup"><span data-stu-id="b984c-116">1</span></span>|<span data-ttu-id="b984c-117">HTTP 仅，没有对等</span><span class="sxs-lookup"><span data-stu-id="b984c-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="b984c-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="b984c-118">httpWithPeeringNat</span></span>|<span data-ttu-id="b984c-119">2</span><span class="sxs-lookup"><span data-stu-id="b984c-119">2</span></span>|<span data-ttu-id="b984c-120">与同一个网络地址转换器后面对等的 OS 默认 – Http 混合</span><span class="sxs-lookup"><span data-stu-id="b984c-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="b984c-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="b984c-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="b984c-122">3</span><span class="sxs-lookup"><span data-stu-id="b984c-122">3</span></span>|<span data-ttu-id="b984c-123">HTTP 与跨专用组对等混合</span><span class="sxs-lookup"><span data-stu-id="b984c-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="b984c-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="b984c-124">httpWithInternetPeering</span></span>|<span data-ttu-id="b984c-125">4</span><span class="sxs-lookup"><span data-stu-id="b984c-125">4</span></span>|<span data-ttu-id="b984c-126">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="b984c-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="b984c-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="b984c-127">simpleDownload</span></span>|<span data-ttu-id="b984c-128">99</span><span class="sxs-lookup"><span data-stu-id="b984c-128">99</span></span>|<span data-ttu-id="b984c-129">与没有对等的简单 download 模式</span><span class="sxs-lookup"><span data-stu-id="b984c-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="b984c-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="b984c-130">bypassMode</span></span>|<span data-ttu-id="b984c-131">100</span><span class="sxs-lookup"><span data-stu-id="b984c-131">100</span></span>|<span data-ttu-id="b984c-132">绕过模式。</span><span class="sxs-lookup"><span data-stu-id="b984c-132">Bypass mode.</span></span> <span data-ttu-id="b984c-133">不使用传递优化并改用位</span><span class="sxs-lookup"><span data-stu-id="b984c-133">Do not use Delivery Optimization and use BITS instead</span></span>|





