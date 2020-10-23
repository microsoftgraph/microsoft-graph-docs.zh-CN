---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d392ec953ba802ccda544238c061d1fbb78eb029
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708891"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="83f04-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="83f04-103">appleVpnConnectionType enum type</span></span>

<span data-ttu-id="83f04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83f04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83f04-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83f04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83f04-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83f04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83f04-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="83f04-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="83f04-108">成员</span><span class="sxs-lookup"><span data-stu-id="83f04-108">Members</span></span>
|<span data-ttu-id="83f04-109">成员</span><span class="sxs-lookup"><span data-stu-id="83f04-109">Member</span></span>|<span data-ttu-id="83f04-110">值</span><span class="sxs-lookup"><span data-stu-id="83f04-110">Value</span></span>|<span data-ttu-id="83f04-111">说明</span><span class="sxs-lookup"><span data-stu-id="83f04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83f04-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="83f04-112">ciscoAnyConnect</span></span>|<span data-ttu-id="83f04-113">0</span><span class="sxs-lookup"><span data-stu-id="83f04-113">0</span></span>|<span data-ttu-id="83f04-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="83f04-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="83f04-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="83f04-115">pulseSecure</span></span>|<span data-ttu-id="83f04-116">1</span><span class="sxs-lookup"><span data-stu-id="83f04-116">1</span></span>|<span data-ttu-id="83f04-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="83f04-117">Pulse Secure.</span></span>|
|<span data-ttu-id="83f04-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="83f04-118">f5EdgeClient</span></span>|<span data-ttu-id="83f04-119">双面</span><span class="sxs-lookup"><span data-stu-id="83f04-119">2</span></span>|<span data-ttu-id="83f04-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="83f04-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="83f04-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="83f04-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="83f04-122">第三章</span><span class="sxs-lookup"><span data-stu-id="83f04-122">3</span></span>|<span data-ttu-id="83f04-123">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="83f04-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="83f04-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="83f04-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="83f04-125">4 </span><span class="sxs-lookup"><span data-stu-id="83f04-125">4</span></span>|<span data-ttu-id="83f04-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="83f04-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="83f04-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="83f04-127">customVpn</span></span>|<span data-ttu-id="83f04-128">5 </span><span class="sxs-lookup"><span data-stu-id="83f04-128">5</span></span>|<span data-ttu-id="83f04-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="83f04-129">Custom VPN.</span></span>|
|<span data-ttu-id="83f04-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="83f04-130">ciscoIPSec</span></span>|<span data-ttu-id="83f04-131">6 </span><span class="sxs-lookup"><span data-stu-id="83f04-131">6</span></span>|<span data-ttu-id="83f04-132">Cisco (IPSec) 。</span><span class="sxs-lookup"><span data-stu-id="83f04-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="83f04-133">citrix</span><span class="sxs-lookup"><span data-stu-id="83f04-133">citrix</span></span>|<span data-ttu-id="83f04-134">7 </span><span class="sxs-lookup"><span data-stu-id="83f04-134">7</span></span>|<span data-ttu-id="83f04-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="83f04-135">Citrix.</span></span>|
|<span data-ttu-id="83f04-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="83f04-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="83f04-137">8 </span><span class="sxs-lookup"><span data-stu-id="83f04-137">8</span></span>|<span data-ttu-id="83f04-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="83f04-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="83f04-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="83f04-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="83f04-140">9 </span><span class="sxs-lookup"><span data-stu-id="83f04-140">9</span></span>|<span data-ttu-id="83f04-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="83f04-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="83f04-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="83f04-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="83f04-143">10  </span><span class="sxs-lookup"><span data-stu-id="83f04-143">10</span></span>|<span data-ttu-id="83f04-144">Zscaler 私有访问。</span><span class="sxs-lookup"><span data-stu-id="83f04-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="83f04-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="83f04-145">f5Access2018</span></span>|<span data-ttu-id="83f04-146">11x17</span><span class="sxs-lookup"><span data-stu-id="83f04-146">11</span></span>|<span data-ttu-id="83f04-147">F5 访问2018。</span><span class="sxs-lookup"><span data-stu-id="83f04-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="83f04-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="83f04-148">citrixSso</span></span>|<span data-ttu-id="83f04-149">12 </span><span class="sxs-lookup"><span data-stu-id="83f04-149">12</span></span>|<span data-ttu-id="83f04-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="83f04-150">Citrix Sso.</span></span>|
|<span data-ttu-id="83f04-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="83f04-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="83f04-152">13 </span><span class="sxs-lookup"><span data-stu-id="83f04-152">13</span></span>|<span data-ttu-id="83f04-153">Palo Alto 网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="83f04-153">Palo Alto Networks GlobalProtect V2.</span></span>|
|<span data-ttu-id="83f04-154">ikEv2</span><span class="sxs-lookup"><span data-stu-id="83f04-154">ikEv2</span></span>|<span data-ttu-id="83f04-155">14 </span><span class="sxs-lookup"><span data-stu-id="83f04-155">14</span></span>|<span data-ttu-id="83f04-156">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="83f04-156">IKEv2.</span></span>|
|<span data-ttu-id="83f04-157">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="83f04-157">alwaysOn</span></span>|<span data-ttu-id="83f04-158">15 </span><span class="sxs-lookup"><span data-stu-id="83f04-158">15</span></span>|<span data-ttu-id="83f04-159">AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="83f04-159">AlwaysOn.</span></span>|
|<span data-ttu-id="83f04-160">microsoftTunnel</span><span class="sxs-lookup"><span data-stu-id="83f04-160">microsoftTunnel</span></span>|<span data-ttu-id="83f04-161">16 </span><span class="sxs-lookup"><span data-stu-id="83f04-161">16</span></span>|<span data-ttu-id="83f04-162">Microsoft 隧道。</span><span class="sxs-lookup"><span data-stu-id="83f04-162">Microsoft Tunnel.</span></span>|
|<span data-ttu-id="83f04-163">netMotionMobility</span><span class="sxs-lookup"><span data-stu-id="83f04-163">netMotionMobility</span></span>|<span data-ttu-id="83f04-164">17 </span><span class="sxs-lookup"><span data-stu-id="83f04-164">17</span></span>|<span data-ttu-id="83f04-165">NetMotion 移动性。</span><span class="sxs-lookup"><span data-stu-id="83f04-165">NetMotion Mobility.</span></span>|





