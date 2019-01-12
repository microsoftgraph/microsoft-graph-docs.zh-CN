---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f80c6b5cbe7316c851954154bdb559f370f02b79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951514"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="64e9e-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="64e9e-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="64e9e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="64e9e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64e9e-105">对等方通讯组的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="64e9e-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="64e9e-106">成员</span><span class="sxs-lookup"><span data-stu-id="64e9e-106">Members</span></span>
|<span data-ttu-id="64e9e-107">成员</span><span class="sxs-lookup"><span data-stu-id="64e9e-107">Member</span></span>|<span data-ttu-id="64e9e-108">值</span><span class="sxs-lookup"><span data-stu-id="64e9e-108">Value</span></span>|<span data-ttu-id="64e9e-109">说明</span><span class="sxs-lookup"><span data-stu-id="64e9e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e9e-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="64e9e-110">userDefined</span></span>|<span data-ttu-id="64e9e-111">0</span><span class="sxs-lookup"><span data-stu-id="64e9e-111">0</span></span>|<span data-ttu-id="64e9e-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="64e9e-112">Allow the user to set.</span></span>|
|<span data-ttu-id="64e9e-113">为 httpOnly</span><span class="sxs-lookup"><span data-stu-id="64e9e-113">httpOnly</span></span>|<span data-ttu-id="64e9e-114">1</span><span class="sxs-lookup"><span data-stu-id="64e9e-114">1</span></span>|<span data-ttu-id="64e9e-115">HTTP 仅，没有对等</span><span class="sxs-lookup"><span data-stu-id="64e9e-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="64e9e-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="64e9e-116">httpWithPeeringNat</span></span>|<span data-ttu-id="64e9e-117">2</span><span class="sxs-lookup"><span data-stu-id="64e9e-117">2</span></span>|<span data-ttu-id="64e9e-118">与同一个网络地址转换器后面对等的 OS 默认 – Http 混合</span><span class="sxs-lookup"><span data-stu-id="64e9e-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="64e9e-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="64e9e-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="64e9e-120">3</span><span class="sxs-lookup"><span data-stu-id="64e9e-120">3</span></span>|<span data-ttu-id="64e9e-121">HTTP 与跨专用组对等混合</span><span class="sxs-lookup"><span data-stu-id="64e9e-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="64e9e-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="64e9e-122">httpWithInternetPeering</span></span>|<span data-ttu-id="64e9e-123">4</span><span class="sxs-lookup"><span data-stu-id="64e9e-123">4</span></span>|<span data-ttu-id="64e9e-124">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="64e9e-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="64e9e-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="64e9e-125">simpleDownload</span></span>|<span data-ttu-id="64e9e-126">99</span><span class="sxs-lookup"><span data-stu-id="64e9e-126">99</span></span>|<span data-ttu-id="64e9e-127">与没有对等的简单 download 模式</span><span class="sxs-lookup"><span data-stu-id="64e9e-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="64e9e-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="64e9e-128">bypassMode</span></span>|<span data-ttu-id="64e9e-129">100</span><span class="sxs-lookup"><span data-stu-id="64e9e-129">100</span></span>|<span data-ttu-id="64e9e-130">绕过模式。</span><span class="sxs-lookup"><span data-stu-id="64e9e-130">Bypass mode.</span></span> <span data-ttu-id="64e9e-131">不使用传递优化并改用位</span><span class="sxs-lookup"><span data-stu-id="64e9e-131">Do not use Delivery Optimization and use BITS instead</span></span>|



