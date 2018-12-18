---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定对于 VPN 通信规则路由的策略。
author: tfitzmac
ms.openlocfilehash: 5aa3f44f0e4ccf177154f97e9849093c52728b2e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343419"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="9f5ae-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9f5ae-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="9f5ae-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9f5ae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f5ae-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f5ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f5ae-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9f5ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f5ae-107">指定对于 VPN 通信规则路由的策略。</span><span class="sxs-lookup"><span data-stu-id="9f5ae-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="9f5ae-108">成员</span><span class="sxs-lookup"><span data-stu-id="9f5ae-108">Members</span></span>
|<span data-ttu-id="9f5ae-109">成员</span><span class="sxs-lookup"><span data-stu-id="9f5ae-109">Member</span></span>|<span data-ttu-id="9f5ae-110">值</span><span class="sxs-lookup"><span data-stu-id="9f5ae-110">Value</span></span>|<span data-ttu-id="9f5ae-111">说明</span><span class="sxs-lookup"><span data-stu-id="9f5ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f5ae-112">无</span><span class="sxs-lookup"><span data-stu-id="9f5ae-112">none</span></span>|<span data-ttu-id="9f5ae-113">0</span><span class="sxs-lookup"><span data-stu-id="9f5ae-113">0</span></span>|<span data-ttu-id="9f5ae-114">未指定的路由策略。</span><span class="sxs-lookup"><span data-stu-id="9f5ae-114">No routing policy specified.</span></span>|
|<span data-ttu-id="9f5ae-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="9f5ae-115">splitTunnel</span></span>|<span data-ttu-id="9f5ae-116">1</span><span class="sxs-lookup"><span data-stu-id="9f5ae-116">1</span></span>|<span data-ttu-id="9f5ae-117">指定的应用程序的网络流量将通过 VPN 进行路由。</span><span class="sxs-lookup"><span data-stu-id="9f5ae-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="9f5ae-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="9f5ae-118">forceTunnel</span></span>|<span data-ttu-id="9f5ae-119">2</span><span class="sxs-lookup"><span data-stu-id="9f5ae-119">2</span></span>|<span data-ttu-id="9f5ae-120">所有网络流量将通过 VPN 进行都路由。</span><span class="sxs-lookup"><span data-stu-id="9f5ae-120">All network traffic will be routed through the VPN.</span></span>|





