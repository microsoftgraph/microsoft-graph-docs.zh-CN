---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定 VPN 流量规则的路由策略。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 529c42722d8ce3827bb9daa4c0f158cfd92d8383
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367517"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="92999-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="92999-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="92999-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92999-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92999-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92999-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92999-106">指定 VPN 流量规则的路由策略。</span><span class="sxs-lookup"><span data-stu-id="92999-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="92999-107">成员</span><span class="sxs-lookup"><span data-stu-id="92999-107">Members</span></span>
|<span data-ttu-id="92999-108">成员</span><span class="sxs-lookup"><span data-stu-id="92999-108">Member</span></span>|<span data-ttu-id="92999-109">值</span><span class="sxs-lookup"><span data-stu-id="92999-109">Value</span></span>|<span data-ttu-id="92999-110">说明</span><span class="sxs-lookup"><span data-stu-id="92999-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92999-111">无</span><span class="sxs-lookup"><span data-stu-id="92999-111">none</span></span>|<span data-ttu-id="92999-112">0</span><span class="sxs-lookup"><span data-stu-id="92999-112">0</span></span>|<span data-ttu-id="92999-113">未指定路由策略。</span><span class="sxs-lookup"><span data-stu-id="92999-113">No routing policy specified.</span></span>|
|<span data-ttu-id="92999-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="92999-114">splitTunnel</span></span>|<span data-ttu-id="92999-115">1</span><span class="sxs-lookup"><span data-stu-id="92999-115">1</span></span>|<span data-ttu-id="92999-116">将通过 VPN 路由指定应用的网络流量。</span><span class="sxs-lookup"><span data-stu-id="92999-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="92999-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="92999-117">forceTunnel</span></span>|<span data-ttu-id="92999-118">双面</span><span class="sxs-lookup"><span data-stu-id="92999-118">2</span></span>|<span data-ttu-id="92999-119">所有网络流量将通过 VPN 路由。</span><span class="sxs-lookup"><span data-stu-id="92999-119">All network traffic will be routed through the VPN.</span></span>|



