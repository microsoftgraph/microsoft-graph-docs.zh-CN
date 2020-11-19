---
title: androidVpnConnectionType 枚举类型
description: Android VPN 连接类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7aa0419c25ea2865e732dc54c331389cab5740fe
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284006"
---
# <a name="androidvpnconnectiontype-enum-type"></a><span data-ttu-id="f9889-103">androidVpnConnectionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f9889-103">androidVpnConnectionType enum type</span></span>

<span data-ttu-id="f9889-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9889-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9889-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9889-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9889-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9889-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9889-107">Android VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="f9889-107">Android VPN connection type.</span></span>

## <a name="members"></a><span data-ttu-id="f9889-108">成员</span><span class="sxs-lookup"><span data-stu-id="f9889-108">Members</span></span>
|<span data-ttu-id="f9889-109">成员</span><span class="sxs-lookup"><span data-stu-id="f9889-109">Member</span></span>|<span data-ttu-id="f9889-110">值</span><span class="sxs-lookup"><span data-stu-id="f9889-110">Value</span></span>|<span data-ttu-id="f9889-111">Description</span><span class="sxs-lookup"><span data-stu-id="f9889-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9889-112">ciscoAnyConnect</span><span class="sxs-lookup"><span data-stu-id="f9889-112">ciscoAnyConnect</span></span>|<span data-ttu-id="f9889-113">0</span><span class="sxs-lookup"><span data-stu-id="f9889-113">0</span></span>|<span data-ttu-id="f9889-114">Cisco AnyConnect。</span><span class="sxs-lookup"><span data-stu-id="f9889-114">Cisco AnyConnect.</span></span>|
|<span data-ttu-id="f9889-115">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="f9889-115">pulseSecure</span></span>|<span data-ttu-id="f9889-116">1</span><span class="sxs-lookup"><span data-stu-id="f9889-116">1</span></span>|<span data-ttu-id="f9889-117">脉冲安全。</span><span class="sxs-lookup"><span data-stu-id="f9889-117">Pulse Secure.</span></span>|
|<span data-ttu-id="f9889-118">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="f9889-118">f5EdgeClient</span></span>|<span data-ttu-id="f9889-119">双面</span><span class="sxs-lookup"><span data-stu-id="f9889-119">2</span></span>|<span data-ttu-id="f9889-120">F5 边缘客户端。</span><span class="sxs-lookup"><span data-stu-id="f9889-120">F5 Edge Client.</span></span>|
|<span data-ttu-id="f9889-121">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="f9889-121">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="f9889-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f9889-122">3</span></span>|<span data-ttu-id="f9889-123">戴尔 SonicWALL 移动连接。</span><span class="sxs-lookup"><span data-stu-id="f9889-123">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="f9889-124">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="f9889-124">checkPointCapsuleVpn</span></span>|<span data-ttu-id="f9889-125">4 </span><span class="sxs-lookup"><span data-stu-id="f9889-125">4</span></span>|<span data-ttu-id="f9889-126">检查点胶囊 VPN。</span><span class="sxs-lookup"><span data-stu-id="f9889-126">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="f9889-127">citrix</span><span class="sxs-lookup"><span data-stu-id="f9889-127">citrix</span></span>|<span data-ttu-id="f9889-128">5 </span><span class="sxs-lookup"><span data-stu-id="f9889-128">5</span></span>|<span data-ttu-id="f9889-129">Citrix</span><span class="sxs-lookup"><span data-stu-id="f9889-129">Citrix</span></span>|
|<span data-ttu-id="f9889-130">microsoftTunnel</span><span class="sxs-lookup"><span data-stu-id="f9889-130">microsoftTunnel</span></span>|<span data-ttu-id="f9889-131">7 </span><span class="sxs-lookup"><span data-stu-id="f9889-131">7</span></span>|<span data-ttu-id="f9889-132">Microsoft 隧道。</span><span class="sxs-lookup"><span data-stu-id="f9889-132">Microsoft Tunnel.</span></span>|
|<span data-ttu-id="f9889-133">netMotionMobility</span><span class="sxs-lookup"><span data-stu-id="f9889-133">netMotionMobility</span></span>|<span data-ttu-id="f9889-134">8 </span><span class="sxs-lookup"><span data-stu-id="f9889-134">8</span></span>|<span data-ttu-id="f9889-135">NetMotion 移动性。</span><span class="sxs-lookup"><span data-stu-id="f9889-135">NetMotion Mobility.</span></span>|




