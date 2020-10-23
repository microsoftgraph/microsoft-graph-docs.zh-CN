---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f20433a7e2bbb0dd134471476fd96fe3e49b9ecd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728326"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="df871-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="df871-103">vpnProviderType enum type</span></span>

<span data-ttu-id="df871-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df871-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df871-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df871-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df871-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df871-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df871-107">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="df871-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="df871-108">成员</span><span class="sxs-lookup"><span data-stu-id="df871-108">Members</span></span>
|<span data-ttu-id="df871-109">成员</span><span class="sxs-lookup"><span data-stu-id="df871-109">Member</span></span>|<span data-ttu-id="df871-110">值</span><span class="sxs-lookup"><span data-stu-id="df871-110">Value</span></span>|<span data-ttu-id="df871-111">说明</span><span class="sxs-lookup"><span data-stu-id="df871-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df871-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="df871-112">notConfigured</span></span>|<span data-ttu-id="df871-113">0</span><span class="sxs-lookup"><span data-stu-id="df871-113">0</span></span>|<span data-ttu-id="df871-114">未显式配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="df871-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="df871-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="df871-115">appProxy</span></span>|<span data-ttu-id="df871-116">1</span><span class="sxs-lookup"><span data-stu-id="df871-116">1</span></span>|<span data-ttu-id="df871-117">应用程序层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="df871-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="df871-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="df871-118">packetTunnel</span></span>|<span data-ttu-id="df871-119">双面</span><span class="sxs-lookup"><span data-stu-id="df871-119">2</span></span>|<span data-ttu-id="df871-120">IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="df871-120">Tunnel traffic at the IP layer.</span></span>|





