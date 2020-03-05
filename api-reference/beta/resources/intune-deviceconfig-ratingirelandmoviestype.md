---
title: ratingIrelandMoviesType 枚举类型
description: 爱尔兰的电影评分标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: effa5631a001acacccc07587dd93302a0142d2fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529495"
---
# <a name="ratingirelandmoviestype-enum-type"></a><span data-ttu-id="8496f-103">ratingIrelandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8496f-103">ratingIrelandMoviesType enum type</span></span>

<span data-ttu-id="8496f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8496f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8496f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8496f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8496f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8496f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8496f-107">爱尔兰的电影评分标签</span><span class="sxs-lookup"><span data-stu-id="8496f-107">Movies rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="8496f-108">成员</span><span class="sxs-lookup"><span data-stu-id="8496f-108">Members</span></span>
|<span data-ttu-id="8496f-109">成员</span><span class="sxs-lookup"><span data-stu-id="8496f-109">Member</span></span>|<span data-ttu-id="8496f-110">值</span><span class="sxs-lookup"><span data-stu-id="8496f-110">Value</span></span>|<span data-ttu-id="8496f-111">说明</span><span class="sxs-lookup"><span data-stu-id="8496f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8496f-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="8496f-112">allAllowed</span></span>|<span data-ttu-id="8496f-113">0</span><span class="sxs-lookup"><span data-stu-id="8496f-113">0</span></span>|<span data-ttu-id="8496f-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="8496f-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="8496f-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="8496f-115">allBlocked</span></span>|<span data-ttu-id="8496f-116">1 </span><span class="sxs-lookup"><span data-stu-id="8496f-116">1</span></span>|<span data-ttu-id="8496f-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="8496f-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="8496f-118">概要</span><span class="sxs-lookup"><span data-stu-id="8496f-118">general</span></span>|<span data-ttu-id="8496f-119">2 </span><span class="sxs-lookup"><span data-stu-id="8496f-119">2</span></span>|<span data-ttu-id="8496f-120">适用于学校使用期限的儿童</span><span class="sxs-lookup"><span data-stu-id="8496f-120">Suitable for children of school going age</span></span>|
|<span data-ttu-id="8496f-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="8496f-121">parentalGuidance</span></span>|<span data-ttu-id="8496f-122">3 </span><span class="sxs-lookup"><span data-stu-id="8496f-122">3</span></span>|<span data-ttu-id="8496f-123">PG 分类建议家长指导</span><span class="sxs-lookup"><span data-stu-id="8496f-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="8496f-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="8496f-124">agesAbove12</span></span>|<span data-ttu-id="8496f-125">4 </span><span class="sxs-lookup"><span data-stu-id="8496f-125">4</span></span>|<span data-ttu-id="8496f-126">12A 分类适用于12岁或更早的查看者</span><span class="sxs-lookup"><span data-stu-id="8496f-126">The 12A classification is suitable for viewers of 12 or older</span></span>|
|<span data-ttu-id="8496f-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="8496f-127">agesAbove15</span></span>|<span data-ttu-id="8496f-128">5 </span><span class="sxs-lookup"><span data-stu-id="8496f-128">5</span></span>|<span data-ttu-id="8496f-129">15A 分类适用于15个或更早的查看者</span><span class="sxs-lookup"><span data-stu-id="8496f-129">The 15A classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="8496f-130">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="8496f-130">agesAbove16</span></span>|<span data-ttu-id="8496f-131">6 </span><span class="sxs-lookup"><span data-stu-id="8496f-131">6</span></span>|<span data-ttu-id="8496f-132">16分类适用于16或更低版本的查看者</span><span class="sxs-lookup"><span data-stu-id="8496f-132">The 16 classification is suitable for viewers of 16 or older</span></span>|
|<span data-ttu-id="8496f-133">成人</span><span class="sxs-lookup"><span data-stu-id="8496f-133">adults</span></span>|<span data-ttu-id="8496f-134">7 </span><span class="sxs-lookup"><span data-stu-id="8496f-134">7</span></span>|<span data-ttu-id="8496f-135">18种分类，仅适用于成年人</span><span class="sxs-lookup"><span data-stu-id="8496f-135">The 18 classification, suitable only for adults</span></span>|



