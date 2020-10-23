---
title: macOSContentCachingParentSelectionPolicy 枚举类型
description: 确定内容缓存如何选择父缓存。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 726c6d4feb7387fd67583c451a9f3399a316f4a0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735818"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a><span data-ttu-id="9c4a2-103">macOSContentCachingParentSelectionPolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9c4a2-103">macOSContentCachingParentSelectionPolicy enum type</span></span>

<span data-ttu-id="9c4a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c4a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c4a2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c4a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c4a2-107">确定内容缓存如何选择父缓存。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-107">Determines how content caches select a parent cache.</span></span>

## <a name="members"></a><span data-ttu-id="9c4a2-108">成员</span><span class="sxs-lookup"><span data-stu-id="9c4a2-108">Members</span></span>
|<span data-ttu-id="9c4a2-109">成员</span><span class="sxs-lookup"><span data-stu-id="9c4a2-109">Member</span></span>|<span data-ttu-id="9c4a2-110">值</span><span class="sxs-lookup"><span data-stu-id="9c4a2-110">Value</span></span>|<span data-ttu-id="9c4a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="9c4a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c4a2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9c4a2-112">notConfigured</span></span>|<span data-ttu-id="9c4a2-113">0</span><span class="sxs-lookup"><span data-stu-id="9c4a2-113">0</span></span>|<span data-ttu-id="9c4a2-114">默认值为循环策略。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-114">Defaults to round-robin strategy.</span></span>|
|<span data-ttu-id="9c4a2-115">roundRobin</span><span class="sxs-lookup"><span data-stu-id="9c4a2-115">roundRobin</span></span>|<span data-ttu-id="9c4a2-116">1</span><span class="sxs-lookup"><span data-stu-id="9c4a2-116">1</span></span>|<span data-ttu-id="9c4a2-117">按顺序旋转父项。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-117">Rotate through the parents in order.</span></span> <span data-ttu-id="9c4a2-118">使用此策略进行负载平衡。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-118">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="9c4a2-119">firstAvailable</span><span class="sxs-lookup"><span data-stu-id="9c4a2-119">firstAvailable</span></span>|<span data-ttu-id="9c4a2-120">双面</span><span class="sxs-lookup"><span data-stu-id="9c4a2-120">2</span></span>|<span data-ttu-id="9c4a2-121">始终使用父列表中的第一个可用父项。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-121">Always use the first available parent in the Parents list.</span></span> <span data-ttu-id="9c4a2-122">使用此策略可指定永久的主要、次要和后续父项。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-122">Use this policy to designate permanent primary, secondary, and subsequent parents.</span></span>|
|<span data-ttu-id="9c4a2-123">urlPathHash</span><span class="sxs-lookup"><span data-stu-id="9c4a2-123">urlPathHash</span></span>|<span data-ttu-id="9c4a2-124">第三章</span><span class="sxs-lookup"><span data-stu-id="9c4a2-124">3</span></span>|<span data-ttu-id="9c4a2-125">对所请求 URL 的路径部分进行哈希运算，以便始终将相同的父项用于相同的 URL。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-125">Hash the path part of the requested URL so that the same parent is always used for the same URL.</span></span> <span data-ttu-id="9c4a2-126">这有助于最大限度地提高父项的合并缓存的大小。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-126">This is useful for maximizing the size of the combined caches of the parents.</span></span>|
|<span data-ttu-id="9c4a2-127">随机</span><span class="sxs-lookup"><span data-stu-id="9c4a2-127">random</span></span>|<span data-ttu-id="9c4a2-128">4 </span><span class="sxs-lookup"><span data-stu-id="9c4a2-128">4</span></span>|<span data-ttu-id="9c4a2-129">随机选择父项。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-129">Choose a parent at random.</span></span> <span data-ttu-id="9c4a2-130">使用此策略进行负载平衡。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-130">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="9c4a2-131">stickyAvailable</span><span class="sxs-lookup"><span data-stu-id="9c4a2-131">stickyAvailable</span></span>|<span data-ttu-id="9c4a2-132">5 </span><span class="sxs-lookup"><span data-stu-id="9c4a2-132">5</span></span>|<span data-ttu-id="9c4a2-133">使用父列表中的第一个可用父项，直到其不可用，然后前进到下一个。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-133">Use the first available parent that is available in the Parents list until it becomes unavailable, then advance to the next one.</span></span> <span data-ttu-id="9c4a2-134">使用此策略可指定浮动的主要、辅助和后续的父项。</span><span class="sxs-lookup"><span data-stu-id="9c4a2-134">Use this policy for designating floating primary, secondary, and subsequent parents.</span></span>|





