---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
ms.openlocfilehash: 5308fd8e5876db1d1a38248776c269ce5d80ad38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043243"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="ea239-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ea239-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="ea239-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea239-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea239-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea239-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea239-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ea239-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea239-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="ea239-107">Apple VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="ea239-108">成员</span><span class="sxs-lookup"><span data-stu-id="ea239-108">Members</span></span>
|<span data-ttu-id="ea239-109">成员</span><span class="sxs-lookup"><span data-stu-id="ea239-109">Member</span></span>|<span data-ttu-id="ea239-110">值</span><span class="sxs-lookup"><span data-stu-id="ea239-110">Value</span></span>|<span data-ttu-id="ea239-111">说明</span><span class="sxs-lookup"><span data-stu-id="ea239-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea239-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="ea239-112">ciscoAnyConnect</span></span>|<span data-ttu-id="ea239-113">0</span><span class="sxs-lookup"><span data-stu-id="ea239-113">0</span></span>|<span data-ttu-id="ea239-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="ea239-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="ea239-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="ea239-115">pulseSecure</span></span>|<span data-ttu-id="ea239-116">1</span><span class="sxs-lookup"><span data-stu-id="ea239-116">1</span></span>|<span data-ttu-id="ea239-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="ea239-117">Pulse Secure.</span></span>|
|<span data-ttu-id="ea239-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="ea239-118">f5EdgeClient</span></span>|<span data-ttu-id="ea239-119">2</span><span class="sxs-lookup"><span data-stu-id="ea239-119">2</span></span>|<span data-ttu-id="ea239-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="ea239-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="ea239-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="ea239-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="ea239-122">3</span><span class="sxs-lookup"><span data-stu-id="ea239-122">3</span></span>|<span data-ttu-id="ea239-123">Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="ea239-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="ea239-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="ea239-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="ea239-125">4</span><span class="sxs-lookup"><span data-stu-id="ea239-125">4</span></span>|<span data-ttu-id="ea239-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="ea239-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ea239-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="ea239-127">customVpn</span></span>|<span data-ttu-id="ea239-128">5</span><span class="sxs-lookup"><span data-stu-id="ea239-128">5</span></span>|<span data-ttu-id="ea239-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="ea239-129">Custom VPN.</span></span>|
|<span data-ttu-id="ea239-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="ea239-130">ciscoIPSec</span></span>|<span data-ttu-id="ea239-131">6</span><span class="sxs-lookup"><span data-stu-id="ea239-131">6</span></span>|<span data-ttu-id="ea239-132">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="ea239-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="ea239-133">citrix</span><span class="sxs-lookup"><span data-stu-id="ea239-133">citrix</span></span>|<span data-ttu-id="ea239-134">7</span><span class="sxs-lookup"><span data-stu-id="ea239-134">7</span></span>|<span data-ttu-id="ea239-135">Citrix。</span><span class="sxs-lookup"><span data-stu-id="ea239-135">Citrix.</span></span>|
|<span data-ttu-id="ea239-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="ea239-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="ea239-137">8</span><span class="sxs-lookup"><span data-stu-id="ea239-137">8</span></span>|<span data-ttu-id="ea239-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="ea239-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="ea239-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="ea239-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="ea239-140">9</span><span class="sxs-lookup"><span data-stu-id="ea239-140">9</span></span>|<span data-ttu-id="ea239-141">帕罗奥市网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="ea239-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="ea239-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="ea239-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="ea239-143">10</span><span class="sxs-lookup"><span data-stu-id="ea239-143">10</span></span>|<span data-ttu-id="ea239-144">Zscaler 专用访问。</span><span class="sxs-lookup"><span data-stu-id="ea239-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="ea239-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="ea239-145">f5Access2018</span></span>|<span data-ttu-id="ea239-146">11</span><span class="sxs-lookup"><span data-stu-id="ea239-146">11</span></span>|<span data-ttu-id="ea239-147">F5 访问 2018。</span><span class="sxs-lookup"><span data-stu-id="ea239-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="ea239-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="ea239-148">citrixSso</span></span>|<span data-ttu-id="ea239-149">12</span><span class="sxs-lookup"><span data-stu-id="ea239-149">12</span></span>|<span data-ttu-id="ea239-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="ea239-150">Citrix Sso.</span></span>|
|<span data-ttu-id="ea239-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="ea239-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="ea239-152">13</span><span class="sxs-lookup"><span data-stu-id="ea239-152">13</span></span>|<span data-ttu-id="ea239-153">帕洛阿尔托市网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="ea239-153">Palo Alto Networks GlobalProtect V2.</span></span>|





