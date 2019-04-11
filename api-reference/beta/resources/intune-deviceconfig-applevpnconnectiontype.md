---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cbb3b3ba87a65d248da248bfe66abb426fdd764
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806018"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="055c8-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="055c8-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="055c8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="055c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="055c8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="055c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="055c8-106">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="055c8-106">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="055c8-107">成员</span><span class="sxs-lookup"><span data-stu-id="055c8-107">Members</span></span>
|<span data-ttu-id="055c8-108">成员</span><span class="sxs-lookup"><span data-stu-id="055c8-108">Member</span></span>|<span data-ttu-id="055c8-109">值</span><span class="sxs-lookup"><span data-stu-id="055c8-109">Value</span></span>|<span data-ttu-id="055c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="055c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="055c8-111">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="055c8-111">ciscoAnyConnect</span></span>|<span data-ttu-id="055c8-112">0</span><span class="sxs-lookup"><span data-stu-id="055c8-112">0</span></span>|<span data-ttu-id="055c8-113">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="055c8-113">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="055c8-114">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="055c8-114">pulseSecure</span></span>|<span data-ttu-id="055c8-115">1</span><span class="sxs-lookup"><span data-stu-id="055c8-115">1</span></span>|<span data-ttu-id="055c8-116">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="055c8-116">Pulse Secure.</span></span>|
|<span data-ttu-id="055c8-117">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="055c8-117">f5EdgeClient</span></span>|<span data-ttu-id="055c8-118">双面</span><span class="sxs-lookup"><span data-stu-id="055c8-118">2</span></span>|<span data-ttu-id="055c8-119">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="055c8-119">F5 Edge Client.</span></span>|
|<span data-ttu-id="055c8-120">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="055c8-120">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="055c8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="055c8-121">3</span></span>|<span data-ttu-id="055c8-122">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="055c8-122">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="055c8-123">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="055c8-123">checkPointCapsuleVpn</span></span>|<span data-ttu-id="055c8-124">4</span><span class="sxs-lookup"><span data-stu-id="055c8-124">4</span></span>|<span data-ttu-id="055c8-125">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="055c8-125">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="055c8-126">customVpn</span><span class="sxs-lookup"><span data-stu-id="055c8-126">customVpn</span></span>|<span data-ttu-id="055c8-127">5</span><span class="sxs-lookup"><span data-stu-id="055c8-127">5</span></span>|<span data-ttu-id="055c8-128">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="055c8-128">Custom VPN.</span></span>|
|<span data-ttu-id="055c8-129">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="055c8-129">ciscoIPSec</span></span>|<span data-ttu-id="055c8-130">型</span><span class="sxs-lookup"><span data-stu-id="055c8-130">6</span></span>|<span data-ttu-id="055c8-131">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="055c8-131">Cisco (IPSec).</span></span>|
|<span data-ttu-id="055c8-132">citrix</span><span class="sxs-lookup"><span data-stu-id="055c8-132">citrix</span></span>|<span data-ttu-id="055c8-133">步</span><span class="sxs-lookup"><span data-stu-id="055c8-133">7</span></span>|<span data-ttu-id="055c8-134">Citrix.</span><span class="sxs-lookup"><span data-stu-id="055c8-134">Citrix.</span></span>|
|<span data-ttu-id="055c8-135">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="055c8-135">ciscoAnyConnectV2</span></span>|<span data-ttu-id="055c8-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="055c8-136">8</span></span>|<span data-ttu-id="055c8-137">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="055c8-137">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="055c8-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="055c8-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="055c8-139">第</span><span class="sxs-lookup"><span data-stu-id="055c8-139">9</span></span>|<span data-ttu-id="055c8-140">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="055c8-140">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="055c8-141">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="055c8-141">zscalerPrivateAccess</span></span>|<span data-ttu-id="055c8-142">10</span><span class="sxs-lookup"><span data-stu-id="055c8-142">10</span></span>|<span data-ttu-id="055c8-143">Zscaler 私有访问。</span><span class="sxs-lookup"><span data-stu-id="055c8-143">Zscaler Private Access.</span></span>|
|<span data-ttu-id="055c8-144">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="055c8-144">f5Access2018</span></span>|<span data-ttu-id="055c8-145">11x17</span><span class="sxs-lookup"><span data-stu-id="055c8-145">11</span></span>|<span data-ttu-id="055c8-146">F5 访问2018。</span><span class="sxs-lookup"><span data-stu-id="055c8-146">F5 Access 2018.</span></span>|
|<span data-ttu-id="055c8-147">citrixSso</span><span class="sxs-lookup"><span data-stu-id="055c8-147">citrixSso</span></span>|<span data-ttu-id="055c8-148">12</span><span class="sxs-lookup"><span data-stu-id="055c8-148">12</span></span>|<span data-ttu-id="055c8-149">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="055c8-149">Citrix Sso.</span></span>|
|<span data-ttu-id="055c8-150">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="055c8-150">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="055c8-151">13</span><span class="sxs-lookup"><span data-stu-id="055c8-151">13</span></span>|<span data-ttu-id="055c8-152">Palo Alto 网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="055c8-152">Palo Alto Networks GlobalProtect V2.</span></span>|





