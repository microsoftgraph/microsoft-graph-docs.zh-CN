---
title: macOSContentCachingPeerPolicy 枚举类型
description: 确定哪些内容缓存其他内容缓存将对等。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1f55bd6aafffc7602632155e4fa3c387c888aae9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735811"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a><span data-ttu-id="24566-103">macOSContentCachingPeerPolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="24566-103">macOSContentCachingPeerPolicy enum type</span></span>

<span data-ttu-id="24566-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24566-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24566-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24566-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24566-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24566-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24566-107">确定哪些内容缓存其他内容缓存将对等。</span><span class="sxs-lookup"><span data-stu-id="24566-107">Determines which content caches other content caches will peer with.</span></span>

## <a name="members"></a><span data-ttu-id="24566-108">成员</span><span class="sxs-lookup"><span data-stu-id="24566-108">Members</span></span>
|<span data-ttu-id="24566-109">成员</span><span class="sxs-lookup"><span data-stu-id="24566-109">Member</span></span>|<span data-ttu-id="24566-110">值</span><span class="sxs-lookup"><span data-stu-id="24566-110">Value</span></span>|<span data-ttu-id="24566-111">说明</span><span class="sxs-lookup"><span data-stu-id="24566-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24566-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="24566-112">notConfigured</span></span>|<span data-ttu-id="24566-113">0</span><span class="sxs-lookup"><span data-stu-id="24566-113">0</span></span>|<span data-ttu-id="24566-114">默认值为本地网络中的对等方。</span><span class="sxs-lookup"><span data-stu-id="24566-114">Defaults to peers in local network.</span></span>|
|<span data-ttu-id="24566-115">peersInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="24566-115">peersInLocalNetwork</span></span>|<span data-ttu-id="24566-116">1</span><span class="sxs-lookup"><span data-stu-id="24566-116">1</span></span>|<span data-ttu-id="24566-117">内容缓存将仅对其直接本地网络中的缓存具有同等的对等缓存。</span><span class="sxs-lookup"><span data-stu-id="24566-117">Content caches will only peer with caches in their immediate local network.</span></span>|
|<span data-ttu-id="24566-118">peersWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="24566-118">peersWithSamePublicIpAddress</span></span>|<span data-ttu-id="24566-119">双面</span><span class="sxs-lookup"><span data-stu-id="24566-119">2</span></span>|<span data-ttu-id="24566-120">内容缓存将仅对共享相同公用 IP 地址的缓存具有同等的对等缓存。</span><span class="sxs-lookup"><span data-stu-id="24566-120">Content caches will only peer with caches that share the same public IP address.</span></span>|
|<span data-ttu-id="24566-121">peersInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="24566-121">peersInCustomLocalNetworks</span></span>|<span data-ttu-id="24566-122">第三章</span><span class="sxs-lookup"><span data-stu-id="24566-122">3</span></span>|<span data-ttu-id="24566-123">内容缓存将使用 contentCachingPeerFilterRanges 和 contentCachingPeerListenRanges 来确定与对等方的缓存。</span><span class="sxs-lookup"><span data-stu-id="24566-123">Content caches will use contentCachingPeerFilterRanges and contentCachingPeerListenRanges to determine which caches to peer with.</span></span>|





