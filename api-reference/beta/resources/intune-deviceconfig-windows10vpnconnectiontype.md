---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e2db29d395a91d43fbb71a634b06a6000f65796
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944220"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="94db8-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="94db8-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="94db8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94db8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94db8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94db8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94db8-106">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="94db8-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="94db8-107">成员</span><span class="sxs-lookup"><span data-stu-id="94db8-107">Members</span></span>
|<span data-ttu-id="94db8-108">成员</span><span class="sxs-lookup"><span data-stu-id="94db8-108">Member</span></span>|<span data-ttu-id="94db8-109">值</span><span class="sxs-lookup"><span data-stu-id="94db8-109">Value</span></span>|<span data-ttu-id="94db8-110">说明</span><span class="sxs-lookup"><span data-stu-id="94db8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94db8-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="94db8-111">pulseSecure</span></span>|<span data-ttu-id="94db8-112">0</span><span class="sxs-lookup"><span data-stu-id="94db8-112">0</span></span>|<span data-ttu-id="94db8-113">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="94db8-113">Pulse Secure.</span></span>|
|<span data-ttu-id="94db8-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="94db8-114">f5EdgeClient</span></span>|<span data-ttu-id="94db8-115">1</span><span class="sxs-lookup"><span data-stu-id="94db8-115">1</span></span>|<span data-ttu-id="94db8-116">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="94db8-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="94db8-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="94db8-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="94db8-118">双面</span><span class="sxs-lookup"><span data-stu-id="94db8-118">2</span></span>|<span data-ttu-id="94db8-119">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="94db8-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="94db8-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="94db8-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="94db8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="94db8-121">3</span></span>|<span data-ttu-id="94db8-122">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="94db8-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="94db8-123">自动</span><span class="sxs-lookup"><span data-stu-id="94db8-123">automatic</span></span>|<span data-ttu-id="94db8-124">4</span><span class="sxs-lookup"><span data-stu-id="94db8-124">4</span></span>|<span data-ttu-id="94db8-125">自动。</span><span class="sxs-lookup"><span data-stu-id="94db8-125">Automatic.</span></span>|
|<span data-ttu-id="94db8-126">ikEv2</span><span class="sxs-lookup"><span data-stu-id="94db8-126">ikEv2</span></span>|<span data-ttu-id="94db8-127">5</span><span class="sxs-lookup"><span data-stu-id="94db8-127">5</span></span>|<span data-ttu-id="94db8-128">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="94db8-128">IKEv2.</span></span>|
|<span data-ttu-id="94db8-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="94db8-129">l2tp</span></span>|<span data-ttu-id="94db8-130">型</span><span class="sxs-lookup"><span data-stu-id="94db8-130">6</span></span>|<span data-ttu-id="94db8-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="94db8-131">L2TP.</span></span>|
|<span data-ttu-id="94db8-132">pptp</span><span class="sxs-lookup"><span data-stu-id="94db8-132">pptp</span></span>|<span data-ttu-id="94db8-133">步</span><span class="sxs-lookup"><span data-stu-id="94db8-133">7</span></span>|<span data-ttu-id="94db8-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="94db8-134">PPTP.</span></span>|
|<span data-ttu-id="94db8-135">citrix</span><span class="sxs-lookup"><span data-stu-id="94db8-135">citrix</span></span>|<span data-ttu-id="94db8-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="94db8-136">8</span></span>|<span data-ttu-id="94db8-137">Citrix.</span><span class="sxs-lookup"><span data-stu-id="94db8-137">Citrix.</span></span>|
|<span data-ttu-id="94db8-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="94db8-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="94db8-139">第</span><span class="sxs-lookup"><span data-stu-id="94db8-139">9</span></span>|<span data-ttu-id="94db8-140">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="94db8-140">Palo Alto Networks GlobalProtect.</span></span>|




