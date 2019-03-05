---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e5e0e3248315fc598d95ea3eb2bb46a6445a5968
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166708"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="a38d9-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a38d9-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="a38d9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a38d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a38d9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a38d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a38d9-106">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="a38d9-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="a38d9-107">成员</span><span class="sxs-lookup"><span data-stu-id="a38d9-107">Members</span></span>
|<span data-ttu-id="a38d9-108">成员</span><span class="sxs-lookup"><span data-stu-id="a38d9-108">Member</span></span>|<span data-ttu-id="a38d9-109">值</span><span class="sxs-lookup"><span data-stu-id="a38d9-109">Value</span></span>|<span data-ttu-id="a38d9-110">说明</span><span class="sxs-lookup"><span data-stu-id="a38d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a38d9-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="a38d9-111">pulseSecure</span></span>|<span data-ttu-id="a38d9-112">0</span><span class="sxs-lookup"><span data-stu-id="a38d9-112">0</span></span>|<span data-ttu-id="a38d9-113">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="a38d9-113">Pulse Secure.</span></span>|
|<span data-ttu-id="a38d9-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="a38d9-114">f5EdgeClient</span></span>|<span data-ttu-id="a38d9-115">1</span><span class="sxs-lookup"><span data-stu-id="a38d9-115">1</span></span>|<span data-ttu-id="a38d9-116">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="a38d9-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="a38d9-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="a38d9-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="a38d9-118">双面</span><span class="sxs-lookup"><span data-stu-id="a38d9-118">2</span></span>|<span data-ttu-id="a38d9-119">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="a38d9-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="a38d9-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="a38d9-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="a38d9-121">第三章</span><span class="sxs-lookup"><span data-stu-id="a38d9-121">3</span></span>|<span data-ttu-id="a38d9-122">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="a38d9-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="a38d9-123">自动</span><span class="sxs-lookup"><span data-stu-id="a38d9-123">automatic</span></span>|<span data-ttu-id="a38d9-124">4</span><span class="sxs-lookup"><span data-stu-id="a38d9-124">4</span></span>|<span data-ttu-id="a38d9-125">自动。</span><span class="sxs-lookup"><span data-stu-id="a38d9-125">Automatic.</span></span>|
|<span data-ttu-id="a38d9-126">ikEv2</span><span class="sxs-lookup"><span data-stu-id="a38d9-126">ikEv2</span></span>|<span data-ttu-id="a38d9-127">5</span><span class="sxs-lookup"><span data-stu-id="a38d9-127">5</span></span>|<span data-ttu-id="a38d9-128">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="a38d9-128">IKEv2.</span></span>|
|<span data-ttu-id="a38d9-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="a38d9-129">l2tp</span></span>|<span data-ttu-id="a38d9-130">型</span><span class="sxs-lookup"><span data-stu-id="a38d9-130">6</span></span>|<span data-ttu-id="a38d9-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="a38d9-131">L2TP.</span></span>|
|<span data-ttu-id="a38d9-132">pptp</span><span class="sxs-lookup"><span data-stu-id="a38d9-132">pptp</span></span>|<span data-ttu-id="a38d9-133">步</span><span class="sxs-lookup"><span data-stu-id="a38d9-133">7</span></span>|<span data-ttu-id="a38d9-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="a38d9-134">PPTP.</span></span>|
|<span data-ttu-id="a38d9-135">citrix</span><span class="sxs-lookup"><span data-stu-id="a38d9-135">citrix</span></span>|<span data-ttu-id="a38d9-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="a38d9-136">8</span></span>|<span data-ttu-id="a38d9-137">Citrix.</span><span class="sxs-lookup"><span data-stu-id="a38d9-137">Citrix.</span></span>|
|<span data-ttu-id="a38d9-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="a38d9-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="a38d9-139">第</span><span class="sxs-lookup"><span data-stu-id="a38d9-139">9</span></span>|<span data-ttu-id="a38d9-140">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="a38d9-140">Palo Alto Networks GlobalProtect.</span></span>|




