---
title: windowsFirewallRuleNetworkProfileTypes 枚举类型
description: 表示哪些网络配置文件类型适用于防火墙规则的标志。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4d2a7a10936df83300c432ea9412790ba33ccc1c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786486"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="d2db4-103">windowsFirewallRuleNetworkProfileTypes 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d2db4-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="d2db4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d2db4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2db4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2db4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2db4-106">表示哪些网络配置文件类型适用于防火墙规则的标志。</span><span class="sxs-lookup"><span data-stu-id="d2db4-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="d2db4-107">成员</span><span class="sxs-lookup"><span data-stu-id="d2db4-107">Members</span></span>
|<span data-ttu-id="d2db4-108">成员</span><span class="sxs-lookup"><span data-stu-id="d2db4-108">Member</span></span>|<span data-ttu-id="d2db4-109">值</span><span class="sxs-lookup"><span data-stu-id="d2db4-109">Value</span></span>|<span data-ttu-id="d2db4-110">说明</span><span class="sxs-lookup"><span data-stu-id="d2db4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2db4-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d2db4-111">notConfigured</span></span>|<span data-ttu-id="d2db4-112">0</span><span class="sxs-lookup"><span data-stu-id="d2db4-112">0</span></span>|<span data-ttu-id="d2db4-113">未设置任何标志。</span><span class="sxs-lookup"><span data-stu-id="d2db4-113">No flags set.</span></span>|
|<span data-ttu-id="d2db4-114">domain</span><span class="sxs-lookup"><span data-stu-id="d2db4-114">domain</span></span>|<span data-ttu-id="d2db4-115">1</span><span class="sxs-lookup"><span data-stu-id="d2db4-115">1</span></span>|<span data-ttu-id="d2db4-116">连接到域的网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="d2db4-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="d2db4-117">private</span><span class="sxs-lookup"><span data-stu-id="d2db4-117">private</span></span>|<span data-ttu-id="d2db4-118">双面</span><span class="sxs-lookup"><span data-stu-id="d2db4-118">2</span></span>|<span data-ttu-id="d2db4-119">专用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="d2db4-119">The profile for private networks.</span></span>|
|<span data-ttu-id="d2db4-120">公开</span><span class="sxs-lookup"><span data-stu-id="d2db4-120">public</span></span>|<span data-ttu-id="d2db4-121">4 </span><span class="sxs-lookup"><span data-stu-id="d2db4-121">4</span></span>|<span data-ttu-id="d2db4-122">公用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="d2db4-122">The profile for public networks.</span></span>|



