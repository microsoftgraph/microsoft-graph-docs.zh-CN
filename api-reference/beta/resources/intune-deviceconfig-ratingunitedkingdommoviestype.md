---
title: ratingUnitedKingdomMoviesType 枚举类型
description: 电影分级中英国标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62194038006b011fdc8a70c4b399beef5e8c742b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412532"
---
# <a name="ratingunitedkingdommoviestype-enum-type"></a><span data-ttu-id="f819a-103">ratingUnitedKingdomMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f819a-103">ratingUnitedKingdomMoviesType enum type</span></span>

> <span data-ttu-id="f819a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f819a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f819a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f819a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f819a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f819a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f819a-107">电影分级中英国标签</span><span class="sxs-lookup"><span data-stu-id="f819a-107">Movies rating labels in United Kingdom</span></span>

## <a name="members"></a><span data-ttu-id="f819a-108">成员</span><span class="sxs-lookup"><span data-stu-id="f819a-108">Members</span></span>
|<span data-ttu-id="f819a-109">成员</span><span class="sxs-lookup"><span data-stu-id="f819a-109">Member</span></span>|<span data-ttu-id="f819a-110">值</span><span class="sxs-lookup"><span data-stu-id="f819a-110">Value</span></span>|<span data-ttu-id="f819a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f819a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f819a-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f819a-112">allAllowed</span></span>|<span data-ttu-id="f819a-113">0</span><span class="sxs-lookup"><span data-stu-id="f819a-113">0</span></span>|<span data-ttu-id="f819a-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="f819a-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="f819a-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f819a-115">allBlocked</span></span>|<span data-ttu-id="f819a-116">1</span><span class="sxs-lookup"><span data-stu-id="f819a-116">1</span></span>|<span data-ttu-id="f819a-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="f819a-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="f819a-118">常规</span><span class="sxs-lookup"><span data-stu-id="f819a-118">general</span></span>|<span data-ttu-id="f819a-119">2</span><span class="sxs-lookup"><span data-stu-id="f819a-119">2</span></span>|<span data-ttu-id="f819a-120">U 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="f819a-120">The U classification is suitable for all ages</span></span>|
|<span data-ttu-id="f819a-121">universalChildren</span><span class="sxs-lookup"><span data-stu-id="f819a-121">universalChildren</span></span>|<span data-ttu-id="f819a-122">3</span><span class="sxs-lookup"><span data-stu-id="f819a-122">3</span></span>|<span data-ttu-id="f819a-123">UC 分类适合前学校子级，旧的分级标签</span><span class="sxs-lookup"><span data-stu-id="f819a-123">The UC classification is suitable for pre-school children, an old rating label</span></span>|
|<span data-ttu-id="f819a-124">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="f819a-124">parentalGuidance</span></span>|<span data-ttu-id="f819a-125">4</span><span class="sxs-lookup"><span data-stu-id="f819a-125">4</span></span>|<span data-ttu-id="f819a-126">PG 分类适合成熟</span><span class="sxs-lookup"><span data-stu-id="f819a-126">The PG classification is suitable for mature</span></span>|
|<span data-ttu-id="f819a-127">agesAbove12Video</span><span class="sxs-lookup"><span data-stu-id="f819a-127">agesAbove12Video</span></span>|<span data-ttu-id="f819a-128">5</span><span class="sxs-lookup"><span data-stu-id="f819a-128">5</span></span>|<span data-ttu-id="f819a-129">12 年时间，通过，12，视频释放合适</span><span class="sxs-lookup"><span data-stu-id="f819a-129">12, video release suitable for 12 years and over</span></span>|
|<span data-ttu-id="f819a-130">agesAbove12Cinema</span><span class="sxs-lookup"><span data-stu-id="f819a-130">agesAbove12Cinema</span></span>|<span data-ttu-id="f819a-131">6</span><span class="sxs-lookup"><span data-stu-id="f819a-131">6</span></span>|<span data-ttu-id="f819a-132">12A，12 年时间，通过合适的电影版</span><span class="sxs-lookup"><span data-stu-id="f819a-132">12A, cinema release suitable for 12 years and over</span></span>|
|<span data-ttu-id="f819a-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="f819a-133">agesAbove15</span></span>|<span data-ttu-id="f819a-134">7</span><span class="sxs-lookup"><span data-stu-id="f819a-134">7</span></span>|<span data-ttu-id="f819a-135">15，只适合 15 年及较早</span><span class="sxs-lookup"><span data-stu-id="f819a-135">15, suitable only for 15 years and older</span></span>|
|<span data-ttu-id="f819a-136">成人</span><span class="sxs-lookup"><span data-stu-id="f819a-136">adults</span></span>|<span data-ttu-id="f819a-137">8</span><span class="sxs-lookup"><span data-stu-id="f819a-137">8</span></span>|<span data-ttu-id="f819a-138">仅适于成人</span><span class="sxs-lookup"><span data-stu-id="f819a-138">Suitable only for adults</span></span>|




