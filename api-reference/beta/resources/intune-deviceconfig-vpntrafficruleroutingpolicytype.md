---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定 VPN 流量规则的路由策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 670fa329323d169a49bab68876cd12d35289f5ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724521"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="9b78a-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9b78a-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="9b78a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b78a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b78a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b78a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b78a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b78a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b78a-107">指定 VPN 流量规则的路由策略。</span><span class="sxs-lookup"><span data-stu-id="9b78a-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="9b78a-108">成员</span><span class="sxs-lookup"><span data-stu-id="9b78a-108">Members</span></span>
|<span data-ttu-id="9b78a-109">成员</span><span class="sxs-lookup"><span data-stu-id="9b78a-109">Member</span></span>|<span data-ttu-id="9b78a-110">值</span><span class="sxs-lookup"><span data-stu-id="9b78a-110">Value</span></span>|<span data-ttu-id="9b78a-111">说明</span><span class="sxs-lookup"><span data-stu-id="9b78a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b78a-112">无</span><span class="sxs-lookup"><span data-stu-id="9b78a-112">none</span></span>|<span data-ttu-id="9b78a-113">0</span><span class="sxs-lookup"><span data-stu-id="9b78a-113">0</span></span>|<span data-ttu-id="9b78a-114">未指定路由策略。</span><span class="sxs-lookup"><span data-stu-id="9b78a-114">No routing policy specified.</span></span>|
|<span data-ttu-id="9b78a-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="9b78a-115">splitTunnel</span></span>|<span data-ttu-id="9b78a-116">1</span><span class="sxs-lookup"><span data-stu-id="9b78a-116">1</span></span>|<span data-ttu-id="9b78a-117">将通过 VPN 路由指定应用的网络流量。</span><span class="sxs-lookup"><span data-stu-id="9b78a-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="9b78a-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="9b78a-118">forceTunnel</span></span>|<span data-ttu-id="9b78a-119">双面</span><span class="sxs-lookup"><span data-stu-id="9b78a-119">2</span></span>|<span data-ttu-id="9b78a-120">所有网络流量将通过 VPN 路由。</span><span class="sxs-lookup"><span data-stu-id="9b78a-120">All network traffic will be routed through the VPN.</span></span>|





