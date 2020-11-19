---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 59ae60a4e438bf2186617c8dbb7c110322519977
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216407"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="9b2c0-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9b2c0-103">appleVpnConnectionType enum type</span></span>

<span data-ttu-id="9b2c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b2c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b2c0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b2c0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b2c0-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="9b2c0-108">成员</span><span class="sxs-lookup"><span data-stu-id="9b2c0-108">Members</span></span>
|<span data-ttu-id="9b2c0-109">成员</span><span class="sxs-lookup"><span data-stu-id="9b2c0-109">Member</span></span>|<span data-ttu-id="9b2c0-110">值</span><span class="sxs-lookup"><span data-stu-id="9b2c0-110">Value</span></span>|<span data-ttu-id="9b2c0-111">说明</span><span class="sxs-lookup"><span data-stu-id="9b2c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b2c0-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="9b2c0-112">ciscoAnyConnect</span></span>|<span data-ttu-id="9b2c0-113">0</span><span class="sxs-lookup"><span data-stu-id="9b2c0-113">0</span></span>|<span data-ttu-id="9b2c0-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="9b2c0-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="9b2c0-115">pulseSecure</span></span>|<span data-ttu-id="9b2c0-116">1</span><span class="sxs-lookup"><span data-stu-id="9b2c0-116">1</span></span>|<span data-ttu-id="9b2c0-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-117">Pulse Secure.</span></span>|
|<span data-ttu-id="9b2c0-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="9b2c0-118">f5EdgeClient</span></span>|<span data-ttu-id="9b2c0-119">双面</span><span class="sxs-lookup"><span data-stu-id="9b2c0-119">2</span></span>|<span data-ttu-id="9b2c0-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="9b2c0-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="9b2c0-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="9b2c0-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9b2c0-122">3</span></span>|<span data-ttu-id="9b2c0-123">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="9b2c0-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="9b2c0-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="9b2c0-125">4 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-125">4</span></span>|<span data-ttu-id="9b2c0-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="9b2c0-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="9b2c0-127">customVpn</span></span>|<span data-ttu-id="9b2c0-128">5 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-128">5</span></span>|<span data-ttu-id="9b2c0-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-129">Custom VPN.</span></span>|
|<span data-ttu-id="9b2c0-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="9b2c0-130">ciscoIPSec</span></span>|<span data-ttu-id="9b2c0-131">6 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-131">6</span></span>|<span data-ttu-id="9b2c0-132">Cisco (IPSec) 。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="9b2c0-133">citrix</span><span class="sxs-lookup"><span data-stu-id="9b2c0-133">citrix</span></span>|<span data-ttu-id="9b2c0-134">7 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-134">7</span></span>|<span data-ttu-id="9b2c0-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="9b2c0-135">Citrix.</span></span>|
|<span data-ttu-id="9b2c0-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="9b2c0-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="9b2c0-137">8 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-137">8</span></span>|<span data-ttu-id="9b2c0-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="9b2c0-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="9b2c0-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="9b2c0-140">9 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-140">9</span></span>|<span data-ttu-id="9b2c0-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="9b2c0-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="9b2c0-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="9b2c0-143">10  </span><span class="sxs-lookup"><span data-stu-id="9b2c0-143">10</span></span>|<span data-ttu-id="9b2c0-144">Zscaler 私有访问。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="9b2c0-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="9b2c0-145">f5Access2018</span></span>|<span data-ttu-id="9b2c0-146">11 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-146">11</span></span>|<span data-ttu-id="9b2c0-147">F5 访问2018。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="9b2c0-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="9b2c0-148">citrixSso</span></span>|<span data-ttu-id="9b2c0-149">12 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-149">12</span></span>|<span data-ttu-id="9b2c0-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-150">Citrix Sso.</span></span>|
|<span data-ttu-id="9b2c0-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="9b2c0-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="9b2c0-152">13 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-152">13</span></span>|<span data-ttu-id="9b2c0-153">Palo Alto 网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-153">Palo Alto Networks GlobalProtect V2.</span></span>|
|<span data-ttu-id="9b2c0-154">ikEv2</span><span class="sxs-lookup"><span data-stu-id="9b2c0-154">ikEv2</span></span>|<span data-ttu-id="9b2c0-155">14 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-155">14</span></span>|<span data-ttu-id="9b2c0-156">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="9b2c0-156">IKEv2.</span></span>|
|<span data-ttu-id="9b2c0-157">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="9b2c0-157">alwaysOn</span></span>|<span data-ttu-id="9b2c0-158">15 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-158">15</span></span>|<span data-ttu-id="9b2c0-159">AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="9b2c0-159">AlwaysOn.</span></span>|
|<span data-ttu-id="9b2c0-160">microsoftTunnel</span><span class="sxs-lookup"><span data-stu-id="9b2c0-160">microsoftTunnel</span></span>|<span data-ttu-id="9b2c0-161">16 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-161">16</span></span>|<span data-ttu-id="9b2c0-162">Microsoft 隧道。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-162">Microsoft Tunnel.</span></span>|
|<span data-ttu-id="9b2c0-163">netMotionMobility</span><span class="sxs-lookup"><span data-stu-id="9b2c0-163">netMotionMobility</span></span>|<span data-ttu-id="9b2c0-164">17 </span><span class="sxs-lookup"><span data-stu-id="9b2c0-164">17</span></span>|<span data-ttu-id="9b2c0-165">NetMotion 移动性。</span><span class="sxs-lookup"><span data-stu-id="9b2c0-165">NetMotion Mobility.</span></span>|




