---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b3797e01d523907731a72aa8b44c9613e4e1400e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075957"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="f2f26-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f2f26-103">appleVpnConnectionType enum type</span></span>

<span data-ttu-id="f2f26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2f26-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f2f26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2f26-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2f26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2f26-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="f2f26-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="f2f26-108">成员</span><span class="sxs-lookup"><span data-stu-id="f2f26-108">Members</span></span>
|<span data-ttu-id="f2f26-109">成员</span><span class="sxs-lookup"><span data-stu-id="f2f26-109">Member</span></span>|<span data-ttu-id="f2f26-110">值</span><span class="sxs-lookup"><span data-stu-id="f2f26-110">Value</span></span>|<span data-ttu-id="f2f26-111">说明</span><span class="sxs-lookup"><span data-stu-id="f2f26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2f26-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="f2f26-112">ciscoAnyConnect</span></span>|<span data-ttu-id="f2f26-113">0</span><span class="sxs-lookup"><span data-stu-id="f2f26-113">0</span></span>|<span data-ttu-id="f2f26-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="f2f26-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="f2f26-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="f2f26-115">pulseSecure</span></span>|<span data-ttu-id="f2f26-116">1 </span><span class="sxs-lookup"><span data-stu-id="f2f26-116">1</span></span>|<span data-ttu-id="f2f26-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="f2f26-117">Pulse Secure.</span></span>|
|<span data-ttu-id="f2f26-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="f2f26-118">f5EdgeClient</span></span>|<span data-ttu-id="f2f26-119">2 </span><span class="sxs-lookup"><span data-stu-id="f2f26-119">2</span></span>|<span data-ttu-id="f2f26-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="f2f26-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="f2f26-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="f2f26-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="f2f26-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f2f26-122">3</span></span>|<span data-ttu-id="f2f26-123">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="f2f26-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="f2f26-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="f2f26-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="f2f26-125">4 </span><span class="sxs-lookup"><span data-stu-id="f2f26-125">4</span></span>|<span data-ttu-id="f2f26-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="f2f26-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="f2f26-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="f2f26-127">customVpn</span></span>|<span data-ttu-id="f2f26-128">5 </span><span class="sxs-lookup"><span data-stu-id="f2f26-128">5</span></span>|<span data-ttu-id="f2f26-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="f2f26-129">Custom VPN.</span></span>|
|<span data-ttu-id="f2f26-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="f2f26-130">ciscoIPSec</span></span>|<span data-ttu-id="f2f26-131">6 </span><span class="sxs-lookup"><span data-stu-id="f2f26-131">6</span></span>|<span data-ttu-id="f2f26-132">Cisco (IPSec) 。</span><span class="sxs-lookup"><span data-stu-id="f2f26-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="f2f26-133">citrix</span><span class="sxs-lookup"><span data-stu-id="f2f26-133">citrix</span></span>|<span data-ttu-id="f2f26-134">7 </span><span class="sxs-lookup"><span data-stu-id="f2f26-134">7</span></span>|<span data-ttu-id="f2f26-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="f2f26-135">Citrix.</span></span>|
|<span data-ttu-id="f2f26-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="f2f26-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="f2f26-137">8 </span><span class="sxs-lookup"><span data-stu-id="f2f26-137">8</span></span>|<span data-ttu-id="f2f26-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="f2f26-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="f2f26-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="f2f26-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="f2f26-140">9 </span><span class="sxs-lookup"><span data-stu-id="f2f26-140">9</span></span>|<span data-ttu-id="f2f26-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="f2f26-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="f2f26-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="f2f26-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="f2f26-143">10 </span><span class="sxs-lookup"><span data-stu-id="f2f26-143">10</span></span>|<span data-ttu-id="f2f26-144">Zscaler 私有访问。</span><span class="sxs-lookup"><span data-stu-id="f2f26-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="f2f26-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="f2f26-145">f5Access2018</span></span>|<span data-ttu-id="f2f26-146">11 </span><span class="sxs-lookup"><span data-stu-id="f2f26-146">11</span></span>|<span data-ttu-id="f2f26-147">F5 访问2018。</span><span class="sxs-lookup"><span data-stu-id="f2f26-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="f2f26-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="f2f26-148">citrixSso</span></span>|<span data-ttu-id="f2f26-149">12 </span><span class="sxs-lookup"><span data-stu-id="f2f26-149">12</span></span>|<span data-ttu-id="f2f26-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="f2f26-150">Citrix Sso.</span></span>|
|<span data-ttu-id="f2f26-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="f2f26-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="f2f26-152">13 </span><span class="sxs-lookup"><span data-stu-id="f2f26-152">13</span></span>|<span data-ttu-id="f2f26-153">Palo Alto 网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="f2f26-153">Palo Alto Networks GlobalProtect V2.</span></span>|
|<span data-ttu-id="f2f26-154">ikEv2</span><span class="sxs-lookup"><span data-stu-id="f2f26-154">ikEv2</span></span>|<span data-ttu-id="f2f26-155">14 </span><span class="sxs-lookup"><span data-stu-id="f2f26-155">14</span></span>|<span data-ttu-id="f2f26-156">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="f2f26-156">IKEv2.</span></span>|
|<span data-ttu-id="f2f26-157">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="f2f26-157">alwaysOn</span></span>|<span data-ttu-id="f2f26-158">15 </span><span class="sxs-lookup"><span data-stu-id="f2f26-158">15</span></span>|<span data-ttu-id="f2f26-159">AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="f2f26-159">AlwaysOn.</span></span>|
|<span data-ttu-id="f2f26-160">microsoftTunnel</span><span class="sxs-lookup"><span data-stu-id="f2f26-160">microsoftTunnel</span></span>|<span data-ttu-id="f2f26-161">16 </span><span class="sxs-lookup"><span data-stu-id="f2f26-161">16</span></span>|<span data-ttu-id="f2f26-162">Microsoft 隧道。</span><span class="sxs-lookup"><span data-stu-id="f2f26-162">Microsoft Tunnel.</span></span>|
|<span data-ttu-id="f2f26-163">netMotionMobility</span><span class="sxs-lookup"><span data-stu-id="f2f26-163">netMotionMobility</span></span>|<span data-ttu-id="f2f26-164">17 </span><span class="sxs-lookup"><span data-stu-id="f2f26-164">17</span></span>|<span data-ttu-id="f2f26-165">NetMotion 移动性。</span><span class="sxs-lookup"><span data-stu-id="f2f26-165">NetMotion Mobility.</span></span>|






