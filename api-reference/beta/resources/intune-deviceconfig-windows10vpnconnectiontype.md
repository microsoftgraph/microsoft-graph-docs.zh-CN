---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b3114c5d608cfed786fab8d2734d723682670ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395935"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="19bbc-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="19bbc-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="19bbc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="19bbc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19bbc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="19bbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19bbc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19bbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19bbc-107">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="19bbc-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="19bbc-108">成员</span><span class="sxs-lookup"><span data-stu-id="19bbc-108">Members</span></span>
|<span data-ttu-id="19bbc-109">成员</span><span class="sxs-lookup"><span data-stu-id="19bbc-109">Member</span></span>|<span data-ttu-id="19bbc-110">值</span><span class="sxs-lookup"><span data-stu-id="19bbc-110">Value</span></span>|<span data-ttu-id="19bbc-111">说明</span><span class="sxs-lookup"><span data-stu-id="19bbc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19bbc-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="19bbc-112">pulseSecure</span></span>|<span data-ttu-id="19bbc-113">0</span><span class="sxs-lookup"><span data-stu-id="19bbc-113">0</span></span>|<span data-ttu-id="19bbc-114">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="19bbc-114">Pulse Secure.</span></span>|
|<span data-ttu-id="19bbc-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="19bbc-115">f5EdgeClient</span></span>|<span data-ttu-id="19bbc-116">1</span><span class="sxs-lookup"><span data-stu-id="19bbc-116">1</span></span>|<span data-ttu-id="19bbc-117">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="19bbc-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="19bbc-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="19bbc-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="19bbc-119">2</span><span class="sxs-lookup"><span data-stu-id="19bbc-119">2</span></span>|<span data-ttu-id="19bbc-120">Dell 使 SonicWALL Mobile 连接。</span><span class="sxs-lookup"><span data-stu-id="19bbc-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="19bbc-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="19bbc-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="19bbc-122">3</span><span class="sxs-lookup"><span data-stu-id="19bbc-122">3</span></span>|<span data-ttu-id="19bbc-123">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="19bbc-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="19bbc-124">自动</span><span class="sxs-lookup"><span data-stu-id="19bbc-124">automatic</span></span>|<span data-ttu-id="19bbc-125">4</span><span class="sxs-lookup"><span data-stu-id="19bbc-125">4</span></span>|<span data-ttu-id="19bbc-126">自动。</span><span class="sxs-lookup"><span data-stu-id="19bbc-126">Automatic.</span></span>|
|<span data-ttu-id="19bbc-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="19bbc-127">ikEv2</span></span>|<span data-ttu-id="19bbc-128">5</span><span class="sxs-lookup"><span data-stu-id="19bbc-128">5</span></span>|<span data-ttu-id="19bbc-129">IKEv2。</span><span class="sxs-lookup"><span data-stu-id="19bbc-129">IKEv2.</span></span>|
|<span data-ttu-id="19bbc-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="19bbc-130">l2tp</span></span>|<span data-ttu-id="19bbc-131">6</span><span class="sxs-lookup"><span data-stu-id="19bbc-131">6</span></span>|<span data-ttu-id="19bbc-132">L2TP。</span><span class="sxs-lookup"><span data-stu-id="19bbc-132">L2TP.</span></span>|
|<span data-ttu-id="19bbc-133">pptp</span><span class="sxs-lookup"><span data-stu-id="19bbc-133">pptp</span></span>|<span data-ttu-id="19bbc-134">7</span><span class="sxs-lookup"><span data-stu-id="19bbc-134">7</span></span>|<span data-ttu-id="19bbc-135">PPTP。</span><span class="sxs-lookup"><span data-stu-id="19bbc-135">PPTP.</span></span>|
|<span data-ttu-id="19bbc-136">citrix</span><span class="sxs-lookup"><span data-stu-id="19bbc-136">citrix</span></span>|<span data-ttu-id="19bbc-137">8</span><span class="sxs-lookup"><span data-stu-id="19bbc-137">8</span></span>|<span data-ttu-id="19bbc-138">Citrix。</span><span class="sxs-lookup"><span data-stu-id="19bbc-138">Citrix.</span></span>|
|<span data-ttu-id="19bbc-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="19bbc-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="19bbc-140">9</span><span class="sxs-lookup"><span data-stu-id="19bbc-140">9</span></span>|<span data-ttu-id="19bbc-141">帕罗奥市网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="19bbc-141">Palo Alto Networks GlobalProtect.</span></span>|




