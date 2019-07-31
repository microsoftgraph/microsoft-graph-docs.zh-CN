---
title: windowsFirewallRuleNetworkProfileTypes 枚举类型
description: 表示哪些网络配置文件类型适用于防火墙规则的标志。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d89ddee30e04ac8d22cf0f754139101b858c259b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969049"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="2cac3-103">windowsFirewallRuleNetworkProfileTypes 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2cac3-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="2cac3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2cac3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cac3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2cac3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cac3-106">表示哪些网络配置文件类型适用于防火墙规则的标志。</span><span class="sxs-lookup"><span data-stu-id="2cac3-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="2cac3-107">成员</span><span class="sxs-lookup"><span data-stu-id="2cac3-107">Members</span></span>
|<span data-ttu-id="2cac3-108">成员</span><span class="sxs-lookup"><span data-stu-id="2cac3-108">Member</span></span>|<span data-ttu-id="2cac3-109">值</span><span class="sxs-lookup"><span data-stu-id="2cac3-109">Value</span></span>|<span data-ttu-id="2cac3-110">说明</span><span class="sxs-lookup"><span data-stu-id="2cac3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cac3-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2cac3-111">notConfigured</span></span>|<span data-ttu-id="2cac3-112">0</span><span class="sxs-lookup"><span data-stu-id="2cac3-112">0</span></span>|<span data-ttu-id="2cac3-113">未设置任何标志。</span><span class="sxs-lookup"><span data-stu-id="2cac3-113">No flags set.</span></span>|
|<span data-ttu-id="2cac3-114">domain</span><span class="sxs-lookup"><span data-stu-id="2cac3-114">domain</span></span>|<span data-ttu-id="2cac3-115">1</span><span class="sxs-lookup"><span data-stu-id="2cac3-115">1</span></span>|<span data-ttu-id="2cac3-116">连接到域的网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="2cac3-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="2cac3-117">private</span><span class="sxs-lookup"><span data-stu-id="2cac3-117">private</span></span>|<span data-ttu-id="2cac3-118">双面</span><span class="sxs-lookup"><span data-stu-id="2cac3-118">2</span></span>|<span data-ttu-id="2cac3-119">专用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="2cac3-119">The profile for private networks.</span></span>|
|<span data-ttu-id="2cac3-120">公开</span><span class="sxs-lookup"><span data-stu-id="2cac3-120">public</span></span>|<span data-ttu-id="2cac3-121">4</span><span class="sxs-lookup"><span data-stu-id="2cac3-121">4</span></span>|<span data-ttu-id="2cac3-122">公用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="2cac3-122">The profile for public networks.</span></span>|





