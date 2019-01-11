---
title: ratingIrelandMoviesType 枚举类型
description: 电影分级在爱尔兰标签
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f5af5fb771821096eb006c0727ef8efb5e45136
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880869"
---
# <a name="ratingirelandmoviestype-enum-type"></a><span data-ttu-id="70a4d-103">ratingIrelandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="70a4d-103">ratingIrelandMoviesType enum type</span></span>

> <span data-ttu-id="70a4d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="70a4d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70a4d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="70a4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70a4d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="70a4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70a4d-107">电影分级在爱尔兰标签</span><span class="sxs-lookup"><span data-stu-id="70a4d-107">Movies rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="70a4d-108">成员</span><span class="sxs-lookup"><span data-stu-id="70a4d-108">Members</span></span>
|<span data-ttu-id="70a4d-109">成员</span><span class="sxs-lookup"><span data-stu-id="70a4d-109">Member</span></span>|<span data-ttu-id="70a4d-110">值</span><span class="sxs-lookup"><span data-stu-id="70a4d-110">Value</span></span>|<span data-ttu-id="70a4d-111">Description</span><span class="sxs-lookup"><span data-stu-id="70a4d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70a4d-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="70a4d-112">allAllowed</span></span>|<span data-ttu-id="70a4d-113">0</span><span class="sxs-lookup"><span data-stu-id="70a4d-113">0</span></span>|<span data-ttu-id="70a4d-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="70a4d-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="70a4d-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="70a4d-115">allBlocked</span></span>|<span data-ttu-id="70a4d-116">1</span><span class="sxs-lookup"><span data-stu-id="70a4d-116">1</span></span>|<span data-ttu-id="70a4d-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="70a4d-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="70a4d-118">常规</span><span class="sxs-lookup"><span data-stu-id="70a4d-118">general</span></span>|<span data-ttu-id="70a4d-119">2</span><span class="sxs-lookup"><span data-stu-id="70a4d-119">2</span></span>|<span data-ttu-id="70a4d-120">适用于学校转期限的子级</span><span class="sxs-lookup"><span data-stu-id="70a4d-120">Suitable for children of school going age</span></span>|
|<span data-ttu-id="70a4d-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="70a4d-121">parentalGuidance</span></span>|<span data-ttu-id="70a4d-122">3</span><span class="sxs-lookup"><span data-stu-id="70a4d-122">3</span></span>|<span data-ttu-id="70a4d-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="70a4d-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="70a4d-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="70a4d-124">agesAbove12</span></span>|<span data-ttu-id="70a4d-125">4</span><span class="sxs-lookup"><span data-stu-id="70a4d-125">4</span></span>|<span data-ttu-id="70a4d-126">12A 分类是合适的查看为 12 或更低</span><span class="sxs-lookup"><span data-stu-id="70a4d-126">The 12A classification is suitable for viewers of 12 or older</span></span>|
|<span data-ttu-id="70a4d-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="70a4d-127">agesAbove15</span></span>|<span data-ttu-id="70a4d-128">5</span><span class="sxs-lookup"><span data-stu-id="70a4d-128">5</span></span>|<span data-ttu-id="70a4d-129">15A 分类是 15 的适用于观众或较旧</span><span class="sxs-lookup"><span data-stu-id="70a4d-129">The 15A classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="70a4d-130">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="70a4d-130">agesAbove16</span></span>|<span data-ttu-id="70a4d-131">6</span><span class="sxs-lookup"><span data-stu-id="70a4d-131">6</span></span>|<span data-ttu-id="70a4d-132">16 分类是 16 的适用于观众或较旧</span><span class="sxs-lookup"><span data-stu-id="70a4d-132">The 16 classification is suitable for viewers of 16 or older</span></span>|
|<span data-ttu-id="70a4d-133">成人</span><span class="sxs-lookup"><span data-stu-id="70a4d-133">adults</span></span>|<span data-ttu-id="70a4d-134">7</span><span class="sxs-lookup"><span data-stu-id="70a4d-134">7</span></span>|<span data-ttu-id="70a4d-135">仅适于成人 18 分类</span><span class="sxs-lookup"><span data-stu-id="70a4d-135">The 18 classification, suitable only for adults</span></span>|





