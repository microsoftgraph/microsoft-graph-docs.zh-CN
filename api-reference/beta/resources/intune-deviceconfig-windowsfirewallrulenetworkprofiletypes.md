---
title: windowsFirewallRuleNetworkProfileTypes 枚举类型
description: 表示哪些网络配置文件类型适用于防火墙规则的标志。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9e46fccf175483090bc78ae0c070112c7e3f18e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215329"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="9e63c-103">windowsFirewallRuleNetworkProfileTypes 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9e63c-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

<span data-ttu-id="9e63c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e63c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e63c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e63c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e63c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e63c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e63c-107">表示哪些网络配置文件类型适用于防火墙规则的标志。</span><span class="sxs-lookup"><span data-stu-id="9e63c-107">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="9e63c-108">成员</span><span class="sxs-lookup"><span data-stu-id="9e63c-108">Members</span></span>
|<span data-ttu-id="9e63c-109">成员</span><span class="sxs-lookup"><span data-stu-id="9e63c-109">Member</span></span>|<span data-ttu-id="9e63c-110">值</span><span class="sxs-lookup"><span data-stu-id="9e63c-110">Value</span></span>|<span data-ttu-id="9e63c-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e63c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e63c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9e63c-112">notConfigured</span></span>|<span data-ttu-id="9e63c-113">0</span><span class="sxs-lookup"><span data-stu-id="9e63c-113">0</span></span>|<span data-ttu-id="9e63c-114">未设置任何标志。</span><span class="sxs-lookup"><span data-stu-id="9e63c-114">No flags set.</span></span>|
|<span data-ttu-id="9e63c-115">domain</span><span class="sxs-lookup"><span data-stu-id="9e63c-115">domain</span></span>|<span data-ttu-id="9e63c-116">1</span><span class="sxs-lookup"><span data-stu-id="9e63c-116">1</span></span>|<span data-ttu-id="9e63c-117">连接到域的网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="9e63c-117">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="9e63c-118">private</span><span class="sxs-lookup"><span data-stu-id="9e63c-118">private</span></span>|<span data-ttu-id="9e63c-119">双面</span><span class="sxs-lookup"><span data-stu-id="9e63c-119">2</span></span>|<span data-ttu-id="9e63c-120">专用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="9e63c-120">The profile for private networks.</span></span>|
|<span data-ttu-id="9e63c-121">公开</span><span class="sxs-lookup"><span data-stu-id="9e63c-121">public</span></span>|<span data-ttu-id="9e63c-122">4 </span><span class="sxs-lookup"><span data-stu-id="9e63c-122">4</span></span>|<span data-ttu-id="9e63c-123">公用网络的配置文件。</span><span class="sxs-lookup"><span data-stu-id="9e63c-123">The profile for public networks.</span></span>|




