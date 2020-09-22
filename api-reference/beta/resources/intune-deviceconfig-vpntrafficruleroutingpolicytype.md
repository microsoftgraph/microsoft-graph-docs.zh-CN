---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定 VPN 流量规则的路由策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e5782555214897ec0513ab7293adf1d877ec5f96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042420"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="16be6-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="16be6-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="16be6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16be6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16be6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16be6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16be6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16be6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16be6-107">指定 VPN 流量规则的路由策略。</span><span class="sxs-lookup"><span data-stu-id="16be6-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="16be6-108">成员</span><span class="sxs-lookup"><span data-stu-id="16be6-108">Members</span></span>
|<span data-ttu-id="16be6-109">成员</span><span class="sxs-lookup"><span data-stu-id="16be6-109">Member</span></span>|<span data-ttu-id="16be6-110">值</span><span class="sxs-lookup"><span data-stu-id="16be6-110">Value</span></span>|<span data-ttu-id="16be6-111">说明</span><span class="sxs-lookup"><span data-stu-id="16be6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16be6-112">无</span><span class="sxs-lookup"><span data-stu-id="16be6-112">none</span></span>|<span data-ttu-id="16be6-113">0</span><span class="sxs-lookup"><span data-stu-id="16be6-113">0</span></span>|<span data-ttu-id="16be6-114">未指定路由策略。</span><span class="sxs-lookup"><span data-stu-id="16be6-114">No routing policy specified.</span></span>|
|<span data-ttu-id="16be6-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="16be6-115">splitTunnel</span></span>|<span data-ttu-id="16be6-116">1 </span><span class="sxs-lookup"><span data-stu-id="16be6-116">1</span></span>|<span data-ttu-id="16be6-117">将通过 VPN 路由指定应用的网络流量。</span><span class="sxs-lookup"><span data-stu-id="16be6-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="16be6-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="16be6-118">forceTunnel</span></span>|<span data-ttu-id="16be6-119">2 </span><span class="sxs-lookup"><span data-stu-id="16be6-119">2</span></span>|<span data-ttu-id="16be6-120">所有网络流量将通过 VPN 路由。</span><span class="sxs-lookup"><span data-stu-id="16be6-120">All network traffic will be routed through the VPN.</span></span>|






