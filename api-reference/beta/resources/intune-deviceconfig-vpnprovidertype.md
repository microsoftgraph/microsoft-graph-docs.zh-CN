---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 43b962235cda6622ca0d7d10d7da57f9f5181471
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048993"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="2986b-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2986b-103">vpnProviderType enum type</span></span>

<span data-ttu-id="2986b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2986b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2986b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2986b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2986b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2986b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2986b-107">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="2986b-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="2986b-108">成员</span><span class="sxs-lookup"><span data-stu-id="2986b-108">Members</span></span>
|<span data-ttu-id="2986b-109">成员</span><span class="sxs-lookup"><span data-stu-id="2986b-109">Member</span></span>|<span data-ttu-id="2986b-110">值</span><span class="sxs-lookup"><span data-stu-id="2986b-110">Value</span></span>|<span data-ttu-id="2986b-111">说明</span><span class="sxs-lookup"><span data-stu-id="2986b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2986b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2986b-112">notConfigured</span></span>|<span data-ttu-id="2986b-113">0</span><span class="sxs-lookup"><span data-stu-id="2986b-113">0</span></span>|<span data-ttu-id="2986b-114">未显式配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="2986b-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="2986b-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="2986b-115">appProxy</span></span>|<span data-ttu-id="2986b-116">1 </span><span class="sxs-lookup"><span data-stu-id="2986b-116">1</span></span>|<span data-ttu-id="2986b-117">应用程序层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="2986b-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="2986b-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="2986b-118">packetTunnel</span></span>|<span data-ttu-id="2986b-119">2 </span><span class="sxs-lookup"><span data-stu-id="2986b-119">2</span></span>|<span data-ttu-id="2986b-120">IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="2986b-120">Tunnel traffic at the IP layer.</span></span>|






