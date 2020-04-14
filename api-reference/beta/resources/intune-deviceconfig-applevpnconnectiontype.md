---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efb6a8c8c77a50f253b01f6a73a41eb922347254
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470025"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="a73d7-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a73d7-103">appleVpnConnectionType enum type</span></span>

<span data-ttu-id="a73d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a73d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a73d7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a73d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a73d7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a73d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a73d7-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="a73d7-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="a73d7-108">成员</span><span class="sxs-lookup"><span data-stu-id="a73d7-108">Members</span></span>
|<span data-ttu-id="a73d7-109">成员</span><span class="sxs-lookup"><span data-stu-id="a73d7-109">Member</span></span>|<span data-ttu-id="a73d7-110">值</span><span class="sxs-lookup"><span data-stu-id="a73d7-110">Value</span></span>|<span data-ttu-id="a73d7-111">说明</span><span class="sxs-lookup"><span data-stu-id="a73d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a73d7-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="a73d7-112">ciscoAnyConnect</span></span>|<span data-ttu-id="a73d7-113">0</span><span class="sxs-lookup"><span data-stu-id="a73d7-113">0</span></span>|<span data-ttu-id="a73d7-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="a73d7-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="a73d7-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="a73d7-115">pulseSecure</span></span>|<span data-ttu-id="a73d7-116">1</span><span class="sxs-lookup"><span data-stu-id="a73d7-116">1</span></span>|<span data-ttu-id="a73d7-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="a73d7-117">Pulse Secure.</span></span>|
|<span data-ttu-id="a73d7-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="a73d7-118">f5EdgeClient</span></span>|<span data-ttu-id="a73d7-119">双面</span><span class="sxs-lookup"><span data-stu-id="a73d7-119">2</span></span>|<span data-ttu-id="a73d7-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="a73d7-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="a73d7-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="a73d7-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="a73d7-122">第三章</span><span class="sxs-lookup"><span data-stu-id="a73d7-122">3</span></span>|<span data-ttu-id="a73d7-123">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="a73d7-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="a73d7-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="a73d7-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="a73d7-125">4 </span><span class="sxs-lookup"><span data-stu-id="a73d7-125">4</span></span>|<span data-ttu-id="a73d7-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="a73d7-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="a73d7-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="a73d7-127">customVpn</span></span>|<span data-ttu-id="a73d7-128">5 </span><span class="sxs-lookup"><span data-stu-id="a73d7-128">5</span></span>|<span data-ttu-id="a73d7-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="a73d7-129">Custom VPN.</span></span>|
|<span data-ttu-id="a73d7-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="a73d7-130">ciscoIPSec</span></span>|<span data-ttu-id="a73d7-131">6 </span><span class="sxs-lookup"><span data-stu-id="a73d7-131">6</span></span>|<span data-ttu-id="a73d7-132">Cisco （IPSec）。</span><span class="sxs-lookup"><span data-stu-id="a73d7-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="a73d7-133">citrix</span><span class="sxs-lookup"><span data-stu-id="a73d7-133">citrix</span></span>|<span data-ttu-id="a73d7-134">7 </span><span class="sxs-lookup"><span data-stu-id="a73d7-134">7</span></span>|<span data-ttu-id="a73d7-135">Citrix.</span><span class="sxs-lookup"><span data-stu-id="a73d7-135">Citrix.</span></span>|
|<span data-ttu-id="a73d7-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="a73d7-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="a73d7-137">8 </span><span class="sxs-lookup"><span data-stu-id="a73d7-137">8</span></span>|<span data-ttu-id="a73d7-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="a73d7-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="a73d7-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="a73d7-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="a73d7-140">9 </span><span class="sxs-lookup"><span data-stu-id="a73d7-140">9</span></span>|<span data-ttu-id="a73d7-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="a73d7-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="a73d7-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="a73d7-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="a73d7-143">10 </span><span class="sxs-lookup"><span data-stu-id="a73d7-143">10</span></span>|<span data-ttu-id="a73d7-144">Zscaler 私有访问。</span><span class="sxs-lookup"><span data-stu-id="a73d7-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="a73d7-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="a73d7-145">f5Access2018</span></span>|<span data-ttu-id="a73d7-146">11x17</span><span class="sxs-lookup"><span data-stu-id="a73d7-146">11</span></span>|<span data-ttu-id="a73d7-147">F5 访问2018。</span><span class="sxs-lookup"><span data-stu-id="a73d7-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="a73d7-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="a73d7-148">citrixSso</span></span>|<span data-ttu-id="a73d7-149">12 </span><span class="sxs-lookup"><span data-stu-id="a73d7-149">12</span></span>|<span data-ttu-id="a73d7-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="a73d7-150">Citrix Sso.</span></span>|
|<span data-ttu-id="a73d7-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="a73d7-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="a73d7-152">13</span><span class="sxs-lookup"><span data-stu-id="a73d7-152">13</span></span>|<span data-ttu-id="a73d7-153">Palo Alto 网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="a73d7-153">Palo Alto Networks GlobalProtect V2.</span></span>|
|<span data-ttu-id="a73d7-154">ikEv2</span><span class="sxs-lookup"><span data-stu-id="a73d7-154">ikEv2</span></span>|<span data-ttu-id="a73d7-155">14 </span><span class="sxs-lookup"><span data-stu-id="a73d7-155">14</span></span>|<span data-ttu-id="a73d7-156">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="a73d7-156">IKEv2.</span></span>|
|<span data-ttu-id="a73d7-157">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="a73d7-157">alwaysOn</span></span>|<span data-ttu-id="a73d7-158">15 </span><span class="sxs-lookup"><span data-stu-id="a73d7-158">15</span></span>|<span data-ttu-id="a73d7-159">AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="a73d7-159">AlwaysOn.</span></span>|



