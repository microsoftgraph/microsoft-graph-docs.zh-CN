---
title: windowsFirewallRuleNetworkProfileTypes 枚举类型
description: 表示哪些网络配置文件类型适用于防火墙规则的标志。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cd5c501c50f74e53c0c00fcef2d3bb8a85cedf7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804646"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="f8629-103">windowsFirewallRuleNetworkProfileTypes 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f8629-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="f8629-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f8629-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8629-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8629-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8629-106">表示哪些网络配置文件类型适用于防火墙规则的标志。</span><span class="sxs-lookup"><span data-stu-id="f8629-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="f8629-107">成员</span><span class="sxs-lookup"><span data-stu-id="f8629-107">Members</span></span>
|<span data-ttu-id="f8629-108">成员</span><span class="sxs-lookup"><span data-stu-id="f8629-108">Member</span></span>|<span data-ttu-id="f8629-109">值</span><span class="sxs-lookup"><span data-stu-id="f8629-109">Value</span></span>|<span data-ttu-id="f8629-110">说明</span><span class="sxs-lookup"><span data-stu-id="f8629-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8629-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f8629-111">notConfigured</span></span>|<span data-ttu-id="f8629-112">0</span><span class="sxs-lookup"><span data-stu-id="f8629-112">0</span></span>|<span data-ttu-id="f8629-113">未设置任何标志。</span><span class="sxs-lookup"><span data-stu-id="f8629-113">No flags set.</span></span>|
|<span data-ttu-id="f8629-114">domain</span><span class="sxs-lookup"><span data-stu-id="f8629-114">domain</span></span>|<span data-ttu-id="f8629-115">1</span><span class="sxs-lookup"><span data-stu-id="f8629-115">1</span></span>|<span data-ttu-id="f8629-116">连接到域的网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="f8629-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="f8629-117">private</span><span class="sxs-lookup"><span data-stu-id="f8629-117">private</span></span>|<span data-ttu-id="f8629-118">双面</span><span class="sxs-lookup"><span data-stu-id="f8629-118">2</span></span>|<span data-ttu-id="f8629-119">专用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="f8629-119">The profile for private networks.</span></span>|
|<span data-ttu-id="f8629-120">公开</span><span class="sxs-lookup"><span data-stu-id="f8629-120">public</span></span>|<span data-ttu-id="f8629-121">4</span><span class="sxs-lookup"><span data-stu-id="f8629-121">4</span></span>|<span data-ttu-id="f8629-122">公用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="f8629-122">The profile for public networks.</span></span>|





