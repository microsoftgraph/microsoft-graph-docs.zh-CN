---
title: macOSContentCachingPeerPolicy 枚举类型
description: 确定哪些内容缓存其他内容缓存将对等。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7305c42098782d9e69e734037fb08d3238c7b4a9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268746"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a><span data-ttu-id="92345-103">macOSContentCachingPeerPolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="92345-103">macOSContentCachingPeerPolicy enum type</span></span>

<span data-ttu-id="92345-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92345-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92345-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92345-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92345-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92345-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92345-107">确定哪些内容缓存其他内容缓存将对等。</span><span class="sxs-lookup"><span data-stu-id="92345-107">Determines which content caches other content caches will peer with.</span></span>

## <a name="members"></a><span data-ttu-id="92345-108">成员</span><span class="sxs-lookup"><span data-stu-id="92345-108">Members</span></span>
|<span data-ttu-id="92345-109">成员</span><span class="sxs-lookup"><span data-stu-id="92345-109">Member</span></span>|<span data-ttu-id="92345-110">值</span><span class="sxs-lookup"><span data-stu-id="92345-110">Value</span></span>|<span data-ttu-id="92345-111">说明</span><span class="sxs-lookup"><span data-stu-id="92345-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92345-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="92345-112">notConfigured</span></span>|<span data-ttu-id="92345-113">0</span><span class="sxs-lookup"><span data-stu-id="92345-113">0</span></span>|<span data-ttu-id="92345-114">默认值为本地网络中的对等方。</span><span class="sxs-lookup"><span data-stu-id="92345-114">Defaults to peers in local network.</span></span>|
|<span data-ttu-id="92345-115">peersInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="92345-115">peersInLocalNetwork</span></span>|<span data-ttu-id="92345-116">1</span><span class="sxs-lookup"><span data-stu-id="92345-116">1</span></span>|<span data-ttu-id="92345-117">内容缓存将仅对其直接本地网络中的缓存具有同等的对等缓存。</span><span class="sxs-lookup"><span data-stu-id="92345-117">Content caches will only peer with caches in their immediate local network.</span></span>|
|<span data-ttu-id="92345-118">peersWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="92345-118">peersWithSamePublicIpAddress</span></span>|<span data-ttu-id="92345-119">双面</span><span class="sxs-lookup"><span data-stu-id="92345-119">2</span></span>|<span data-ttu-id="92345-120">内容缓存将仅对共享相同公用 IP 地址的缓存具有同等的对等缓存。</span><span class="sxs-lookup"><span data-stu-id="92345-120">Content caches will only peer with caches that share the same public IP address.</span></span>|
|<span data-ttu-id="92345-121">peersInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="92345-121">peersInCustomLocalNetworks</span></span>|<span data-ttu-id="92345-122">第三章</span><span class="sxs-lookup"><span data-stu-id="92345-122">3</span></span>|<span data-ttu-id="92345-123">内容缓存将使用 contentCachingPeerFilterRanges 和 contentCachingPeerListenRanges 来确定与对等方的缓存。</span><span class="sxs-lookup"><span data-stu-id="92345-123">Content caches will use contentCachingPeerFilterRanges and contentCachingPeerListenRanges to determine which caches to peer with.</span></span>|




