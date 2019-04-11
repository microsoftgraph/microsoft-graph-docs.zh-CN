---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ac61b494fc261832a864c4c87998532a863f87b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774139"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="11ca1-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="11ca1-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="11ca1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11ca1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11ca1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11ca1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11ca1-106">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="11ca1-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="11ca1-107">成员</span><span class="sxs-lookup"><span data-stu-id="11ca1-107">Members</span></span>
|<span data-ttu-id="11ca1-108">成员</span><span class="sxs-lookup"><span data-stu-id="11ca1-108">Member</span></span>|<span data-ttu-id="11ca1-109">值</span><span class="sxs-lookup"><span data-stu-id="11ca1-109">Value</span></span>|<span data-ttu-id="11ca1-110">说明</span><span class="sxs-lookup"><span data-stu-id="11ca1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11ca1-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="11ca1-111">pulseSecure</span></span>|<span data-ttu-id="11ca1-112">0</span><span class="sxs-lookup"><span data-stu-id="11ca1-112">0</span></span>|<span data-ttu-id="11ca1-113">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="11ca1-113">Pulse Secure.</span></span>|
|<span data-ttu-id="11ca1-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="11ca1-114">f5EdgeClient</span></span>|<span data-ttu-id="11ca1-115">1</span><span class="sxs-lookup"><span data-stu-id="11ca1-115">1</span></span>|<span data-ttu-id="11ca1-116">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="11ca1-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="11ca1-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="11ca1-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="11ca1-118">双面</span><span class="sxs-lookup"><span data-stu-id="11ca1-118">2</span></span>|<span data-ttu-id="11ca1-119">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="11ca1-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="11ca1-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="11ca1-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="11ca1-121">第三章</span><span class="sxs-lookup"><span data-stu-id="11ca1-121">3</span></span>|<span data-ttu-id="11ca1-122">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="11ca1-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="11ca1-123">自动</span><span class="sxs-lookup"><span data-stu-id="11ca1-123">automatic</span></span>|<span data-ttu-id="11ca1-124">4</span><span class="sxs-lookup"><span data-stu-id="11ca1-124">4</span></span>|<span data-ttu-id="11ca1-125">自动。</span><span class="sxs-lookup"><span data-stu-id="11ca1-125">Automatic.</span></span>|
|<span data-ttu-id="11ca1-126">ikEv2</span><span class="sxs-lookup"><span data-stu-id="11ca1-126">ikEv2</span></span>|<span data-ttu-id="11ca1-127">5</span><span class="sxs-lookup"><span data-stu-id="11ca1-127">5</span></span>|<span data-ttu-id="11ca1-128">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="11ca1-128">IKEv2.</span></span>|
|<span data-ttu-id="11ca1-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="11ca1-129">l2tp</span></span>|<span data-ttu-id="11ca1-130">型</span><span class="sxs-lookup"><span data-stu-id="11ca1-130">6</span></span>|<span data-ttu-id="11ca1-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="11ca1-131">L2TP.</span></span>|
|<span data-ttu-id="11ca1-132">pptp</span><span class="sxs-lookup"><span data-stu-id="11ca1-132">pptp</span></span>|<span data-ttu-id="11ca1-133">步</span><span class="sxs-lookup"><span data-stu-id="11ca1-133">7</span></span>|<span data-ttu-id="11ca1-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="11ca1-134">PPTP.</span></span>|
|<span data-ttu-id="11ca1-135">citrix</span><span class="sxs-lookup"><span data-stu-id="11ca1-135">citrix</span></span>|<span data-ttu-id="11ca1-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="11ca1-136">8</span></span>|<span data-ttu-id="11ca1-137">Citrix.</span><span class="sxs-lookup"><span data-stu-id="11ca1-137">Citrix.</span></span>|
|<span data-ttu-id="11ca1-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="11ca1-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="11ca1-139">第</span><span class="sxs-lookup"><span data-stu-id="11ca1-139">9</span></span>|<span data-ttu-id="11ca1-140">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="11ca1-140">Palo Alto Networks GlobalProtect.</span></span>|





