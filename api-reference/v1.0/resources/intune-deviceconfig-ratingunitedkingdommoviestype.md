---
title: ratingUnitedKingdomMoviesType 枚举类型
description: 电影分级中英国标签
author: tfitzmac
ms.openlocfilehash: 6593ff7f65e49b103c0a7004f3f701bbe9590a2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334480"
---
# <a name="ratingunitedkingdommoviestype-enum-type"></a><span data-ttu-id="716fc-103">ratingUnitedKingdomMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="716fc-103">ratingUnitedKingdomMoviesType enum type</span></span>

> <span data-ttu-id="716fc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="716fc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="716fc-105">电影分级中英国标签</span><span class="sxs-lookup"><span data-stu-id="716fc-105">Movies rating labels in United Kingdom</span></span>
## <a name="members"></a><span data-ttu-id="716fc-106">成员</span><span class="sxs-lookup"><span data-stu-id="716fc-106">Members</span></span>
|<span data-ttu-id="716fc-107">成员</span><span class="sxs-lookup"><span data-stu-id="716fc-107">Member</span></span>|<span data-ttu-id="716fc-108">值</span><span class="sxs-lookup"><span data-stu-id="716fc-108">Value</span></span>|<span data-ttu-id="716fc-109">说明</span><span class="sxs-lookup"><span data-stu-id="716fc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="716fc-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="716fc-110">allAllowed</span></span>|<span data-ttu-id="716fc-111">0</span><span class="sxs-lookup"><span data-stu-id="716fc-111">0</span></span>|<span data-ttu-id="716fc-112">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="716fc-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="716fc-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="716fc-113">allBlocked</span></span>|<span data-ttu-id="716fc-114">1</span><span class="sxs-lookup"><span data-stu-id="716fc-114">1</span></span>|<span data-ttu-id="716fc-115">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="716fc-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="716fc-116">常规</span><span class="sxs-lookup"><span data-stu-id="716fc-116">general</span></span>|<span data-ttu-id="716fc-117">2</span><span class="sxs-lookup"><span data-stu-id="716fc-117">2</span></span>|<span data-ttu-id="716fc-118">U 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="716fc-118">The U classification is suitable for all ages</span></span>|
|<span data-ttu-id="716fc-119">universalChildren</span><span class="sxs-lookup"><span data-stu-id="716fc-119">universalChildren</span></span>|<span data-ttu-id="716fc-120">3</span><span class="sxs-lookup"><span data-stu-id="716fc-120">3</span></span>|<span data-ttu-id="716fc-121">UC 分类适合前学校子级，旧的分级标签</span><span class="sxs-lookup"><span data-stu-id="716fc-121">The UC classification is suitable for pre-school children, an old rating label</span></span>|
|<span data-ttu-id="716fc-122">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="716fc-122">parentalGuidance</span></span>|<span data-ttu-id="716fc-123">4</span><span class="sxs-lookup"><span data-stu-id="716fc-123">4</span></span>|<span data-ttu-id="716fc-124">PG 分类适合成熟</span><span class="sxs-lookup"><span data-stu-id="716fc-124">The PG classification is suitable for mature</span></span>|
|<span data-ttu-id="716fc-125">agesAbove12Video</span><span class="sxs-lookup"><span data-stu-id="716fc-125">agesAbove12Video</span></span>|<span data-ttu-id="716fc-126">5</span><span class="sxs-lookup"><span data-stu-id="716fc-126">5</span></span>|<span data-ttu-id="716fc-127">12 年时间，通过，12，视频释放合适</span><span class="sxs-lookup"><span data-stu-id="716fc-127">12, video release suitable for 12 years and over</span></span>|
|<span data-ttu-id="716fc-128">agesAbove12Cinema</span><span class="sxs-lookup"><span data-stu-id="716fc-128">agesAbove12Cinema</span></span>|<span data-ttu-id="716fc-129">6</span><span class="sxs-lookup"><span data-stu-id="716fc-129">6</span></span>|<span data-ttu-id="716fc-130">12A，12 年时间，通过合适的电影版</span><span class="sxs-lookup"><span data-stu-id="716fc-130">12A, cinema release suitable for 12 years and over</span></span>|
|<span data-ttu-id="716fc-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="716fc-131">agesAbove15</span></span>|<span data-ttu-id="716fc-132">7</span><span class="sxs-lookup"><span data-stu-id="716fc-132">7</span></span>|<span data-ttu-id="716fc-133">15，只适合 15 年及较早</span><span class="sxs-lookup"><span data-stu-id="716fc-133">15, suitable only for 15 years and older</span></span>|
|<span data-ttu-id="716fc-134">成人</span><span class="sxs-lookup"><span data-stu-id="716fc-134">adults</span></span>|<span data-ttu-id="716fc-135">8</span><span class="sxs-lookup"><span data-stu-id="716fc-135">8</span></span>|<span data-ttu-id="716fc-136">仅适于成人</span><span class="sxs-lookup"><span data-stu-id="716fc-136">Suitable only for adults</span></span>|



