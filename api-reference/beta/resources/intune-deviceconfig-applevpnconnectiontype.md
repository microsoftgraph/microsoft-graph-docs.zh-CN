---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d31ca3ad0f3b216f727d1f4a8f6f12afa9520758
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124084"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="d2db5-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d2db5-103">appleVpnConnectionType enum type</span></span>

<span data-ttu-id="d2db5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2db5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2db5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2db5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2db5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2db5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2db5-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="d2db5-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="d2db5-108">成员</span><span class="sxs-lookup"><span data-stu-id="d2db5-108">Members</span></span>
|<span data-ttu-id="d2db5-109">成员</span><span class="sxs-lookup"><span data-stu-id="d2db5-109">Member</span></span>|<span data-ttu-id="d2db5-110">值</span><span class="sxs-lookup"><span data-stu-id="d2db5-110">Value</span></span>|<span data-ttu-id="d2db5-111">说明</span><span class="sxs-lookup"><span data-stu-id="d2db5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2db5-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="d2db5-112">ciscoAnyConnect</span></span>|<span data-ttu-id="d2db5-113">0</span><span class="sxs-lookup"><span data-stu-id="d2db5-113">0</span></span>|<span data-ttu-id="d2db5-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="d2db5-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="d2db5-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="d2db5-115">pulseSecure</span></span>|<span data-ttu-id="d2db5-116">1 </span><span class="sxs-lookup"><span data-stu-id="d2db5-116">1</span></span>|<span data-ttu-id="d2db5-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="d2db5-117">Pulse Secure.</span></span>|
|<span data-ttu-id="d2db5-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="d2db5-118">f5EdgeClient</span></span>|<span data-ttu-id="d2db5-119">2 </span><span class="sxs-lookup"><span data-stu-id="d2db5-119">2</span></span>|<span data-ttu-id="d2db5-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="d2db5-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="d2db5-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="d2db5-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="d2db5-122">3 </span><span class="sxs-lookup"><span data-stu-id="d2db5-122">3</span></span>|<span data-ttu-id="d2db5-123">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="d2db5-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="d2db5-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="d2db5-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="d2db5-125">4 </span><span class="sxs-lookup"><span data-stu-id="d2db5-125">4</span></span>|<span data-ttu-id="d2db5-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="d2db5-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="d2db5-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="d2db5-127">customVpn</span></span>|<span data-ttu-id="d2db5-128">5 </span><span class="sxs-lookup"><span data-stu-id="d2db5-128">5</span></span>|<span data-ttu-id="d2db5-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="d2db5-129">Custom VPN.</span></span>|
|<span data-ttu-id="d2db5-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="d2db5-130">ciscoIPSec</span></span>|<span data-ttu-id="d2db5-131">6 </span><span class="sxs-lookup"><span data-stu-id="d2db5-131">6</span></span>|<span data-ttu-id="d2db5-132">Cisco (IPSec) 。</span><span class="sxs-lookup"><span data-stu-id="d2db5-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="d2db5-133">citrix</span><span class="sxs-lookup"><span data-stu-id="d2db5-133">citrix</span></span>|<span data-ttu-id="d2db5-134">7 </span><span class="sxs-lookup"><span data-stu-id="d2db5-134">7</span></span>|<span data-ttu-id="d2db5-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="d2db5-135">Citrix.</span></span>|
|<span data-ttu-id="d2db5-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="d2db5-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="d2db5-137">8 </span><span class="sxs-lookup"><span data-stu-id="d2db5-137">8</span></span>|<span data-ttu-id="d2db5-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="d2db5-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="d2db5-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="d2db5-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="d2db5-140">9 </span><span class="sxs-lookup"><span data-stu-id="d2db5-140">9</span></span>|<span data-ttu-id="d2db5-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="d2db5-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="d2db5-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="d2db5-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="d2db5-143">10 </span><span class="sxs-lookup"><span data-stu-id="d2db5-143">10</span></span>|<span data-ttu-id="d2db5-144">Zscaler 私有访问。</span><span class="sxs-lookup"><span data-stu-id="d2db5-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="d2db5-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="d2db5-145">f5Access2018</span></span>|<span data-ttu-id="d2db5-146">11 </span><span class="sxs-lookup"><span data-stu-id="d2db5-146">11</span></span>|<span data-ttu-id="d2db5-147">F5 访问2018。</span><span class="sxs-lookup"><span data-stu-id="d2db5-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="d2db5-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="d2db5-148">citrixSso</span></span>|<span data-ttu-id="d2db5-149">12 </span><span class="sxs-lookup"><span data-stu-id="d2db5-149">12</span></span>|<span data-ttu-id="d2db5-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="d2db5-150">Citrix Sso.</span></span>|
|<span data-ttu-id="d2db5-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="d2db5-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="d2db5-152">13</span><span class="sxs-lookup"><span data-stu-id="d2db5-152">13</span></span>|<span data-ttu-id="d2db5-153">Palo Alto 网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="d2db5-153">Palo Alto Networks GlobalProtect V2.</span></span>|
|<span data-ttu-id="d2db5-154">ikEv2</span><span class="sxs-lookup"><span data-stu-id="d2db5-154">ikEv2</span></span>|<span data-ttu-id="d2db5-155">14 </span><span class="sxs-lookup"><span data-stu-id="d2db5-155">14</span></span>|<span data-ttu-id="d2db5-156">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="d2db5-156">IKEv2.</span></span>|
|<span data-ttu-id="d2db5-157">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="d2db5-157">alwaysOn</span></span>|<span data-ttu-id="d2db5-158">15 </span><span class="sxs-lookup"><span data-stu-id="d2db5-158">15</span></span>|<span data-ttu-id="d2db5-159">AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="d2db5-159">AlwaysOn.</span></span>|
|<span data-ttu-id="d2db5-160">microsoftTunnel</span><span class="sxs-lookup"><span data-stu-id="d2db5-160">microsoftTunnel</span></span>|<span data-ttu-id="d2db5-161">16 </span><span class="sxs-lookup"><span data-stu-id="d2db5-161">16</span></span>|<span data-ttu-id="d2db5-162">Microsoft 隧道。</span><span class="sxs-lookup"><span data-stu-id="d2db5-162">Microsoft Tunnel.</span></span>|



