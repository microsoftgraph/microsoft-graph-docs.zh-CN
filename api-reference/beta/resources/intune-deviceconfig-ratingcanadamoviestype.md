---
title: ratingCanadaMoviesType 枚举类型
description: 电影分级加拿大标签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 469bbf1b177df8bdf40dcdfea4ef6b0c4721cd3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918474"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="b55a2-103">ratingCanadaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b55a2-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="b55a2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b55a2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b55a2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b55a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b55a2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b55a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b55a2-107">电影分级加拿大标签</span><span class="sxs-lookup"><span data-stu-id="b55a2-107">Movies rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="b55a2-108">成员</span><span class="sxs-lookup"><span data-stu-id="b55a2-108">Members</span></span>
|<span data-ttu-id="b55a2-109">成员</span><span class="sxs-lookup"><span data-stu-id="b55a2-109">Member</span></span>|<span data-ttu-id="b55a2-110">值</span><span class="sxs-lookup"><span data-stu-id="b55a2-110">Value</span></span>|<span data-ttu-id="b55a2-111">Description</span><span class="sxs-lookup"><span data-stu-id="b55a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b55a2-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="b55a2-112">allAllowed</span></span>|<span data-ttu-id="b55a2-113">0</span><span class="sxs-lookup"><span data-stu-id="b55a2-113">0</span></span>|<span data-ttu-id="b55a2-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="b55a2-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="b55a2-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="b55a2-115">allBlocked</span></span>|<span data-ttu-id="b55a2-116">1</span><span class="sxs-lookup"><span data-stu-id="b55a2-116">1</span></span>|<span data-ttu-id="b55a2-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="b55a2-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="b55a2-118">常规</span><span class="sxs-lookup"><span data-stu-id="b55a2-118">general</span></span>|<span data-ttu-id="b55a2-119">2</span><span class="sxs-lookup"><span data-stu-id="b55a2-119">2</span></span>|<span data-ttu-id="b55a2-120">G 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="b55a2-120">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="b55a2-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="b55a2-121">parentalGuidance</span></span>|<span data-ttu-id="b55a2-122">3</span><span class="sxs-lookup"><span data-stu-id="b55a2-122">3</span></span>|<span data-ttu-id="b55a2-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="b55a2-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="b55a2-124">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="b55a2-124">agesAbove14</span></span>|<span data-ttu-id="b55a2-125">4</span><span class="sxs-lookup"><span data-stu-id="b55a2-125">4</span></span>|<span data-ttu-id="b55a2-126">14A 分类适于上面 14 或更低的查看者</span><span class="sxs-lookup"><span data-stu-id="b55a2-126">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="b55a2-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="b55a2-127">agesAbove18</span></span>|<span data-ttu-id="b55a2-128">5</span><span class="sxs-lookup"><span data-stu-id="b55a2-128">5</span></span>|<span data-ttu-id="b55a2-129">18A 分类适于上面 18 或更低的查看者</span><span class="sxs-lookup"><span data-stu-id="b55a2-129">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="b55a2-130">受限制</span><span class="sxs-lookup"><span data-stu-id="b55a2-130">restricted</span></span>|<span data-ttu-id="b55a2-131">6</span><span class="sxs-lookup"><span data-stu-id="b55a2-131">6</span></span>|<span data-ttu-id="b55a2-132">R 分类是限制为 18 年及较早</span><span class="sxs-lookup"><span data-stu-id="b55a2-132">The R classification is restricted to 18 years and older</span></span>|





