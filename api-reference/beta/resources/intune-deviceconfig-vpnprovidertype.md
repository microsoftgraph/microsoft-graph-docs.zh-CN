---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a62436f56a210bbb71606ebb8f2586e5b48f8d1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163187"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="0a26e-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0a26e-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="0a26e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0a26e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a26e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a26e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a26e-106">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="0a26e-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="0a26e-107">成员</span><span class="sxs-lookup"><span data-stu-id="0a26e-107">Members</span></span>
|<span data-ttu-id="0a26e-108">成员</span><span class="sxs-lookup"><span data-stu-id="0a26e-108">Member</span></span>|<span data-ttu-id="0a26e-109">值</span><span class="sxs-lookup"><span data-stu-id="0a26e-109">Value</span></span>|<span data-ttu-id="0a26e-110">说明</span><span class="sxs-lookup"><span data-stu-id="0a26e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a26e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0a26e-111">notConfigured</span></span>|<span data-ttu-id="0a26e-112">0</span><span class="sxs-lookup"><span data-stu-id="0a26e-112">0</span></span>|<span data-ttu-id="0a26e-113">未显式配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="0a26e-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="0a26e-114">appProxy</span><span class="sxs-lookup"><span data-stu-id="0a26e-114">appProxy</span></span>|<span data-ttu-id="0a26e-115">1</span><span class="sxs-lookup"><span data-stu-id="0a26e-115">1</span></span>|<span data-ttu-id="0a26e-116">应用程序层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="0a26e-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="0a26e-117">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="0a26e-117">packetTunnel</span></span>|<span data-ttu-id="0a26e-118">双面</span><span class="sxs-lookup"><span data-stu-id="0a26e-118">2</span></span>|<span data-ttu-id="0a26e-119">IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="0a26e-119">Tunnel traffic at the IP layer.</span></span>|




