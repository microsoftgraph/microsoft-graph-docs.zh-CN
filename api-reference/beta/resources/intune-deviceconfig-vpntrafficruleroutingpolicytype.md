---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定对于 VPN 通信规则路由的策略。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c8ec4303dc16c7cb0606e4b9cf86594446f571e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974950"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="7dca1-103">vpnTrafficRuleRoutingPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7dca1-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="7dca1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7dca1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7dca1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7dca1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7dca1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7dca1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7dca1-107">指定对于 VPN 通信规则路由的策略。</span><span class="sxs-lookup"><span data-stu-id="7dca1-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="7dca1-108">成员</span><span class="sxs-lookup"><span data-stu-id="7dca1-108">Members</span></span>
|<span data-ttu-id="7dca1-109">成员</span><span class="sxs-lookup"><span data-stu-id="7dca1-109">Member</span></span>|<span data-ttu-id="7dca1-110">值</span><span class="sxs-lookup"><span data-stu-id="7dca1-110">Value</span></span>|<span data-ttu-id="7dca1-111">说明</span><span class="sxs-lookup"><span data-stu-id="7dca1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dca1-112">无</span><span class="sxs-lookup"><span data-stu-id="7dca1-112">none</span></span>|<span data-ttu-id="7dca1-113">0</span><span class="sxs-lookup"><span data-stu-id="7dca1-113">0</span></span>|<span data-ttu-id="7dca1-114">未指定的路由策略。</span><span class="sxs-lookup"><span data-stu-id="7dca1-114">No routing policy specified.</span></span>|
|<span data-ttu-id="7dca1-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="7dca1-115">splitTunnel</span></span>|<span data-ttu-id="7dca1-116">1</span><span class="sxs-lookup"><span data-stu-id="7dca1-116">1</span></span>|<span data-ttu-id="7dca1-117">指定的应用程序的网络流量将通过 VPN 进行路由。</span><span class="sxs-lookup"><span data-stu-id="7dca1-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="7dca1-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="7dca1-118">forceTunnel</span></span>|<span data-ttu-id="7dca1-119">2</span><span class="sxs-lookup"><span data-stu-id="7dca1-119">2</span></span>|<span data-ttu-id="7dca1-120">所有网络流量将通过 VPN 进行都路由。</span><span class="sxs-lookup"><span data-stu-id="7dca1-120">All network traffic will be routed through the VPN.</span></span>|





