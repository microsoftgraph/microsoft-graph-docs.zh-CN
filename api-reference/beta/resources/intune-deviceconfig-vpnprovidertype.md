---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 43e9c146fc30e9dfaadef45b42e45dcf0787f13f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969462"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="145b7-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="145b7-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="145b7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="145b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="145b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="145b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="145b7-106">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="145b7-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="145b7-107">成员</span><span class="sxs-lookup"><span data-stu-id="145b7-107">Members</span></span>
|<span data-ttu-id="145b7-108">成员</span><span class="sxs-lookup"><span data-stu-id="145b7-108">Member</span></span>|<span data-ttu-id="145b7-109">值</span><span class="sxs-lookup"><span data-stu-id="145b7-109">Value</span></span>|<span data-ttu-id="145b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="145b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="145b7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="145b7-111">notConfigured</span></span>|<span data-ttu-id="145b7-112">0</span><span class="sxs-lookup"><span data-stu-id="145b7-112">0</span></span>|<span data-ttu-id="145b7-113">未显式配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="145b7-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="145b7-114">appProxy</span><span class="sxs-lookup"><span data-stu-id="145b7-114">appProxy</span></span>|<span data-ttu-id="145b7-115">1</span><span class="sxs-lookup"><span data-stu-id="145b7-115">1</span></span>|<span data-ttu-id="145b7-116">应用程序层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="145b7-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="145b7-117">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="145b7-117">packetTunnel</span></span>|<span data-ttu-id="145b7-118">双面</span><span class="sxs-lookup"><span data-stu-id="145b7-118">2</span></span>|<span data-ttu-id="145b7-119">IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="145b7-119">Tunnel traffic at the IP layer.</span></span>|





