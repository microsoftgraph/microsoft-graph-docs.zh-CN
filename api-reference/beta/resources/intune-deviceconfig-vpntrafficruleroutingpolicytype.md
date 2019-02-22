---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定 VPN 流量规则的路由策略。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a7c6121b9adc47d116a7b3321ca150a8d42449a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157342"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="f3e02-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f3e02-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="f3e02-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3e02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3e02-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3e02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3e02-106">指定 VPN 流量规则的路由策略。</span><span class="sxs-lookup"><span data-stu-id="f3e02-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="f3e02-107">成员</span><span class="sxs-lookup"><span data-stu-id="f3e02-107">Members</span></span>
|<span data-ttu-id="f3e02-108">成员</span><span class="sxs-lookup"><span data-stu-id="f3e02-108">Member</span></span>|<span data-ttu-id="f3e02-109">值</span><span class="sxs-lookup"><span data-stu-id="f3e02-109">Value</span></span>|<span data-ttu-id="f3e02-110">说明</span><span class="sxs-lookup"><span data-stu-id="f3e02-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3e02-111">无</span><span class="sxs-lookup"><span data-stu-id="f3e02-111">none</span></span>|<span data-ttu-id="f3e02-112">0</span><span class="sxs-lookup"><span data-stu-id="f3e02-112">0</span></span>|<span data-ttu-id="f3e02-113">未指定路由策略。</span><span class="sxs-lookup"><span data-stu-id="f3e02-113">No routing policy specified.</span></span>|
|<span data-ttu-id="f3e02-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="f3e02-114">splitTunnel</span></span>|<span data-ttu-id="f3e02-115">1</span><span class="sxs-lookup"><span data-stu-id="f3e02-115">1</span></span>|<span data-ttu-id="f3e02-116">将通过 VPN 路由指定应用的网络流量。</span><span class="sxs-lookup"><span data-stu-id="f3e02-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="f3e02-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="f3e02-117">forceTunnel</span></span>|<span data-ttu-id="f3e02-118">双面</span><span class="sxs-lookup"><span data-stu-id="f3e02-118">2</span></span>|<span data-ttu-id="f3e02-119">所有网络流量将通过 VPN 路由。</span><span class="sxs-lookup"><span data-stu-id="f3e02-119">All network traffic will be routed through the VPN.</span></span>|




