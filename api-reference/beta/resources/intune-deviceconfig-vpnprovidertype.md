---
title: vpnProviderType 枚举类型
description: 每个应用程序 VPN 的提供程序类型。
author: tfitzmac
ms.openlocfilehash: d8f002582879302bcbe0fb965110eaa5e674a689
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351595"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="de8ea-103">vpnProviderType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="de8ea-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="de8ea-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de8ea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de8ea-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de8ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de8ea-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="de8ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de8ea-107">每个应用程序 VPN 的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="de8ea-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="de8ea-108">成员</span><span class="sxs-lookup"><span data-stu-id="de8ea-108">Members</span></span>
|<span data-ttu-id="de8ea-109">成员</span><span class="sxs-lookup"><span data-stu-id="de8ea-109">Member</span></span>|<span data-ttu-id="de8ea-110">值</span><span class="sxs-lookup"><span data-stu-id="de8ea-110">Value</span></span>|<span data-ttu-id="de8ea-111">说明</span><span class="sxs-lookup"><span data-stu-id="de8ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de8ea-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="de8ea-112">notConfigured</span></span>|<span data-ttu-id="de8ea-113">0</span><span class="sxs-lookup"><span data-stu-id="de8ea-113">0</span></span>|<span data-ttu-id="de8ea-114">不明确地配置隧道通信。</span><span class="sxs-lookup"><span data-stu-id="de8ea-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="de8ea-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="de8ea-115">appProxy</span></span>|<span data-ttu-id="de8ea-116">1</span><span class="sxs-lookup"><span data-stu-id="de8ea-116">1</span></span>|<span data-ttu-id="de8ea-117">在应用层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="de8ea-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="de8ea-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="de8ea-118">packetTunnel</span></span>|<span data-ttu-id="de8ea-119">2</span><span class="sxs-lookup"><span data-stu-id="de8ea-119">2</span></span>|<span data-ttu-id="de8ea-120">在 IP 层的隧道流量。</span><span class="sxs-lookup"><span data-stu-id="de8ea-120">Tunnel traffic at the IP layer.</span></span>|





