---
title: ratingUnitedKingdomMoviesType 枚举类型
description: 电影分级中英国标签
author: tfitzmac
ms.openlocfilehash: ec8d134cc1ca3425c7503f6b072d37d88990191c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332387"
---
# <a name="ratingunitedkingdommoviestype-enum-type"></a><span data-ttu-id="1dc85-103">ratingUnitedKingdomMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1dc85-103">ratingUnitedKingdomMoviesType enum type</span></span>

> <span data-ttu-id="1dc85-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1dc85-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1dc85-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1dc85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1dc85-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1dc85-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dc85-107">电影分级中英国标签</span><span class="sxs-lookup"><span data-stu-id="1dc85-107">Movies rating labels in United Kingdom</span></span>
## <a name="members"></a><span data-ttu-id="1dc85-108">成员</span><span class="sxs-lookup"><span data-stu-id="1dc85-108">Members</span></span>
|<span data-ttu-id="1dc85-109">成员</span><span class="sxs-lookup"><span data-stu-id="1dc85-109">Member</span></span>|<span data-ttu-id="1dc85-110">值</span><span class="sxs-lookup"><span data-stu-id="1dc85-110">Value</span></span>|<span data-ttu-id="1dc85-111">说明</span><span class="sxs-lookup"><span data-stu-id="1dc85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dc85-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="1dc85-112">allAllowed</span></span>|<span data-ttu-id="1dc85-113">0</span><span class="sxs-lookup"><span data-stu-id="1dc85-113">0</span></span>|<span data-ttu-id="1dc85-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="1dc85-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="1dc85-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="1dc85-115">allBlocked</span></span>|<span data-ttu-id="1dc85-116">1</span><span class="sxs-lookup"><span data-stu-id="1dc85-116">1</span></span>|<span data-ttu-id="1dc85-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="1dc85-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="1dc85-118">常规</span><span class="sxs-lookup"><span data-stu-id="1dc85-118">general</span></span>|<span data-ttu-id="1dc85-119">2</span><span class="sxs-lookup"><span data-stu-id="1dc85-119">2</span></span>|<span data-ttu-id="1dc85-120">U 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="1dc85-120">The U classification is suitable for all ages</span></span>|
|<span data-ttu-id="1dc85-121">universalChildren</span><span class="sxs-lookup"><span data-stu-id="1dc85-121">universalChildren</span></span>|<span data-ttu-id="1dc85-122">3</span><span class="sxs-lookup"><span data-stu-id="1dc85-122">3</span></span>|<span data-ttu-id="1dc85-123">UC 分类适合前学校子级，旧的分级标签</span><span class="sxs-lookup"><span data-stu-id="1dc85-123">The UC classification is suitable for pre-school children, an old rating label</span></span>|
|<span data-ttu-id="1dc85-124">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="1dc85-124">parentalGuidance</span></span>|<span data-ttu-id="1dc85-125">4</span><span class="sxs-lookup"><span data-stu-id="1dc85-125">4</span></span>|<span data-ttu-id="1dc85-126">PG 分类适合成熟</span><span class="sxs-lookup"><span data-stu-id="1dc85-126">The PG classification is suitable for mature</span></span>|
|<span data-ttu-id="1dc85-127">agesAbove12Video</span><span class="sxs-lookup"><span data-stu-id="1dc85-127">agesAbove12Video</span></span>|<span data-ttu-id="1dc85-128">5</span><span class="sxs-lookup"><span data-stu-id="1dc85-128">5</span></span>|<span data-ttu-id="1dc85-129">12 年时间，通过，12，视频释放合适</span><span class="sxs-lookup"><span data-stu-id="1dc85-129">12, video release suitable for 12 years and over</span></span>|
|<span data-ttu-id="1dc85-130">agesAbove12Cinema</span><span class="sxs-lookup"><span data-stu-id="1dc85-130">agesAbove12Cinema</span></span>|<span data-ttu-id="1dc85-131">6</span><span class="sxs-lookup"><span data-stu-id="1dc85-131">6</span></span>|<span data-ttu-id="1dc85-132">12A，12 年时间，通过合适的电影版</span><span class="sxs-lookup"><span data-stu-id="1dc85-132">12A, cinema release suitable for 12 years and over</span></span>|
|<span data-ttu-id="1dc85-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="1dc85-133">agesAbove15</span></span>|<span data-ttu-id="1dc85-134">7</span><span class="sxs-lookup"><span data-stu-id="1dc85-134">7</span></span>|<span data-ttu-id="1dc85-135">15，只适合 15 年及较早</span><span class="sxs-lookup"><span data-stu-id="1dc85-135">15, suitable only for 15 years and older</span></span>|
|<span data-ttu-id="1dc85-136">成人</span><span class="sxs-lookup"><span data-stu-id="1dc85-136">adults</span></span>|<span data-ttu-id="1dc85-137">8</span><span class="sxs-lookup"><span data-stu-id="1dc85-137">8</span></span>|<span data-ttu-id="1dc85-138">仅适于成人</span><span class="sxs-lookup"><span data-stu-id="1dc85-138">Suitable only for adults</span></span>|





