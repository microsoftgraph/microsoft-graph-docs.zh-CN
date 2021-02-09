---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8ce68a0c9fda0bde6dec8035fb788c55920775f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158735"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="32f18-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="32f18-103">appleVpnConnectionType enum type</span></span>

<span data-ttu-id="32f18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32f18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32f18-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32f18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32f18-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32f18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32f18-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="32f18-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="32f18-108">成员</span><span class="sxs-lookup"><span data-stu-id="32f18-108">Members</span></span>
|<span data-ttu-id="32f18-109">成员</span><span class="sxs-lookup"><span data-stu-id="32f18-109">Member</span></span>|<span data-ttu-id="32f18-110">值</span><span class="sxs-lookup"><span data-stu-id="32f18-110">Value</span></span>|<span data-ttu-id="32f18-111">说明</span><span class="sxs-lookup"><span data-stu-id="32f18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32f18-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="32f18-112">ciscoAnyConnect</span></span>|<span data-ttu-id="32f18-113">0</span><span class="sxs-lookup"><span data-stu-id="32f18-113">0</span></span>|<span data-ttu-id="32f18-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="32f18-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="32f18-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="32f18-115">pulseSecure</span></span>|<span data-ttu-id="32f18-116">1 </span><span class="sxs-lookup"><span data-stu-id="32f18-116">1</span></span>|<span data-ttu-id="32f18-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="32f18-117">Pulse Secure.</span></span>|
|<span data-ttu-id="32f18-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="32f18-118">f5EdgeClient</span></span>|<span data-ttu-id="32f18-119">2 </span><span class="sxs-lookup"><span data-stu-id="32f18-119">2</span></span>|<span data-ttu-id="32f18-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="32f18-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="32f18-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="32f18-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="32f18-122">3 </span><span class="sxs-lookup"><span data-stu-id="32f18-122">3</span></span>|<span data-ttu-id="32f18-123">Dell SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="32f18-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="32f18-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="32f18-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="32f18-125">4 </span><span class="sxs-lookup"><span data-stu-id="32f18-125">4</span></span>|<span data-ttu-id="32f18-126">Check Point Capsule VPN.</span><span class="sxs-lookup"><span data-stu-id="32f18-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="32f18-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="32f18-127">customVpn</span></span>|<span data-ttu-id="32f18-128">5 </span><span class="sxs-lookup"><span data-stu-id="32f18-128">5</span></span>|<span data-ttu-id="32f18-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="32f18-129">Custom VPN.</span></span>|
|<span data-ttu-id="32f18-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="32f18-130">ciscoIPSec</span></span>|<span data-ttu-id="32f18-131">6 </span><span class="sxs-lookup"><span data-stu-id="32f18-131">6</span></span>|<span data-ttu-id="32f18-132">Cisco (IPSec) 。</span><span class="sxs-lookup"><span data-stu-id="32f18-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="32f18-133">citrix</span><span class="sxs-lookup"><span data-stu-id="32f18-133">citrix</span></span>|<span data-ttu-id="32f18-134">7 </span><span class="sxs-lookup"><span data-stu-id="32f18-134">7</span></span>|<span data-ttu-id="32f18-135">Citrix。</span><span class="sxs-lookup"><span data-stu-id="32f18-135">Citrix.</span></span>|
|<span data-ttu-id="32f18-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="32f18-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="32f18-137">8 </span><span class="sxs-lookup"><span data-stu-id="32f18-137">8</span></span>|<span data-ttu-id="32f18-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="32f18-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="32f18-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="32f18-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="32f18-140">9 </span><span class="sxs-lookup"><span data-stu-id="32f18-140">9</span></span>|<span data-ttu-id="32f18-141">Palo Alto Networks GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="32f18-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="32f18-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="32f18-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="32f18-143">10  </span><span class="sxs-lookup"><span data-stu-id="32f18-143">10</span></span>|<span data-ttu-id="32f18-144">Zscaler Private Access。</span><span class="sxs-lookup"><span data-stu-id="32f18-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="32f18-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="32f18-145">f5Access2018</span></span>|<span data-ttu-id="32f18-146">11 </span><span class="sxs-lookup"><span data-stu-id="32f18-146">11</span></span>|<span data-ttu-id="32f18-147">F5 Access 2018。</span><span class="sxs-lookup"><span data-stu-id="32f18-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="32f18-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="32f18-148">citrixSso</span></span>|<span data-ttu-id="32f18-149">12 </span><span class="sxs-lookup"><span data-stu-id="32f18-149">12</span></span>|<span data-ttu-id="32f18-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="32f18-150">Citrix Sso.</span></span>|
|<span data-ttu-id="32f18-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="32f18-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="32f18-152">13 </span><span class="sxs-lookup"><span data-stu-id="32f18-152">13</span></span>|<span data-ttu-id="32f18-153">Palo Alto Networks GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="32f18-153">Palo Alto Networks GlobalProtect V2.</span></span>|
|<span data-ttu-id="32f18-154">ikEv2</span><span class="sxs-lookup"><span data-stu-id="32f18-154">ikEv2</span></span>|<span data-ttu-id="32f18-155">14 </span><span class="sxs-lookup"><span data-stu-id="32f18-155">14</span></span>|<span data-ttu-id="32f18-156">IKEv2。</span><span class="sxs-lookup"><span data-stu-id="32f18-156">IKEv2.</span></span>|
|<span data-ttu-id="32f18-157">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="32f18-157">alwaysOn</span></span>|<span data-ttu-id="32f18-158">15 </span><span class="sxs-lookup"><span data-stu-id="32f18-158">15</span></span>|<span data-ttu-id="32f18-159">AlwaysOn。</span><span class="sxs-lookup"><span data-stu-id="32f18-159">AlwaysOn.</span></span>|
|<span data-ttu-id="32f18-160">microsoftTunnel</span><span class="sxs-lookup"><span data-stu-id="32f18-160">microsoftTunnel</span></span>|<span data-ttu-id="32f18-161">16 </span><span class="sxs-lookup"><span data-stu-id="32f18-161">16</span></span>|<span data-ttu-id="32f18-162">Microsoft 隧道。</span><span class="sxs-lookup"><span data-stu-id="32f18-162">Microsoft Tunnel.</span></span>|
|<span data-ttu-id="32f18-163">netMotionMobility</span><span class="sxs-lookup"><span data-stu-id="32f18-163">netMotionMobility</span></span>|<span data-ttu-id="32f18-164">17 </span><span class="sxs-lookup"><span data-stu-id="32f18-164">17</span></span>|<span data-ttu-id="32f18-165">NetMotion Mobility。</span><span class="sxs-lookup"><span data-stu-id="32f18-165">NetMotion Mobility.</span></span>|
|<span data-ttu-id="32f18-166">microsoftProtect</span><span class="sxs-lookup"><span data-stu-id="32f18-166">microsoftProtect</span></span>|<span data-ttu-id="32f18-167">18 </span><span class="sxs-lookup"><span data-stu-id="32f18-167">18</span></span>|<span data-ttu-id="32f18-168">Microsoft 保护。</span><span class="sxs-lookup"><span data-stu-id="32f18-168">Microsoft Protect.</span></span>|




