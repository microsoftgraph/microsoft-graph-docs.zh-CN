---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f40281934aa241f245772e0bc4c5cd5bbbd0ec33
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415675"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="56ca7-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="56ca7-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="56ca7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="56ca7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56ca7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="56ca7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56ca7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56ca7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56ca7-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="56ca7-107">Apple VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="56ca7-108">成员</span><span class="sxs-lookup"><span data-stu-id="56ca7-108">Members</span></span>
|<span data-ttu-id="56ca7-109">成员</span><span class="sxs-lookup"><span data-stu-id="56ca7-109">Member</span></span>|<span data-ttu-id="56ca7-110">值</span><span class="sxs-lookup"><span data-stu-id="56ca7-110">Value</span></span>|<span data-ttu-id="56ca7-111">说明</span><span class="sxs-lookup"><span data-stu-id="56ca7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56ca7-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="56ca7-112">ciscoAnyConnect</span></span>|<span data-ttu-id="56ca7-113">0</span><span class="sxs-lookup"><span data-stu-id="56ca7-113">0</span></span>|<span data-ttu-id="56ca7-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="56ca7-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="56ca7-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="56ca7-115">pulseSecure</span></span>|<span data-ttu-id="56ca7-116">1</span><span class="sxs-lookup"><span data-stu-id="56ca7-116">1</span></span>|<span data-ttu-id="56ca7-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="56ca7-117">Pulse Secure.</span></span>|
|<span data-ttu-id="56ca7-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="56ca7-118">f5EdgeClient</span></span>|<span data-ttu-id="56ca7-119">2</span><span class="sxs-lookup"><span data-stu-id="56ca7-119">2</span></span>|<span data-ttu-id="56ca7-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="56ca7-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="56ca7-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="56ca7-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="56ca7-122">3</span><span class="sxs-lookup"><span data-stu-id="56ca7-122">3</span></span>|<span data-ttu-id="56ca7-123">Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="56ca7-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="56ca7-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="56ca7-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="56ca7-125">4</span><span class="sxs-lookup"><span data-stu-id="56ca7-125">4</span></span>|<span data-ttu-id="56ca7-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="56ca7-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="56ca7-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="56ca7-127">customVpn</span></span>|<span data-ttu-id="56ca7-128">5</span><span class="sxs-lookup"><span data-stu-id="56ca7-128">5</span></span>|<span data-ttu-id="56ca7-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="56ca7-129">Custom VPN.</span></span>|
|<span data-ttu-id="56ca7-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="56ca7-130">ciscoIPSec</span></span>|<span data-ttu-id="56ca7-131">6</span><span class="sxs-lookup"><span data-stu-id="56ca7-131">6</span></span>|<span data-ttu-id="56ca7-132">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="56ca7-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="56ca7-133">citrix</span><span class="sxs-lookup"><span data-stu-id="56ca7-133">citrix</span></span>|<span data-ttu-id="56ca7-134">7</span><span class="sxs-lookup"><span data-stu-id="56ca7-134">7</span></span>|<span data-ttu-id="56ca7-135">Citrix。</span><span class="sxs-lookup"><span data-stu-id="56ca7-135">Citrix.</span></span>|
|<span data-ttu-id="56ca7-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="56ca7-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="56ca7-137">8</span><span class="sxs-lookup"><span data-stu-id="56ca7-137">8</span></span>|<span data-ttu-id="56ca7-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="56ca7-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="56ca7-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="56ca7-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="56ca7-140">9</span><span class="sxs-lookup"><span data-stu-id="56ca7-140">9</span></span>|<span data-ttu-id="56ca7-141">帕罗奥市网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="56ca7-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="56ca7-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="56ca7-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="56ca7-143">10</span><span class="sxs-lookup"><span data-stu-id="56ca7-143">10</span></span>|<span data-ttu-id="56ca7-144">Zscaler 专用访问。</span><span class="sxs-lookup"><span data-stu-id="56ca7-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="56ca7-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="56ca7-145">f5Access2018</span></span>|<span data-ttu-id="56ca7-146">11</span><span class="sxs-lookup"><span data-stu-id="56ca7-146">11</span></span>|<span data-ttu-id="56ca7-147">F5 访问 2018。</span><span class="sxs-lookup"><span data-stu-id="56ca7-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="56ca7-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="56ca7-148">citrixSso</span></span>|<span data-ttu-id="56ca7-149">12</span><span class="sxs-lookup"><span data-stu-id="56ca7-149">12</span></span>|<span data-ttu-id="56ca7-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="56ca7-150">Citrix Sso.</span></span>|
|<span data-ttu-id="56ca7-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="56ca7-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="56ca7-152">13</span><span class="sxs-lookup"><span data-stu-id="56ca7-152">13</span></span>|<span data-ttu-id="56ca7-153">帕洛阿尔托市网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="56ca7-153">Palo Alto Networks GlobalProtect V2.</span></span>|




