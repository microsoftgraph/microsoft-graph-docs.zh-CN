---
title: appleVpnConnectionType 枚举类型
description: Apple VPN 连接类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 94b39d6804a304cf84e6dbefa3ef715f837b55af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912692"
---
# <a name="applevpnconnectiontype-enum-type"></a><span data-ttu-id="3191b-103">appleVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3191b-103">appleVpnConnectionType enum type</span></span>

> <span data-ttu-id="3191b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3191b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3191b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3191b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3191b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3191b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3191b-107">Apple VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="3191b-107">Apple VPN connection type.</span></span>
## <a name="members"></a><span data-ttu-id="3191b-108">成员</span><span class="sxs-lookup"><span data-stu-id="3191b-108">Members</span></span>
|<span data-ttu-id="3191b-109">成员</span><span class="sxs-lookup"><span data-stu-id="3191b-109">Member</span></span>|<span data-ttu-id="3191b-110">值</span><span class="sxs-lookup"><span data-stu-id="3191b-110">Value</span></span>|<span data-ttu-id="3191b-111">Description</span><span class="sxs-lookup"><span data-stu-id="3191b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3191b-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="3191b-112">ciscoAnyConnect</span></span>|<span data-ttu-id="3191b-113">0</span><span class="sxs-lookup"><span data-stu-id="3191b-113">0</span></span>|<span data-ttu-id="3191b-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="3191b-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="3191b-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="3191b-115">pulseSecure</span></span>|<span data-ttu-id="3191b-116">1</span><span class="sxs-lookup"><span data-stu-id="3191b-116">1</span></span>|<span data-ttu-id="3191b-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="3191b-117">Pulse Secure.</span></span>|
|<span data-ttu-id="3191b-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="3191b-118">f5EdgeClient</span></span>|<span data-ttu-id="3191b-119">2</span><span class="sxs-lookup"><span data-stu-id="3191b-119">2</span></span>|<span data-ttu-id="3191b-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="3191b-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="3191b-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="3191b-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="3191b-122">3</span><span class="sxs-lookup"><span data-stu-id="3191b-122">3</span></span>|<span data-ttu-id="3191b-123">Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="3191b-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="3191b-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="3191b-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="3191b-125">4</span><span class="sxs-lookup"><span data-stu-id="3191b-125">4</span></span>|<span data-ttu-id="3191b-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="3191b-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="3191b-127">customVpn</span><span class="sxs-lookup"><span data-stu-id="3191b-127">customVpn</span></span>|<span data-ttu-id="3191b-128">5</span><span class="sxs-lookup"><span data-stu-id="3191b-128">5</span></span>|<span data-ttu-id="3191b-129">自定义 VPN。</span><span class="sxs-lookup"><span data-stu-id="3191b-129">Custom VPN.</span></span>|
|<span data-ttu-id="3191b-130">ciscoIPSec</span><span class="sxs-lookup"><span data-stu-id="3191b-130">ciscoIPSec</span></span>|<span data-ttu-id="3191b-131">6</span><span class="sxs-lookup"><span data-stu-id="3191b-131">6</span></span>|<span data-ttu-id="3191b-132">Cisco (IPSec)。</span><span class="sxs-lookup"><span data-stu-id="3191b-132">Cisco (IPSec).</span></span>|
|<span data-ttu-id="3191b-133">citrix</span><span class="sxs-lookup"><span data-stu-id="3191b-133">citrix</span></span>|<span data-ttu-id="3191b-134">7</span><span class="sxs-lookup"><span data-stu-id="3191b-134">7</span></span>|<span data-ttu-id="3191b-135">Citrix。</span><span class="sxs-lookup"><span data-stu-id="3191b-135">Citrix.</span></span>|
|<span data-ttu-id="3191b-136">ciscoAnyConnectV2</span><span class="sxs-lookup"><span data-stu-id="3191b-136">ciscoAnyConnectV2</span></span>|<span data-ttu-id="3191b-137">8</span><span class="sxs-lookup"><span data-stu-id="3191b-137">8</span></span>|<span data-ttu-id="3191b-138">Cisco AnyConnect V2。</span><span class="sxs-lookup"><span data-stu-id="3191b-138">Cisco AnyConnect V2.</span></span>|
|<span data-ttu-id="3191b-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="3191b-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="3191b-140">9</span><span class="sxs-lookup"><span data-stu-id="3191b-140">9</span></span>|<span data-ttu-id="3191b-141">帕罗奥市网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="3191b-141">Palo Alto Networks GlobalProtect.</span></span>|
|<span data-ttu-id="3191b-142">zscalerPrivateAccess</span><span class="sxs-lookup"><span data-stu-id="3191b-142">zscalerPrivateAccess</span></span>|<span data-ttu-id="3191b-143">10</span><span class="sxs-lookup"><span data-stu-id="3191b-143">10</span></span>|<span data-ttu-id="3191b-144">Zscaler 专用访问。</span><span class="sxs-lookup"><span data-stu-id="3191b-144">Zscaler Private Access.</span></span>|
|<span data-ttu-id="3191b-145">f5Access2018</span><span class="sxs-lookup"><span data-stu-id="3191b-145">f5Access2018</span></span>|<span data-ttu-id="3191b-146">11</span><span class="sxs-lookup"><span data-stu-id="3191b-146">11</span></span>|<span data-ttu-id="3191b-147">F5 访问 2018。</span><span class="sxs-lookup"><span data-stu-id="3191b-147">F5 Access 2018.</span></span>|
|<span data-ttu-id="3191b-148">citrixSso</span><span class="sxs-lookup"><span data-stu-id="3191b-148">citrixSso</span></span>|<span data-ttu-id="3191b-149">12</span><span class="sxs-lookup"><span data-stu-id="3191b-149">12</span></span>|<span data-ttu-id="3191b-150">Citrix Sso。</span><span class="sxs-lookup"><span data-stu-id="3191b-150">Citrix Sso.</span></span>|
|<span data-ttu-id="3191b-151">paloAltoGlobalProtectV2</span><span class="sxs-lookup"><span data-stu-id="3191b-151">paloAltoGlobalProtectV2</span></span>|<span data-ttu-id="3191b-152">13</span><span class="sxs-lookup"><span data-stu-id="3191b-152">13</span></span>|<span data-ttu-id="3191b-153">帕洛阿尔托市网络 GlobalProtect V2。</span><span class="sxs-lookup"><span data-stu-id="3191b-153">Palo Alto Networks GlobalProtect V2.</span></span>|





