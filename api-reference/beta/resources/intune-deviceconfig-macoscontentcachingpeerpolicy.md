---
title: macOSContentCachingPeerPolicy 枚举类型
description: 确定哪些内容缓存其他内容缓存将对等。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4a42b90bde7feba7c3d1904529d0c0f31ad0a412
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790185"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a><span data-ttu-id="59895-103">macOSContentCachingPeerPolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="59895-103">macOSContentCachingPeerPolicy enum type</span></span>

<span data-ttu-id="59895-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59895-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59895-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="59895-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59895-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59895-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59895-107">确定哪些内容缓存其他内容缓存将对等。</span><span class="sxs-lookup"><span data-stu-id="59895-107">Determines which content caches other content caches will peer with.</span></span>

## <a name="members"></a><span data-ttu-id="59895-108">成员</span><span class="sxs-lookup"><span data-stu-id="59895-108">Members</span></span>
|<span data-ttu-id="59895-109">成员</span><span class="sxs-lookup"><span data-stu-id="59895-109">Member</span></span>|<span data-ttu-id="59895-110">值</span><span class="sxs-lookup"><span data-stu-id="59895-110">Value</span></span>|<span data-ttu-id="59895-111">说明</span><span class="sxs-lookup"><span data-stu-id="59895-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59895-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="59895-112">notConfigured</span></span>|<span data-ttu-id="59895-113">0</span><span class="sxs-lookup"><span data-stu-id="59895-113">0</span></span>|<span data-ttu-id="59895-114">默认值为本地网络中的对等方。</span><span class="sxs-lookup"><span data-stu-id="59895-114">Defaults to peers in local network.</span></span>|
|<span data-ttu-id="59895-115">peersInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="59895-115">peersInLocalNetwork</span></span>|<span data-ttu-id="59895-116">1 </span><span class="sxs-lookup"><span data-stu-id="59895-116">1</span></span>|<span data-ttu-id="59895-117">内容缓存将仅对其直接本地网络中的缓存具有同等的对等缓存。</span><span class="sxs-lookup"><span data-stu-id="59895-117">Content caches will only peer with caches in their immediate local network.</span></span>|
|<span data-ttu-id="59895-118">peersWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="59895-118">peersWithSamePublicIpAddress</span></span>|<span data-ttu-id="59895-119">双面</span><span class="sxs-lookup"><span data-stu-id="59895-119">2</span></span>|<span data-ttu-id="59895-120">内容缓存将仅对共享相同公用 IP 地址的缓存具有同等的对等缓存。</span><span class="sxs-lookup"><span data-stu-id="59895-120">Content caches will only peer with caches that share the same public IP address.</span></span>|
|<span data-ttu-id="59895-121">peersInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="59895-121">peersInCustomLocalNetworks</span></span>|<span data-ttu-id="59895-122">第三章</span><span class="sxs-lookup"><span data-stu-id="59895-122">3</span></span>|<span data-ttu-id="59895-123">内容缓存将使用 contentCachingPeerFilterRanges 和 contentCachingPeerListenRanges 来确定与对等方的缓存。</span><span class="sxs-lookup"><span data-stu-id="59895-123">Content caches will use contentCachingPeerFilterRanges and contentCachingPeerListenRanges to determine which caches to peer with.</span></span>|



