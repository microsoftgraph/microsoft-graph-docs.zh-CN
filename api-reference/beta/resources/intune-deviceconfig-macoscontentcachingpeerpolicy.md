---
title: macOSContentCachingPeerPolicy 枚举类型
description: 确定哪些内容缓存其他内容缓存将对等。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e45f6d0e92624693139cd09ca4eff52cd483b46c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993824"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a><span data-ttu-id="d045a-103">macOSContentCachingPeerPolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d045a-103">macOSContentCachingPeerPolicy enum type</span></span>

<span data-ttu-id="d045a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d045a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d045a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d045a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d045a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d045a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d045a-107">确定哪些内容缓存其他内容缓存将对等。</span><span class="sxs-lookup"><span data-stu-id="d045a-107">Determines which content caches other content caches will peer with.</span></span>

## <a name="members"></a><span data-ttu-id="d045a-108">成员</span><span class="sxs-lookup"><span data-stu-id="d045a-108">Members</span></span>
|<span data-ttu-id="d045a-109">成员</span><span class="sxs-lookup"><span data-stu-id="d045a-109">Member</span></span>|<span data-ttu-id="d045a-110">值</span><span class="sxs-lookup"><span data-stu-id="d045a-110">Value</span></span>|<span data-ttu-id="d045a-111">说明</span><span class="sxs-lookup"><span data-stu-id="d045a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d045a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d045a-112">notConfigured</span></span>|<span data-ttu-id="d045a-113">0</span><span class="sxs-lookup"><span data-stu-id="d045a-113">0</span></span>|<span data-ttu-id="d045a-114">默认值为本地网络中的对等方。</span><span class="sxs-lookup"><span data-stu-id="d045a-114">Defaults to peers in local network.</span></span>|
|<span data-ttu-id="d045a-115">peersInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="d045a-115">peersInLocalNetwork</span></span>|<span data-ttu-id="d045a-116">1 </span><span class="sxs-lookup"><span data-stu-id="d045a-116">1</span></span>|<span data-ttu-id="d045a-117">内容缓存将仅对其直接本地网络中的缓存具有同等的对等缓存。</span><span class="sxs-lookup"><span data-stu-id="d045a-117">Content caches will only peer with caches in their immediate local network.</span></span>|
|<span data-ttu-id="d045a-118">peersWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="d045a-118">peersWithSamePublicIpAddress</span></span>|<span data-ttu-id="d045a-119">2 </span><span class="sxs-lookup"><span data-stu-id="d045a-119">2</span></span>|<span data-ttu-id="d045a-120">内容缓存将仅对共享相同公用 IP 地址的缓存具有同等的对等缓存。</span><span class="sxs-lookup"><span data-stu-id="d045a-120">Content caches will only peer with caches that share the same public IP address.</span></span>|
|<span data-ttu-id="d045a-121">peersInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="d045a-121">peersInCustomLocalNetworks</span></span>|<span data-ttu-id="d045a-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d045a-122">3</span></span>|<span data-ttu-id="d045a-123">内容缓存将使用 contentCachingPeerFilterRanges 和 contentCachingPeerListenRanges 来确定与对等方的缓存。</span><span class="sxs-lookup"><span data-stu-id="d045a-123">Content caches will use contentCachingPeerFilterRanges and contentCachingPeerListenRanges to determine which caches to peer with.</span></span>|






