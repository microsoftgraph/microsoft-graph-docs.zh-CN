---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定 VPN 流量规则的路由策略。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d26e9c84f21fb952d4db58ef5faf28d1b696454
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529272"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="4c7fd-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4c7fd-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="4c7fd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4c7fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c7fd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4c7fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c7fd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c7fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c7fd-107">指定 VPN 流量规则的路由策略。</span><span class="sxs-lookup"><span data-stu-id="4c7fd-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="4c7fd-108">成员</span><span class="sxs-lookup"><span data-stu-id="4c7fd-108">Members</span></span>
|<span data-ttu-id="4c7fd-109">成员</span><span class="sxs-lookup"><span data-stu-id="4c7fd-109">Member</span></span>|<span data-ttu-id="4c7fd-110">值</span><span class="sxs-lookup"><span data-stu-id="4c7fd-110">Value</span></span>|<span data-ttu-id="4c7fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="4c7fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c7fd-112">无</span><span class="sxs-lookup"><span data-stu-id="4c7fd-112">none</span></span>|<span data-ttu-id="4c7fd-113">0</span><span class="sxs-lookup"><span data-stu-id="4c7fd-113">0</span></span>|<span data-ttu-id="4c7fd-114">未指定路由策略。</span><span class="sxs-lookup"><span data-stu-id="4c7fd-114">No routing policy specified.</span></span>|
|<span data-ttu-id="4c7fd-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="4c7fd-115">splitTunnel</span></span>|<span data-ttu-id="4c7fd-116">1 </span><span class="sxs-lookup"><span data-stu-id="4c7fd-116">1</span></span>|<span data-ttu-id="4c7fd-117">将通过 VPN 路由指定应用的网络流量。</span><span class="sxs-lookup"><span data-stu-id="4c7fd-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="4c7fd-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="4c7fd-118">forceTunnel</span></span>|<span data-ttu-id="4c7fd-119">2 </span><span class="sxs-lookup"><span data-stu-id="4c7fd-119">2</span></span>|<span data-ttu-id="4c7fd-120">所有网络流量将通过 VPN 路由。</span><span class="sxs-lookup"><span data-stu-id="4c7fd-120">All network traffic will be routed through the VPN.</span></span>|



