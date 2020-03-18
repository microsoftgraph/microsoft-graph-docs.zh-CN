---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3a5e514b5cbaecd2272c4bb94e2f21356633e8fb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786626"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="16d69-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="16d69-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="16d69-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16d69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16d69-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16d69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16d69-106">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="16d69-106">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="16d69-107">成员</span><span class="sxs-lookup"><span data-stu-id="16d69-107">Members</span></span>
|<span data-ttu-id="16d69-108">成员</span><span class="sxs-lookup"><span data-stu-id="16d69-108">Member</span></span>|<span data-ttu-id="16d69-109">值</span><span class="sxs-lookup"><span data-stu-id="16d69-109">Value</span></span>|<span data-ttu-id="16d69-110">说明</span><span class="sxs-lookup"><span data-stu-id="16d69-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16d69-111">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="16d69-111">pulseSecure</span></span>|<span data-ttu-id="16d69-112">0</span><span class="sxs-lookup"><span data-stu-id="16d69-112">0</span></span>|<span data-ttu-id="16d69-113">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="16d69-113">Pulse Secure.</span></span>|
|<span data-ttu-id="16d69-114">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="16d69-114">f5EdgeClient</span></span>|<span data-ttu-id="16d69-115">1</span><span class="sxs-lookup"><span data-stu-id="16d69-115">1</span></span>|<span data-ttu-id="16d69-116">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="16d69-116">F5 Edge Client.</span></span>|
|<span data-ttu-id="16d69-117">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="16d69-117">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="16d69-118">双面</span><span class="sxs-lookup"><span data-stu-id="16d69-118">2</span></span>|<span data-ttu-id="16d69-119">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="16d69-119">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="16d69-120">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="16d69-120">checkPointCapsuleVpn</span></span>|<span data-ttu-id="16d69-121">第三章</span><span class="sxs-lookup"><span data-stu-id="16d69-121">3</span></span>|<span data-ttu-id="16d69-122">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="16d69-122">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="16d69-123">自动</span><span class="sxs-lookup"><span data-stu-id="16d69-123">automatic</span></span>|<span data-ttu-id="16d69-124">4 </span><span class="sxs-lookup"><span data-stu-id="16d69-124">4</span></span>|<span data-ttu-id="16d69-125">自动。</span><span class="sxs-lookup"><span data-stu-id="16d69-125">Automatic.</span></span>|
|<span data-ttu-id="16d69-126">ikEv2</span><span class="sxs-lookup"><span data-stu-id="16d69-126">ikEv2</span></span>|<span data-ttu-id="16d69-127">5 </span><span class="sxs-lookup"><span data-stu-id="16d69-127">5</span></span>|<span data-ttu-id="16d69-128">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="16d69-128">IKEv2.</span></span>|
|<span data-ttu-id="16d69-129">l2tp</span><span class="sxs-lookup"><span data-stu-id="16d69-129">l2tp</span></span>|<span data-ttu-id="16d69-130">6 </span><span class="sxs-lookup"><span data-stu-id="16d69-130">6</span></span>|<span data-ttu-id="16d69-131">L2TP.</span><span class="sxs-lookup"><span data-stu-id="16d69-131">L2TP.</span></span>|
|<span data-ttu-id="16d69-132">pptp</span><span class="sxs-lookup"><span data-stu-id="16d69-132">pptp</span></span>|<span data-ttu-id="16d69-133">7 </span><span class="sxs-lookup"><span data-stu-id="16d69-133">7</span></span>|<span data-ttu-id="16d69-134">PPTP.</span><span class="sxs-lookup"><span data-stu-id="16d69-134">PPTP.</span></span>|
|<span data-ttu-id="16d69-135">citrix</span><span class="sxs-lookup"><span data-stu-id="16d69-135">citrix</span></span>|<span data-ttu-id="16d69-136">8 </span><span class="sxs-lookup"><span data-stu-id="16d69-136">8</span></span>|<span data-ttu-id="16d69-137">Citrix.</span><span class="sxs-lookup"><span data-stu-id="16d69-137">Citrix.</span></span>|
|<span data-ttu-id="16d69-138">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="16d69-138">paloAltoGlobalProtect</span></span>|<span data-ttu-id="16d69-139">9 </span><span class="sxs-lookup"><span data-stu-id="16d69-139">9</span></span>|<span data-ttu-id="16d69-140">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="16d69-140">Palo Alto Networks GlobalProtect.</span></span>|



