---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ea4dee71a18a6ddca4519d8b421d2097fc7907b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367643"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="4e0c7-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4e0c7-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="4e0c7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e0c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e0c7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e0c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e0c7-106">每应用 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="4e0c7-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="4e0c7-107">成员</span><span class="sxs-lookup"><span data-stu-id="4e0c7-107">Members</span></span>
|<span data-ttu-id="4e0c7-108">成员</span><span class="sxs-lookup"><span data-stu-id="4e0c7-108">Member</span></span>|<span data-ttu-id="4e0c7-109">值</span><span class="sxs-lookup"><span data-stu-id="4e0c7-109">Value</span></span>|<span data-ttu-id="4e0c7-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e0c7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e0c7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4e0c7-111">notConfigured</span></span>|<span data-ttu-id="4e0c7-112">0</span><span class="sxs-lookup"><span data-stu-id="4e0c7-112">0</span></span>|<span data-ttu-id="4e0c7-113">未显式配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="4e0c7-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="4e0c7-114">appProxy</span><span class="sxs-lookup"><span data-stu-id="4e0c7-114">appProxy</span></span>|<span data-ttu-id="4e0c7-115">1</span><span class="sxs-lookup"><span data-stu-id="4e0c7-115">1</span></span>|<span data-ttu-id="4e0c7-116">应用程序层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="4e0c7-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="4e0c7-117">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="4e0c7-117">packetTunnel</span></span>|<span data-ttu-id="4e0c7-118">双面</span><span class="sxs-lookup"><span data-stu-id="4e0c7-118">2</span></span>|<span data-ttu-id="4e0c7-119">IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="4e0c7-119">Tunnel traffic at the IP layer.</span></span>|



