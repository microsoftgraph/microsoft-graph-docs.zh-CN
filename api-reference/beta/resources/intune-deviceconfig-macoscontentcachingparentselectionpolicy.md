---
title: macOSContentCachingParentSelectionPolicy 枚举类型
description: 确定内容缓存如何选择父缓存。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 221d33640a3e100adbad4fe013e10b6c5ab90b4e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790199"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a><span data-ttu-id="c8e0f-103">macOSContentCachingParentSelectionPolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c8e0f-103">macOSContentCachingParentSelectionPolicy enum type</span></span>

<span data-ttu-id="c8e0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8e0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8e0f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8e0f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8e0f-107">确定内容缓存如何选择父缓存。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-107">Determines how content caches select a parent cache.</span></span>

## <a name="members"></a><span data-ttu-id="c8e0f-108">成员</span><span class="sxs-lookup"><span data-stu-id="c8e0f-108">Members</span></span>
|<span data-ttu-id="c8e0f-109">成员</span><span class="sxs-lookup"><span data-stu-id="c8e0f-109">Member</span></span>|<span data-ttu-id="c8e0f-110">值</span><span class="sxs-lookup"><span data-stu-id="c8e0f-110">Value</span></span>|<span data-ttu-id="c8e0f-111">说明</span><span class="sxs-lookup"><span data-stu-id="c8e0f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8e0f-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c8e0f-112">notConfigured</span></span>|<span data-ttu-id="c8e0f-113">0</span><span class="sxs-lookup"><span data-stu-id="c8e0f-113">0</span></span>|<span data-ttu-id="c8e0f-114">默认值为循环策略。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-114">Defaults to round-robin strategy.</span></span>|
|<span data-ttu-id="c8e0f-115">roundRobin</span><span class="sxs-lookup"><span data-stu-id="c8e0f-115">roundRobin</span></span>|<span data-ttu-id="c8e0f-116">1 </span><span class="sxs-lookup"><span data-stu-id="c8e0f-116">1</span></span>|<span data-ttu-id="c8e0f-117">按顺序旋转父项。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-117">Rotate through the parents in order.</span></span> <span data-ttu-id="c8e0f-118">使用此策略进行负载平衡。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-118">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="c8e0f-119">firstAvailable</span><span class="sxs-lookup"><span data-stu-id="c8e0f-119">firstAvailable</span></span>|<span data-ttu-id="c8e0f-120">双面</span><span class="sxs-lookup"><span data-stu-id="c8e0f-120">2</span></span>|<span data-ttu-id="c8e0f-121">始终使用父列表中的第一个可用父项。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-121">Always use the first available parent in the Parents list.</span></span> <span data-ttu-id="c8e0f-122">使用此策略可指定永久的主要、次要和后续父项。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-122">Use this policy to designate permanent primary, secondary, and subsequent parents.</span></span>|
|<span data-ttu-id="c8e0f-123">urlPathHash</span><span class="sxs-lookup"><span data-stu-id="c8e0f-123">urlPathHash</span></span>|<span data-ttu-id="c8e0f-124">第三章</span><span class="sxs-lookup"><span data-stu-id="c8e0f-124">3</span></span>|<span data-ttu-id="c8e0f-125">对所请求 URL 的路径部分进行哈希运算，以便始终将相同的父项用于相同的 URL。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-125">Hash the path part of the requested URL so that the same parent is always used for the same URL.</span></span> <span data-ttu-id="c8e0f-126">这有助于最大限度地提高父项的合并缓存的大小。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-126">This is useful for maximizing the size of the combined caches of the parents.</span></span>|
|<span data-ttu-id="c8e0f-127">随机</span><span class="sxs-lookup"><span data-stu-id="c8e0f-127">random</span></span>|<span data-ttu-id="c8e0f-128">4 </span><span class="sxs-lookup"><span data-stu-id="c8e0f-128">4</span></span>|<span data-ttu-id="c8e0f-129">随机选择父项。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-129">Choose a parent at random.</span></span> <span data-ttu-id="c8e0f-130">使用此策略进行负载平衡。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-130">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="c8e0f-131">stickyAvailable</span><span class="sxs-lookup"><span data-stu-id="c8e0f-131">stickyAvailable</span></span>|<span data-ttu-id="c8e0f-132">5 </span><span class="sxs-lookup"><span data-stu-id="c8e0f-132">5</span></span>|<span data-ttu-id="c8e0f-133">使用父列表中的第一个可用父项，直到其不可用，然后前进到下一个。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-133">Use the first available parent that is available in the Parents list until it becomes unavailable, then advance to the next one.</span></span> <span data-ttu-id="c8e0f-134">使用此策略可指定浮动的主要、辅助和后续的父项。</span><span class="sxs-lookup"><span data-stu-id="c8e0f-134">Use this policy for designating floating primary, secondary, and subsequent parents.</span></span>|



