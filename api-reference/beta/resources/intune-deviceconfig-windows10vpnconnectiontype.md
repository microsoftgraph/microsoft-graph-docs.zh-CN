---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e464f8136c069edd94d7ebacf9946d6648028dc6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529160"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="cc789-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cc789-103">windows10VpnConnectionType enum type</span></span>

<span data-ttu-id="cc789-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cc789-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc789-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc789-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc789-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc789-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc789-107">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="cc789-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="cc789-108">成员</span><span class="sxs-lookup"><span data-stu-id="cc789-108">Members</span></span>
|<span data-ttu-id="cc789-109">成员</span><span class="sxs-lookup"><span data-stu-id="cc789-109">Member</span></span>|<span data-ttu-id="cc789-110">值</span><span class="sxs-lookup"><span data-stu-id="cc789-110">Value</span></span>|<span data-ttu-id="cc789-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc789-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc789-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="cc789-112">pulseSecure</span></span>|<span data-ttu-id="cc789-113">0</span><span class="sxs-lookup"><span data-stu-id="cc789-113">0</span></span>|<span data-ttu-id="cc789-114">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="cc789-114">Pulse Secure.</span></span>|
|<span data-ttu-id="cc789-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="cc789-115">f5EdgeClient</span></span>|<span data-ttu-id="cc789-116">1 </span><span class="sxs-lookup"><span data-stu-id="cc789-116">1</span></span>|<span data-ttu-id="cc789-117">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="cc789-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="cc789-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="cc789-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="cc789-119">2 </span><span class="sxs-lookup"><span data-stu-id="cc789-119">2</span></span>|<span data-ttu-id="cc789-120">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="cc789-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="cc789-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="cc789-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="cc789-122">3 </span><span class="sxs-lookup"><span data-stu-id="cc789-122">3</span></span>|<span data-ttu-id="cc789-123">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="cc789-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="cc789-124">自动</span><span class="sxs-lookup"><span data-stu-id="cc789-124">automatic</span></span>|<span data-ttu-id="cc789-125">4 </span><span class="sxs-lookup"><span data-stu-id="cc789-125">4</span></span>|<span data-ttu-id="cc789-126">自动。</span><span class="sxs-lookup"><span data-stu-id="cc789-126">Automatic.</span></span>|
|<span data-ttu-id="cc789-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="cc789-127">ikEv2</span></span>|<span data-ttu-id="cc789-128">5 </span><span class="sxs-lookup"><span data-stu-id="cc789-128">5</span></span>|<span data-ttu-id="cc789-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="cc789-129">IKEv2.</span></span>|
|<span data-ttu-id="cc789-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="cc789-130">l2tp</span></span>|<span data-ttu-id="cc789-131">6 </span><span class="sxs-lookup"><span data-stu-id="cc789-131">6</span></span>|<span data-ttu-id="cc789-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="cc789-132">L2TP.</span></span>|
|<span data-ttu-id="cc789-133">pptp</span><span class="sxs-lookup"><span data-stu-id="cc789-133">pptp</span></span>|<span data-ttu-id="cc789-134">7 </span><span class="sxs-lookup"><span data-stu-id="cc789-134">7</span></span>|<span data-ttu-id="cc789-135">PPTP.</span><span class="sxs-lookup"><span data-stu-id="cc789-135">PPTP.</span></span>|
|<span data-ttu-id="cc789-136">citrix</span><span class="sxs-lookup"><span data-stu-id="cc789-136">citrix</span></span>|<span data-ttu-id="cc789-137">8 </span><span class="sxs-lookup"><span data-stu-id="cc789-137">8</span></span>|<span data-ttu-id="cc789-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="cc789-138">Citrix.</span></span>|
|<span data-ttu-id="cc789-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="cc789-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="cc789-140">9 </span><span class="sxs-lookup"><span data-stu-id="cc789-140">9</span></span>|<span data-ttu-id="cc789-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="cc789-141">Palo Alto Networks GlobalProtect.</span></span>|



