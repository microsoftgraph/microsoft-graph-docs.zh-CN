---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定 VPN 流量规则的路由策略。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 360a7ea9ab46a9d482fd8e41c2d2a64041453e88
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777779"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="89829-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89829-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="89829-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89829-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89829-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89829-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89829-106">指定 VPN 流量规则的路由策略。</span><span class="sxs-lookup"><span data-stu-id="89829-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="89829-107">成员</span><span class="sxs-lookup"><span data-stu-id="89829-107">Members</span></span>
|<span data-ttu-id="89829-108">成员</span><span class="sxs-lookup"><span data-stu-id="89829-108">Member</span></span>|<span data-ttu-id="89829-109">值</span><span class="sxs-lookup"><span data-stu-id="89829-109">Value</span></span>|<span data-ttu-id="89829-110">说明</span><span class="sxs-lookup"><span data-stu-id="89829-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89829-111">无</span><span class="sxs-lookup"><span data-stu-id="89829-111">none</span></span>|<span data-ttu-id="89829-112">0</span><span class="sxs-lookup"><span data-stu-id="89829-112">0</span></span>|<span data-ttu-id="89829-113">未指定路由策略。</span><span class="sxs-lookup"><span data-stu-id="89829-113">No routing policy specified.</span></span>|
|<span data-ttu-id="89829-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="89829-114">splitTunnel</span></span>|<span data-ttu-id="89829-115">1</span><span class="sxs-lookup"><span data-stu-id="89829-115">1</span></span>|<span data-ttu-id="89829-116">将通过 VPN 路由指定应用的网络流量。</span><span class="sxs-lookup"><span data-stu-id="89829-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="89829-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="89829-117">forceTunnel</span></span>|<span data-ttu-id="89829-118">双面</span><span class="sxs-lookup"><span data-stu-id="89829-118">2</span></span>|<span data-ttu-id="89829-119">所有网络流量将通过 VPN 路由。</span><span class="sxs-lookup"><span data-stu-id="89829-119">All network traffic will be routed through the VPN.</span></span>|





