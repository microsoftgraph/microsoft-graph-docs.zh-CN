---
title: windowsDeliveryOptimizationMode 枚举类型
description: 对等方通讯组的传递优化模式
author: tfitzmac
ms.openlocfilehash: ae61d7dde5fc02ff329eaf9cc970ee7078c3a254
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360156"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="8bbd5-103">windowsDeliveryOptimizationMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8bbd5-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="8bbd5-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8bbd5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bbd5-105">对等方通讯组的传递优化模式</span><span class="sxs-lookup"><span data-stu-id="8bbd5-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="8bbd5-106">成员</span><span class="sxs-lookup"><span data-stu-id="8bbd5-106">Members</span></span>
|<span data-ttu-id="8bbd5-107">成员</span><span class="sxs-lookup"><span data-stu-id="8bbd5-107">Member</span></span>|<span data-ttu-id="8bbd5-108">值</span><span class="sxs-lookup"><span data-stu-id="8bbd5-108">Value</span></span>|<span data-ttu-id="8bbd5-109">说明</span><span class="sxs-lookup"><span data-stu-id="8bbd5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bbd5-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="8bbd5-110">userDefined</span></span>|<span data-ttu-id="8bbd5-111">0</span><span class="sxs-lookup"><span data-stu-id="8bbd5-111">0</span></span>|<span data-ttu-id="8bbd5-112">允许用户设置。</span><span class="sxs-lookup"><span data-stu-id="8bbd5-112">Allow the user to set.</span></span>|
|<span data-ttu-id="8bbd5-113">为 httpOnly</span><span class="sxs-lookup"><span data-stu-id="8bbd5-113">httpOnly</span></span>|<span data-ttu-id="8bbd5-114">1</span><span class="sxs-lookup"><span data-stu-id="8bbd5-114">1</span></span>|<span data-ttu-id="8bbd5-115">HTTP 仅，没有对等</span><span class="sxs-lookup"><span data-stu-id="8bbd5-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="8bbd5-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="8bbd5-116">httpWithPeeringNat</span></span>|<span data-ttu-id="8bbd5-117">2</span><span class="sxs-lookup"><span data-stu-id="8bbd5-117">2</span></span>|<span data-ttu-id="8bbd5-118">与同一个网络地址转换器后面对等的 OS 默认 – Http 混合</span><span class="sxs-lookup"><span data-stu-id="8bbd5-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="8bbd5-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="8bbd5-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="8bbd5-120">3</span><span class="sxs-lookup"><span data-stu-id="8bbd5-120">3</span></span>|<span data-ttu-id="8bbd5-121">HTTP 与跨专用组对等混合</span><span class="sxs-lookup"><span data-stu-id="8bbd5-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="8bbd5-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="8bbd5-122">httpWithInternetPeering</span></span>|<span data-ttu-id="8bbd5-123">4</span><span class="sxs-lookup"><span data-stu-id="8bbd5-123">4</span></span>|<span data-ttu-id="8bbd5-124">与 Internet 对等混合的 HTTP</span><span class="sxs-lookup"><span data-stu-id="8bbd5-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="8bbd5-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="8bbd5-125">simpleDownload</span></span>|<span data-ttu-id="8bbd5-126">99</span><span class="sxs-lookup"><span data-stu-id="8bbd5-126">99</span></span>|<span data-ttu-id="8bbd5-127">与没有对等的简单 download 模式</span><span class="sxs-lookup"><span data-stu-id="8bbd5-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="8bbd5-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="8bbd5-128">bypassMode</span></span>|<span data-ttu-id="8bbd5-129">100</span><span class="sxs-lookup"><span data-stu-id="8bbd5-129">100</span></span>|<span data-ttu-id="8bbd5-130">绕过模式。</span><span class="sxs-lookup"><span data-stu-id="8bbd5-130">Bypass mode.</span></span> <span data-ttu-id="8bbd5-131">不使用传递优化并改用位</span><span class="sxs-lookup"><span data-stu-id="8bbd5-131">Do not use Delivery Optimization and use BITS instead</span></span>|



