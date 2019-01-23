---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定对于 VPN 通信规则路由的策略。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 028e49085e4a1fa5f01ac59ff00fbafd8846dfb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415003"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="492a0-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="492a0-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="492a0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="492a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="492a0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="492a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="492a0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="492a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="492a0-107">指定对于 VPN 通信规则路由的策略。</span><span class="sxs-lookup"><span data-stu-id="492a0-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="492a0-108">成员</span><span class="sxs-lookup"><span data-stu-id="492a0-108">Members</span></span>
|<span data-ttu-id="492a0-109">成员</span><span class="sxs-lookup"><span data-stu-id="492a0-109">Member</span></span>|<span data-ttu-id="492a0-110">值</span><span class="sxs-lookup"><span data-stu-id="492a0-110">Value</span></span>|<span data-ttu-id="492a0-111">说明</span><span class="sxs-lookup"><span data-stu-id="492a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="492a0-112">无</span><span class="sxs-lookup"><span data-stu-id="492a0-112">none</span></span>|<span data-ttu-id="492a0-113">0</span><span class="sxs-lookup"><span data-stu-id="492a0-113">0</span></span>|<span data-ttu-id="492a0-114">未指定的路由策略。</span><span class="sxs-lookup"><span data-stu-id="492a0-114">No routing policy specified.</span></span>|
|<span data-ttu-id="492a0-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="492a0-115">splitTunnel</span></span>|<span data-ttu-id="492a0-116">1</span><span class="sxs-lookup"><span data-stu-id="492a0-116">1</span></span>|<span data-ttu-id="492a0-117">指定的应用程序的网络流量将通过 VPN 进行路由。</span><span class="sxs-lookup"><span data-stu-id="492a0-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="492a0-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="492a0-118">forceTunnel</span></span>|<span data-ttu-id="492a0-119">2</span><span class="sxs-lookup"><span data-stu-id="492a0-119">2</span></span>|<span data-ttu-id="492a0-120">所有网络流量将通过 VPN 进行都路由。</span><span class="sxs-lookup"><span data-stu-id="492a0-120">All network traffic will be routed through the VPN.</span></span>|




