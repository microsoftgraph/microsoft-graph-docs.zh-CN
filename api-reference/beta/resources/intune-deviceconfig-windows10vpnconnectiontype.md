---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6a31c72f9c8dbb3d63d94c6c4f83e060fd80e0f1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729596"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="46e6f-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="46e6f-103">windows10VpnConnectionType enum type</span></span>

<span data-ttu-id="46e6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46e6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46e6f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46e6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46e6f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46e6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46e6f-107">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="46e6f-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="46e6f-108">成员</span><span class="sxs-lookup"><span data-stu-id="46e6f-108">Members</span></span>
|<span data-ttu-id="46e6f-109">成员</span><span class="sxs-lookup"><span data-stu-id="46e6f-109">Member</span></span>|<span data-ttu-id="46e6f-110">值</span><span class="sxs-lookup"><span data-stu-id="46e6f-110">Value</span></span>|<span data-ttu-id="46e6f-111">说明</span><span class="sxs-lookup"><span data-stu-id="46e6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46e6f-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="46e6f-112">pulseSecure</span></span>|<span data-ttu-id="46e6f-113">0</span><span class="sxs-lookup"><span data-stu-id="46e6f-113">0</span></span>|<span data-ttu-id="46e6f-114">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="46e6f-114">Pulse Secure.</span></span>|
|<span data-ttu-id="46e6f-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="46e6f-115">f5EdgeClient</span></span>|<span data-ttu-id="46e6f-116">1</span><span class="sxs-lookup"><span data-stu-id="46e6f-116">1</span></span>|<span data-ttu-id="46e6f-117">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="46e6f-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="46e6f-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="46e6f-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="46e6f-119">双面</span><span class="sxs-lookup"><span data-stu-id="46e6f-119">2</span></span>|<span data-ttu-id="46e6f-120">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="46e6f-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="46e6f-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="46e6f-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="46e6f-122">第三章</span><span class="sxs-lookup"><span data-stu-id="46e6f-122">3</span></span>|<span data-ttu-id="46e6f-123">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="46e6f-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="46e6f-124">自动</span><span class="sxs-lookup"><span data-stu-id="46e6f-124">automatic</span></span>|<span data-ttu-id="46e6f-125">4 </span><span class="sxs-lookup"><span data-stu-id="46e6f-125">4</span></span>|<span data-ttu-id="46e6f-126">自动。</span><span class="sxs-lookup"><span data-stu-id="46e6f-126">Automatic.</span></span>|
|<span data-ttu-id="46e6f-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="46e6f-127">ikEv2</span></span>|<span data-ttu-id="46e6f-128">5 </span><span class="sxs-lookup"><span data-stu-id="46e6f-128">5</span></span>|<span data-ttu-id="46e6f-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="46e6f-129">IKEv2.</span></span>|
|<span data-ttu-id="46e6f-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="46e6f-130">l2tp</span></span>|<span data-ttu-id="46e6f-131">6 </span><span class="sxs-lookup"><span data-stu-id="46e6f-131">6</span></span>|<span data-ttu-id="46e6f-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="46e6f-132">L2TP.</span></span>|
|<span data-ttu-id="46e6f-133">pptp</span><span class="sxs-lookup"><span data-stu-id="46e6f-133">pptp</span></span>|<span data-ttu-id="46e6f-134">7 </span><span class="sxs-lookup"><span data-stu-id="46e6f-134">7</span></span>|<span data-ttu-id="46e6f-135">PPTP.</span><span class="sxs-lookup"><span data-stu-id="46e6f-135">PPTP.</span></span>|
|<span data-ttu-id="46e6f-136">citrix</span><span class="sxs-lookup"><span data-stu-id="46e6f-136">citrix</span></span>|<span data-ttu-id="46e6f-137">8 </span><span class="sxs-lookup"><span data-stu-id="46e6f-137">8</span></span>|<span data-ttu-id="46e6f-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="46e6f-138">Citrix.</span></span>|
|<span data-ttu-id="46e6f-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="46e6f-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="46e6f-140">9 </span><span class="sxs-lookup"><span data-stu-id="46e6f-140">9</span></span>|<span data-ttu-id="46e6f-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="46e6f-141">Palo Alto Networks GlobalProtect.</span></span>|





