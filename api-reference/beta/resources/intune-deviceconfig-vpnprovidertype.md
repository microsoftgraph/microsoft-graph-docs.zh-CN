---
title: vpnProviderType 枚举类型
description: 每个应用程序 VPN 的提供程序类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2de8f78222ba0c945000b84f28039c2f6af58daa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407219"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="5f610-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5f610-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="5f610-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5f610-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f610-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5f610-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f610-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f610-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f610-107">每个应用程序 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="5f610-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="5f610-108">成员</span><span class="sxs-lookup"><span data-stu-id="5f610-108">Members</span></span>
|<span data-ttu-id="5f610-109">成员</span><span class="sxs-lookup"><span data-stu-id="5f610-109">Member</span></span>|<span data-ttu-id="5f610-110">值</span><span class="sxs-lookup"><span data-stu-id="5f610-110">Value</span></span>|<span data-ttu-id="5f610-111">说明</span><span class="sxs-lookup"><span data-stu-id="5f610-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f610-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5f610-112">notConfigured</span></span>|<span data-ttu-id="5f610-113">0</span><span class="sxs-lookup"><span data-stu-id="5f610-113">0</span></span>|<span data-ttu-id="5f610-114">不明确地配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="5f610-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="5f610-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="5f610-115">appProxy</span></span>|<span data-ttu-id="5f610-116">1</span><span class="sxs-lookup"><span data-stu-id="5f610-116">1</span></span>|<span data-ttu-id="5f610-117">在应用层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="5f610-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="5f610-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="5f610-118">packetTunnel</span></span>|<span data-ttu-id="5f610-119">2</span><span class="sxs-lookup"><span data-stu-id="5f610-119">2</span></span>|<span data-ttu-id="5f610-120">在 IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="5f610-120">Tunnel traffic at the IP layer.</span></span>|




