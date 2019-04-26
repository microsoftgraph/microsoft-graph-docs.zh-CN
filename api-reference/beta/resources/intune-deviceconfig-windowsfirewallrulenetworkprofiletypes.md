---
title: windowsFirewallRuleNetworkProfileTypes 枚举类型
description: 表示哪些网络配置文件类型适用于防火墙规则的标志。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cd5c501c50f74e53c0c00fcef2d3bb8a85cedf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570122"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="57ff0-103">windowsFirewallRuleNetworkProfileTypes 枚举类型</span><span class="sxs-lookup"><span data-stu-id="57ff0-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="57ff0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57ff0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57ff0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57ff0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57ff0-106">表示哪些网络配置文件类型适用于防火墙规则的标志。</span><span class="sxs-lookup"><span data-stu-id="57ff0-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="57ff0-107">成员</span><span class="sxs-lookup"><span data-stu-id="57ff0-107">Members</span></span>
|<span data-ttu-id="57ff0-108">成员</span><span class="sxs-lookup"><span data-stu-id="57ff0-108">Member</span></span>|<span data-ttu-id="57ff0-109">值</span><span class="sxs-lookup"><span data-stu-id="57ff0-109">Value</span></span>|<span data-ttu-id="57ff0-110">说明</span><span class="sxs-lookup"><span data-stu-id="57ff0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57ff0-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="57ff0-111">notConfigured</span></span>|<span data-ttu-id="57ff0-112">0</span><span class="sxs-lookup"><span data-stu-id="57ff0-112">0</span></span>|<span data-ttu-id="57ff0-113">未设置任何标志。</span><span class="sxs-lookup"><span data-stu-id="57ff0-113">No flags set.</span></span>|
|<span data-ttu-id="57ff0-114">domain</span><span class="sxs-lookup"><span data-stu-id="57ff0-114">domain</span></span>|<span data-ttu-id="57ff0-115">1</span><span class="sxs-lookup"><span data-stu-id="57ff0-115">1</span></span>|<span data-ttu-id="57ff0-116">连接到域的网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="57ff0-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="57ff0-117">private</span><span class="sxs-lookup"><span data-stu-id="57ff0-117">private</span></span>|<span data-ttu-id="57ff0-118">2 </span><span class="sxs-lookup"><span data-stu-id="57ff0-118">2</span></span>|<span data-ttu-id="57ff0-119">专用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="57ff0-119">The profile for private networks.</span></span>|
|<span data-ttu-id="57ff0-120">公开</span><span class="sxs-lookup"><span data-stu-id="57ff0-120">public</span></span>|<span data-ttu-id="57ff0-121">4 </span><span class="sxs-lookup"><span data-stu-id="57ff0-121">4</span></span>|<span data-ttu-id="57ff0-122">公用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="57ff0-122">The profile for public networks.</span></span>|





