---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定 VPN 流量规则的路由策略。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5cbbba22017a40ae2f7db41e25f497c09156a2f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969371"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="2a610-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2a610-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="2a610-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a610-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a610-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a610-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a610-106">指定 VPN 流量规则的路由策略。</span><span class="sxs-lookup"><span data-stu-id="2a610-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="2a610-107">成员</span><span class="sxs-lookup"><span data-stu-id="2a610-107">Members</span></span>
|<span data-ttu-id="2a610-108">成员</span><span class="sxs-lookup"><span data-stu-id="2a610-108">Member</span></span>|<span data-ttu-id="2a610-109">值</span><span class="sxs-lookup"><span data-stu-id="2a610-109">Value</span></span>|<span data-ttu-id="2a610-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a610-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a610-111">无</span><span class="sxs-lookup"><span data-stu-id="2a610-111">none</span></span>|<span data-ttu-id="2a610-112">0</span><span class="sxs-lookup"><span data-stu-id="2a610-112">0</span></span>|<span data-ttu-id="2a610-113">未指定路由策略。</span><span class="sxs-lookup"><span data-stu-id="2a610-113">No routing policy specified.</span></span>|
|<span data-ttu-id="2a610-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="2a610-114">splitTunnel</span></span>|<span data-ttu-id="2a610-115">1</span><span class="sxs-lookup"><span data-stu-id="2a610-115">1</span></span>|<span data-ttu-id="2a610-116">将通过 VPN 路由指定应用的网络流量。</span><span class="sxs-lookup"><span data-stu-id="2a610-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="2a610-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="2a610-117">forceTunnel</span></span>|<span data-ttu-id="2a610-118">双面</span><span class="sxs-lookup"><span data-stu-id="2a610-118">2</span></span>|<span data-ttu-id="2a610-119">所有网络流量将通过 VPN 路由。</span><span class="sxs-lookup"><span data-stu-id="2a610-119">All network traffic will be routed through the VPN.</span></span>|





