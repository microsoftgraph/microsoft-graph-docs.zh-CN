---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53ed413b05e29a10cebf151c718e55c75de702c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155599"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="65ac9-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="65ac9-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="65ac9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65ac9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65ac9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65ac9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65ac9-106">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="65ac9-106">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="65ac9-107">成员</span><span class="sxs-lookup"><span data-stu-id="65ac9-107">Members</span></span>
|<span data-ttu-id="65ac9-108">成员</span><span class="sxs-lookup"><span data-stu-id="65ac9-108">Member</span></span>|<span data-ttu-id="65ac9-109">值</span><span class="sxs-lookup"><span data-stu-id="65ac9-109">Value</span></span>|<span data-ttu-id="65ac9-110">说明</span><span class="sxs-lookup"><span data-stu-id="65ac9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65ac9-111">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="65ac9-111">ciscoAnyConnect</span></span>|<span data-ttu-id="65ac9-112">0</span><span class="sxs-lookup"><span data-stu-id="65ac9-112">0</span></span>|<span data-ttu-id="65ac9-113">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="65ac9-113">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="65ac9-114">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="65ac9-114">pulseSecure</span></span>|<span data-ttu-id="65ac9-115">1</span><span class="sxs-lookup"><span data-stu-id="65ac9-115">1</span></span>|<span data-ttu-id="65ac9-116">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="65ac9-116">Pulse Secure.</span></span>|
|<span data-ttu-id="65ac9-117">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="65ac9-117">f5EdgeClient</span></span>|<span data-ttu-id="65ac9-118">双面</span><span class="sxs-lookup"><span data-stu-id="65ac9-118">2</span></span>|<span data-ttu-id="65ac9-119">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="65ac9-119">F5 Edge Client.</span></span>|
|<span data-ttu-id="65ac9-120">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="65ac9-120">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="65ac9-121">第三章</span><span class="sxs-lookup"><span data-stu-id="65ac9-121">3</span></span>|<span data-ttu-id="65ac9-122">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="65ac9-122">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="65ac9-123">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="65ac9-123">checkPointCapsuleVpn</span></span>|<span data-ttu-id="65ac9-124">4</span><span class="sxs-lookup"><span data-stu-id="65ac9-124">4</span></span>|<span data-ttu-id="65ac9-125">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="65ac9-125">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="65ac9-126">customVpn</span><span class="sxs-lookup"><span data-stu-id="65ac9-126">customVpn</span></span>|<span data-ttu-id="65ac9-127">5</span><span class="sxs-lookup"><span data-stu-id="65ac9-127">5</span></span>|<span data-ttu-id="65ac9-128">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="65ac9-128">Custom VPN.</span></span>|
|<span data-ttu-id="65ac9-129">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="65ac9-129">ciscoIPSec</span></span>|<span data-ttu-id="65ac9-130">型</span><span class="sxs-lookup"><span data-stu-id="65ac9-130">6</span></span>|<span data-ttu-id="65ac9-131">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="65ac9-131">Cisco (IPSec).</span></span>|
|<span data-ttu-id="65ac9-132">citrix</span><span class="sxs-lookup"><span data-stu-id="65ac9-132">citrix</span></span>|<span data-ttu-id="65ac9-133">步</span><span class="sxs-lookup"><span data-stu-id="65ac9-133">7</span></span>|<span data-ttu-id="65ac9-134">Citrix.</span><span class="sxs-lookup"><span data-stu-id="65ac9-134">Citrix.</span></span>|
|<span data-ttu-id="65ac9-135">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="65ac9-135">ciscoAnyConnectV2</span></span>|<span data-ttu-id="65ac9-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="65ac9-136">8</span></span>|<span data-ttu-id="65ac9-137">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="65ac9-137">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="65ac9-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="65ac9-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="65ac9-139">第</span><span class="sxs-lookup"><span data-stu-id="65ac9-139">9</span></span>|<span data-ttu-id="65ac9-140">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="65ac9-140">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="65ac9-141">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="65ac9-141">zscalerPrivateAccess</span></span>|<span data-ttu-id="65ac9-142">10</span><span class="sxs-lookup"><span data-stu-id="65ac9-142">10</span></span>|<span data-ttu-id="65ac9-143">Zscaler 私有访问。</span><span class="sxs-lookup"><span data-stu-id="65ac9-143">Zscaler Private Access.</span></span>|
|<span data-ttu-id="65ac9-144">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="65ac9-144">f5Access2018</span></span>|<span data-ttu-id="65ac9-145">11x17</span><span class="sxs-lookup"><span data-stu-id="65ac9-145">11</span></span>|<span data-ttu-id="65ac9-146">F5 访问2018。</span><span class="sxs-lookup"><span data-stu-id="65ac9-146">F5 Access 2018.</span></span>|
|<span data-ttu-id="65ac9-147">citrixSso</span><span class="sxs-lookup"><span data-stu-id="65ac9-147">citrixSso</span></span>|<span data-ttu-id="65ac9-148">12</span><span class="sxs-lookup"><span data-stu-id="65ac9-148">12</span></span>|<span data-ttu-id="65ac9-149">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="65ac9-149">Citrix Sso.</span></span>|
|<span data-ttu-id="65ac9-150">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="65ac9-150">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="65ac9-151">13</span><span class="sxs-lookup"><span data-stu-id="65ac9-151">13</span></span>|<span data-ttu-id="65ac9-152">Palo Alto 网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="65ac9-152">Palo Alto Networks GlobalProtect V2.</span></span>|




