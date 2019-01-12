---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 77b9fb91f86cfa29b13e58c9a4c1a4dff768c3a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937871"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="da16f-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="da16f-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="da16f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="da16f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da16f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da16f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da16f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="da16f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da16f-107">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="da16f-107">VPN connection types.</span></span>
## <a name="members"></a><span data-ttu-id="da16f-108">成员</span><span class="sxs-lookup"><span data-stu-id="da16f-108">Members</span></span>
|<span data-ttu-id="da16f-109">成员</span><span class="sxs-lookup"><span data-stu-id="da16f-109">Member</span></span>|<span data-ttu-id="da16f-110">值</span><span class="sxs-lookup"><span data-stu-id="da16f-110">Value</span></span>|<span data-ttu-id="da16f-111">Description</span><span class="sxs-lookup"><span data-stu-id="da16f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da16f-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="da16f-112">pulseSecure</span></span>|<span data-ttu-id="da16f-113">0</span><span class="sxs-lookup"><span data-stu-id="da16f-113">0</span></span>|<span data-ttu-id="da16f-114">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="da16f-114">Pulse Secure.</span></span>|
|<span data-ttu-id="da16f-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="da16f-115">f5EdgeClient</span></span>|<span data-ttu-id="da16f-116">1</span><span class="sxs-lookup"><span data-stu-id="da16f-116">1</span></span>|<span data-ttu-id="da16f-117">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="da16f-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="da16f-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="da16f-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="da16f-119">2</span><span class="sxs-lookup"><span data-stu-id="da16f-119">2</span></span>|<span data-ttu-id="da16f-120">Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="da16f-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="da16f-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="da16f-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="da16f-122">3</span><span class="sxs-lookup"><span data-stu-id="da16f-122">3</span></span>|<span data-ttu-id="da16f-123">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="da16f-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="da16f-124">automatic</span><span class="sxs-lookup"><span data-stu-id="da16f-124">automatic</span></span>|<span data-ttu-id="da16f-125">4</span><span class="sxs-lookup"><span data-stu-id="da16f-125">4</span></span>|<span data-ttu-id="da16f-126">自动。</span><span class="sxs-lookup"><span data-stu-id="da16f-126">Automatic.</span></span>|
|<span data-ttu-id="da16f-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="da16f-127">ikEv2</span></span>|<span data-ttu-id="da16f-128">5</span><span class="sxs-lookup"><span data-stu-id="da16f-128">5</span></span>|<span data-ttu-id="da16f-129">IKEv2。</span><span class="sxs-lookup"><span data-stu-id="da16f-129">IKEv2.</span></span>|
|<span data-ttu-id="da16f-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="da16f-130">l2tp</span></span>|<span data-ttu-id="da16f-131">6</span><span class="sxs-lookup"><span data-stu-id="da16f-131">6</span></span>|<span data-ttu-id="da16f-132">L2TP。</span><span class="sxs-lookup"><span data-stu-id="da16f-132">L2TP.</span></span>|
|<span data-ttu-id="da16f-133">pptp</span><span class="sxs-lookup"><span data-stu-id="da16f-133">pptp</span></span>|<span data-ttu-id="da16f-134">7</span><span class="sxs-lookup"><span data-stu-id="da16f-134">7</span></span>|<span data-ttu-id="da16f-135">PPTP。</span><span class="sxs-lookup"><span data-stu-id="da16f-135">PPTP.</span></span>|
|<span data-ttu-id="da16f-136">citrix</span><span class="sxs-lookup"><span data-stu-id="da16f-136">citrix</span></span>|<span data-ttu-id="da16f-137">8</span><span class="sxs-lookup"><span data-stu-id="da16f-137">8</span></span>|<span data-ttu-id="da16f-138">Citrix。</span><span class="sxs-lookup"><span data-stu-id="da16f-138">Citrix.</span></span>|
|<span data-ttu-id="da16f-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="da16f-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="da16f-140">9</span><span class="sxs-lookup"><span data-stu-id="da16f-140">9</span></span>|<span data-ttu-id="da16f-141">帕罗奥市网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="da16f-141">Palo Alto Networks GlobalProtect.</span></span>|





