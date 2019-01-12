---
title: vpnProviderType 枚举类型
description: 每个应用程序 VPN 的提供程序类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1eeb0acf2f6e7b0773cbf4697e5a27699d1f2f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937724"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="5b390-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5b390-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="5b390-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b390-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b390-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b390-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b390-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5b390-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b390-107">每个应用程序 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="5b390-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="5b390-108">成员</span><span class="sxs-lookup"><span data-stu-id="5b390-108">Members</span></span>
|<span data-ttu-id="5b390-109">成员</span><span class="sxs-lookup"><span data-stu-id="5b390-109">Member</span></span>|<span data-ttu-id="5b390-110">值</span><span class="sxs-lookup"><span data-stu-id="5b390-110">Value</span></span>|<span data-ttu-id="5b390-111">Description</span><span class="sxs-lookup"><span data-stu-id="5b390-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b390-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5b390-112">notConfigured</span></span>|<span data-ttu-id="5b390-113">0</span><span class="sxs-lookup"><span data-stu-id="5b390-113">0</span></span>|<span data-ttu-id="5b390-114">不明确地配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="5b390-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="5b390-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="5b390-115">appProxy</span></span>|<span data-ttu-id="5b390-116">1</span><span class="sxs-lookup"><span data-stu-id="5b390-116">1</span></span>|<span data-ttu-id="5b390-117">在应用层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="5b390-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="5b390-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="5b390-118">packetTunnel</span></span>|<span data-ttu-id="5b390-119">2</span><span class="sxs-lookup"><span data-stu-id="5b390-119">2</span></span>|<span data-ttu-id="5b390-120">在 IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="5b390-120">Tunnel traffic at the IP layer.</span></span>|





