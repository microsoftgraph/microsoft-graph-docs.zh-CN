---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0f9fb609ab1386105c3b80c060d6dbde35080d53
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444509"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="e6186-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e6186-103">windows10VpnConnectionType enum type</span></span>

<span data-ttu-id="e6186-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6186-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6186-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6186-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6186-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6186-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6186-107">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="e6186-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="e6186-108">成员</span><span class="sxs-lookup"><span data-stu-id="e6186-108">Members</span></span>
|<span data-ttu-id="e6186-109">成员</span><span class="sxs-lookup"><span data-stu-id="e6186-109">Member</span></span>|<span data-ttu-id="e6186-110">值</span><span class="sxs-lookup"><span data-stu-id="e6186-110">Value</span></span>|<span data-ttu-id="e6186-111">说明</span><span class="sxs-lookup"><span data-stu-id="e6186-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6186-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="e6186-112">pulseSecure</span></span>|<span data-ttu-id="e6186-113">0</span><span class="sxs-lookup"><span data-stu-id="e6186-113">0</span></span>|<span data-ttu-id="e6186-114">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="e6186-114">Pulse Secure.</span></span>|
|<span data-ttu-id="e6186-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="e6186-115">f5EdgeClient</span></span>|<span data-ttu-id="e6186-116">1 </span><span class="sxs-lookup"><span data-stu-id="e6186-116">1</span></span>|<span data-ttu-id="e6186-117">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="e6186-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="e6186-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="e6186-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="e6186-119">2 </span><span class="sxs-lookup"><span data-stu-id="e6186-119">2</span></span>|<span data-ttu-id="e6186-120">Dell SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="e6186-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="e6186-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="e6186-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="e6186-122">3 </span><span class="sxs-lookup"><span data-stu-id="e6186-122">3</span></span>|<span data-ttu-id="e6186-123">Check Point Capsule VPN。</span><span class="sxs-lookup"><span data-stu-id="e6186-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="e6186-124">自动</span><span class="sxs-lookup"><span data-stu-id="e6186-124">automatic</span></span>|<span data-ttu-id="e6186-125">4 </span><span class="sxs-lookup"><span data-stu-id="e6186-125">4</span></span>|<span data-ttu-id="e6186-126">自动。</span><span class="sxs-lookup"><span data-stu-id="e6186-126">Automatic.</span></span>|
|<span data-ttu-id="e6186-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="e6186-127">ikEv2</span></span>|<span data-ttu-id="e6186-128">5 </span><span class="sxs-lookup"><span data-stu-id="e6186-128">5</span></span>|<span data-ttu-id="e6186-129">IKEv2。</span><span class="sxs-lookup"><span data-stu-id="e6186-129">IKEv2.</span></span>|
|<span data-ttu-id="e6186-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="e6186-130">l2tp</span></span>|<span data-ttu-id="e6186-131">6 </span><span class="sxs-lookup"><span data-stu-id="e6186-131">6</span></span>|<span data-ttu-id="e6186-132">L2TP。</span><span class="sxs-lookup"><span data-stu-id="e6186-132">L2TP.</span></span>|
|<span data-ttu-id="e6186-133">pptp</span><span class="sxs-lookup"><span data-stu-id="e6186-133">pptp</span></span>|<span data-ttu-id="e6186-134">7 </span><span class="sxs-lookup"><span data-stu-id="e6186-134">7</span></span>|<span data-ttu-id="e6186-135">PPTP。</span><span class="sxs-lookup"><span data-stu-id="e6186-135">PPTP.</span></span>|
|<span data-ttu-id="e6186-136">citrix</span><span class="sxs-lookup"><span data-stu-id="e6186-136">citrix</span></span>|<span data-ttu-id="e6186-137">8 </span><span class="sxs-lookup"><span data-stu-id="e6186-137">8</span></span>|<span data-ttu-id="e6186-138">Citrix。</span><span class="sxs-lookup"><span data-stu-id="e6186-138">Citrix.</span></span>|
|<span data-ttu-id="e6186-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="e6186-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="e6186-140">9 </span><span class="sxs-lookup"><span data-stu-id="e6186-140">9</span></span>|<span data-ttu-id="e6186-141">Palo Alto Networks GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="e6186-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="e6186-142">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="e6186-142">ciscoAnyConnect</span></span>|<span data-ttu-id="e6186-143">10  </span><span class="sxs-lookup"><span data-stu-id="e6186-143">10</span></span>|<span data-ttu-id="e6186-144">Cisco AnyConnect</span><span class="sxs-lookup"><span data-stu-id="e6186-144">Cisco AnyConnect</span></span>|




