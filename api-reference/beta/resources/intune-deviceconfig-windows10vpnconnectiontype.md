---
title: windows10VpnConnectionType 枚举类型
description: VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 77eb25bbf1d77d1c0316f8970280943b4dcdb282
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272554"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="2060c-103">windows10VpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2060c-103">windows10VpnConnectionType enum type</span></span>

<span data-ttu-id="2060c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2060c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2060c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2060c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2060c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2060c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2060c-107">VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="2060c-107">VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="2060c-108">成员</span><span class="sxs-lookup"><span data-stu-id="2060c-108">Members</span></span>
|<span data-ttu-id="2060c-109">成员</span><span class="sxs-lookup"><span data-stu-id="2060c-109">Member</span></span>|<span data-ttu-id="2060c-110">值</span><span class="sxs-lookup"><span data-stu-id="2060c-110">Value</span></span>|<span data-ttu-id="2060c-111">说明</span><span class="sxs-lookup"><span data-stu-id="2060c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2060c-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="2060c-112">pulseSecure</span></span>|<span data-ttu-id="2060c-113">0</span><span class="sxs-lookup"><span data-stu-id="2060c-113">0</span></span>|<span data-ttu-id="2060c-114">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="2060c-114">Pulse Secure.</span></span>|
|<span data-ttu-id="2060c-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="2060c-115">f5EdgeClient</span></span>|<span data-ttu-id="2060c-116">1</span><span class="sxs-lookup"><span data-stu-id="2060c-116">1</span></span>|<span data-ttu-id="2060c-117">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="2060c-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="2060c-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="2060c-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="2060c-119">双面</span><span class="sxs-lookup"><span data-stu-id="2060c-119">2</span></span>|<span data-ttu-id="2060c-120">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="2060c-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="2060c-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="2060c-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="2060c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="2060c-122">3</span></span>|<span data-ttu-id="2060c-123">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="2060c-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="2060c-124">自动</span><span class="sxs-lookup"><span data-stu-id="2060c-124">automatic</span></span>|<span data-ttu-id="2060c-125">4 </span><span class="sxs-lookup"><span data-stu-id="2060c-125">4</span></span>|<span data-ttu-id="2060c-126">自动。</span><span class="sxs-lookup"><span data-stu-id="2060c-126">Automatic.</span></span>|
|<span data-ttu-id="2060c-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="2060c-127">ikEv2</span></span>|<span data-ttu-id="2060c-128">5 </span><span class="sxs-lookup"><span data-stu-id="2060c-128">5</span></span>|<span data-ttu-id="2060c-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="2060c-129">IKEv2.</span></span>|
|<span data-ttu-id="2060c-130">l2tp</span><span class="sxs-lookup"><span data-stu-id="2060c-130">l2tp</span></span>|<span data-ttu-id="2060c-131">6 </span><span class="sxs-lookup"><span data-stu-id="2060c-131">6</span></span>|<span data-ttu-id="2060c-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="2060c-132">L2TP.</span></span>|
|<span data-ttu-id="2060c-133">pptp</span><span class="sxs-lookup"><span data-stu-id="2060c-133">pptp</span></span>|<span data-ttu-id="2060c-134">7 </span><span class="sxs-lookup"><span data-stu-id="2060c-134">7</span></span>|<span data-ttu-id="2060c-135">PPTP.</span><span class="sxs-lookup"><span data-stu-id="2060c-135">PPTP.</span></span>|
|<span data-ttu-id="2060c-136">citrix</span><span class="sxs-lookup"><span data-stu-id="2060c-136">citrix</span></span>|<span data-ttu-id="2060c-137">8 </span><span class="sxs-lookup"><span data-stu-id="2060c-137">8</span></span>|<span data-ttu-id="2060c-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="2060c-138">Citrix.</span></span>|
|<span data-ttu-id="2060c-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="2060c-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="2060c-140">9 </span><span class="sxs-lookup"><span data-stu-id="2060c-140">9</span></span>|<span data-ttu-id="2060c-141">Palo Alto 网络 GlobalProtect。</span><span class="sxs-lookup"><span data-stu-id="2060c-141">Palo Alto Networks GlobalProtect.</span></span>|




