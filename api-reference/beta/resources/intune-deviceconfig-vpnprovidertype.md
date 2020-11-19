---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb29fc6a77eb6db051279cdeb630dbf4104aa9af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279575"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="3e73e-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3e73e-103">vpnProviderType enum type</span></span>

<span data-ttu-id="3e73e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e73e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e73e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e73e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e73e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e73e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e73e-107">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="3e73e-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="3e73e-108">成员</span><span class="sxs-lookup"><span data-stu-id="3e73e-108">Members</span></span>
|<span data-ttu-id="3e73e-109">成员</span><span class="sxs-lookup"><span data-stu-id="3e73e-109">Member</span></span>|<span data-ttu-id="3e73e-110">值</span><span class="sxs-lookup"><span data-stu-id="3e73e-110">Value</span></span>|<span data-ttu-id="3e73e-111">说明</span><span class="sxs-lookup"><span data-stu-id="3e73e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e73e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3e73e-112">notConfigured</span></span>|<span data-ttu-id="3e73e-113">0</span><span class="sxs-lookup"><span data-stu-id="3e73e-113">0</span></span>|<span data-ttu-id="3e73e-114">未显式配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="3e73e-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="3e73e-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="3e73e-115">appProxy</span></span>|<span data-ttu-id="3e73e-116">1</span><span class="sxs-lookup"><span data-stu-id="3e73e-116">1</span></span>|<span data-ttu-id="3e73e-117">应用程序层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="3e73e-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="3e73e-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="3e73e-118">packetTunnel</span></span>|<span data-ttu-id="3e73e-119">双面</span><span class="sxs-lookup"><span data-stu-id="3e73e-119">2</span></span>|<span data-ttu-id="3e73e-120">IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="3e73e-120">Tunnel traffic at the IP layer.</span></span>|




