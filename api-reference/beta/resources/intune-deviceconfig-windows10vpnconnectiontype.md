---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: tfitzmac
ms.openlocfilehash: 0452eff174cf12fdd7508e5000ed3fcbd9a01eeb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346429"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="b5e49-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b5e49-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="b5e49-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b5e49-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5e49-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5e49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5e49-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b5e49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5e49-107">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="b5e49-107">VPN connection types.</span></span>
## <a name="members"></a><span data-ttu-id="b5e49-108">成员</span><span class="sxs-lookup"><span data-stu-id="b5e49-108">Members</span></span>
|<span data-ttu-id="b5e49-109">成员</span><span class="sxs-lookup"><span data-stu-id="b5e49-109">Member</span></span>|<span data-ttu-id="b5e49-110">值</span><span class="sxs-lookup"><span data-stu-id="b5e49-110">Value</span></span>|<span data-ttu-id="b5e49-111">说明</span><span class="sxs-lookup"><span data-stu-id="b5e49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5e49-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="b5e49-112">pulseSecure</span></span>|<span data-ttu-id="b5e49-113">0</span><span class="sxs-lookup"><span data-stu-id="b5e49-113">0</span></span>|<span data-ttu-id="b5e49-114">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="b5e49-114">Pulse Secure.</span></span>|
|<span data-ttu-id="b5e49-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="b5e49-115">f5EdgeClient</span></span>|<span data-ttu-id="b5e49-116">1</span><span class="sxs-lookup"><span data-stu-id="b5e49-116">1</span></span>|<span data-ttu-id="b5e49-117">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="b5e49-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="b5e49-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="b5e49-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="b5e49-119">2</span><span class="sxs-lookup"><span data-stu-id="b5e49-119">2</span></span>|<span data-ttu-id="b5e49-120">Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="b5e49-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="b5e49-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="b5e49-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="b5e49-122">3</span><span class="sxs-lookup"><span data-stu-id="b5e49-122">3</span></span>|<span data-ttu-id="b5e49-123">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="b5e49-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="b5e49-124">automatic</span><span class="sxs-lookup"><span data-stu-id="b5e49-124">automatic</span></span>|<span data-ttu-id="b5e49-125">4</span><span class="sxs-lookup"><span data-stu-id="b5e49-125">4</span></span>|<span data-ttu-id="b5e49-126">自动。</span><span class="sxs-lookup"><span data-stu-id="b5e49-126">Automatic.</span></span>|
|<span data-ttu-id="b5e49-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="b5e49-127">ikEv2</span></span>|<span data-ttu-id="b5e49-128">5</span><span class="sxs-lookup"><span data-stu-id="b5e49-128">5</span></span>|<span data-ttu-id="b5e49-129">IKEv2。</span><span class="sxs-lookup"><span data-stu-id="b5e49-129">IKEv2.</span></span>|
|<span data-ttu-id="b5e49-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="b5e49-130">l2tp</span></span>|<span data-ttu-id="b5e49-131">6</span><span class="sxs-lookup"><span data-stu-id="b5e49-131">6</span></span>|<span data-ttu-id="b5e49-132">L2TP。</span><span class="sxs-lookup"><span data-stu-id="b5e49-132">L2TP.</span></span>|
|<span data-ttu-id="b5e49-133">pptp</span><span class="sxs-lookup"><span data-stu-id="b5e49-133">pptp</span></span>|<span data-ttu-id="b5e49-134">7</span><span class="sxs-lookup"><span data-stu-id="b5e49-134">7</span></span>|<span data-ttu-id="b5e49-135">PPTP。</span><span class="sxs-lookup"><span data-stu-id="b5e49-135">PPTP.</span></span>|
|<span data-ttu-id="b5e49-136">citrix</span><span class="sxs-lookup"><span data-stu-id="b5e49-136">citrix</span></span>|<span data-ttu-id="b5e49-137">8</span><span class="sxs-lookup"><span data-stu-id="b5e49-137">8</span></span>|<span data-ttu-id="b5e49-138">Citrix。</span><span class="sxs-lookup"><span data-stu-id="b5e49-138">Citrix.</span></span>|
|<span data-ttu-id="b5e49-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="b5e49-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="b5e49-140">9</span><span class="sxs-lookup"><span data-stu-id="b5e49-140">9</span></span>|<span data-ttu-id="b5e49-141">帕罗奥市网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="b5e49-141">Palo Alto Networks GlobalProtect.</span></span>|





