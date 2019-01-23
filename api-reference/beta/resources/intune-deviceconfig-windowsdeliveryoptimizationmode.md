---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5565965f9ba9395d7cd07b2935e6772478e0bb50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406883"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="11747-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="11747-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="11747-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="11747-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11747-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="11747-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11747-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11747-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11747-107">对等方通讯组的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="11747-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="11747-108">成员</span><span class="sxs-lookup"><span data-stu-id="11747-108">Members</span></span>
|<span data-ttu-id="11747-109">成员</span><span class="sxs-lookup"><span data-stu-id="11747-109">Member</span></span>|<span data-ttu-id="11747-110">值</span><span class="sxs-lookup"><span data-stu-id="11747-110">Value</span></span>|<span data-ttu-id="11747-111">说明</span><span class="sxs-lookup"><span data-stu-id="11747-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11747-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="11747-112">userDefined</span></span>|<span data-ttu-id="11747-113">0</span><span class="sxs-lookup"><span data-stu-id="11747-113">0</span></span>|<span data-ttu-id="11747-114">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="11747-114">Allow the user to set.</span></span>|
|<span data-ttu-id="11747-115">为 httpOnly</span><span class="sxs-lookup"><span data-stu-id="11747-115">httpOnly</span></span>|<span data-ttu-id="11747-116">1</span><span class="sxs-lookup"><span data-stu-id="11747-116">1</span></span>|<span data-ttu-id="11747-117">HTTP 仅，没有对等</span><span class="sxs-lookup"><span data-stu-id="11747-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="11747-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="11747-118">httpWithPeeringNat</span></span>|<span data-ttu-id="11747-119">2</span><span class="sxs-lookup"><span data-stu-id="11747-119">2</span></span>|<span data-ttu-id="11747-120">与同一个网络地址转换器后面对等的 OS 默认 – Http 混合</span><span class="sxs-lookup"><span data-stu-id="11747-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="11747-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="11747-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="11747-122">3</span><span class="sxs-lookup"><span data-stu-id="11747-122">3</span></span>|<span data-ttu-id="11747-123">HTTP 与跨专用组对等混合</span><span class="sxs-lookup"><span data-stu-id="11747-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="11747-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="11747-124">httpWithInternetPeering</span></span>|<span data-ttu-id="11747-125">4</span><span class="sxs-lookup"><span data-stu-id="11747-125">4</span></span>|<span data-ttu-id="11747-126">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="11747-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="11747-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="11747-127">simpleDownload</span></span>|<span data-ttu-id="11747-128">99</span><span class="sxs-lookup"><span data-stu-id="11747-128">99</span></span>|<span data-ttu-id="11747-129">与没有对等的简单 download 模式</span><span class="sxs-lookup"><span data-stu-id="11747-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="11747-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="11747-130">bypassMode</span></span>|<span data-ttu-id="11747-131">100</span><span class="sxs-lookup"><span data-stu-id="11747-131">100</span></span>|<span data-ttu-id="11747-132">绕过模式。</span><span class="sxs-lookup"><span data-stu-id="11747-132">Bypass mode.</span></span> <span data-ttu-id="11747-133">不使用传递优化并改用位</span><span class="sxs-lookup"><span data-stu-id="11747-133">Do not use Delivery Optimization and use BITS instead</span></span>|




