---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8badac8419f2a3327ad608b334d2f6190f091d58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084700"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="ea115-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ea115-103">windows10VpnConnectionType enum type</span></span>

<span data-ttu-id="ea115-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea115-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea115-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea115-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea115-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea115-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea115-107">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="ea115-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="ea115-108">成员</span><span class="sxs-lookup"><span data-stu-id="ea115-108">Members</span></span>
|<span data-ttu-id="ea115-109">成员</span><span class="sxs-lookup"><span data-stu-id="ea115-109">Member</span></span>|<span data-ttu-id="ea115-110">值</span><span class="sxs-lookup"><span data-stu-id="ea115-110">Value</span></span>|<span data-ttu-id="ea115-111">说明</span><span class="sxs-lookup"><span data-stu-id="ea115-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea115-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="ea115-112">pulseSecure</span></span>|<span data-ttu-id="ea115-113">0</span><span class="sxs-lookup"><span data-stu-id="ea115-113">0</span></span>|<span data-ttu-id="ea115-114">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="ea115-114">Pulse Secure.</span></span>|
|<span data-ttu-id="ea115-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="ea115-115">f5EdgeClient</span></span>|<span data-ttu-id="ea115-116">1 </span><span class="sxs-lookup"><span data-stu-id="ea115-116">1</span></span>|<span data-ttu-id="ea115-117">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="ea115-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="ea115-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="ea115-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="ea115-119">2 </span><span class="sxs-lookup"><span data-stu-id="ea115-119">2</span></span>|<span data-ttu-id="ea115-120">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="ea115-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="ea115-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="ea115-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="ea115-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ea115-122">3</span></span>|<span data-ttu-id="ea115-123">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="ea115-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ea115-124">自动</span><span class="sxs-lookup"><span data-stu-id="ea115-124">automatic</span></span>|<span data-ttu-id="ea115-125">4 </span><span class="sxs-lookup"><span data-stu-id="ea115-125">4</span></span>|<span data-ttu-id="ea115-126">自动。</span><span class="sxs-lookup"><span data-stu-id="ea115-126">Automatic.</span></span>|
|<span data-ttu-id="ea115-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="ea115-127">ikEv2</span></span>|<span data-ttu-id="ea115-128">5 </span><span class="sxs-lookup"><span data-stu-id="ea115-128">5</span></span>|<span data-ttu-id="ea115-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="ea115-129">IKEv2.</span></span>|
|<span data-ttu-id="ea115-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="ea115-130">l2tp</span></span>|<span data-ttu-id="ea115-131">6 </span><span class="sxs-lookup"><span data-stu-id="ea115-131">6</span></span>|<span data-ttu-id="ea115-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="ea115-132">L2TP.</span></span>|
|<span data-ttu-id="ea115-133">pptp</span><span class="sxs-lookup"><span data-stu-id="ea115-133">pptp</span></span>|<span data-ttu-id="ea115-134">7 </span><span class="sxs-lookup"><span data-stu-id="ea115-134">7</span></span>|<span data-ttu-id="ea115-135">PPTP.</span><span class="sxs-lookup"><span data-stu-id="ea115-135">PPTP.</span></span>|
|<span data-ttu-id="ea115-136">citrix</span><span class="sxs-lookup"><span data-stu-id="ea115-136">citrix</span></span>|<span data-ttu-id="ea115-137">8 </span><span class="sxs-lookup"><span data-stu-id="ea115-137">8</span></span>|<span data-ttu-id="ea115-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="ea115-138">Citrix.</span></span>|
|<span data-ttu-id="ea115-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="ea115-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="ea115-140">9 </span><span class="sxs-lookup"><span data-stu-id="ea115-140">9</span></span>|<span data-ttu-id="ea115-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="ea115-141">Palo Alto Networks GlobalProtect.</span></span>|






