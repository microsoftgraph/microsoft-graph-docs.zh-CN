---
title: ratingIrelandMoviesType 枚举类型
description: 电影分级在爱尔兰标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1e9103c3e756f95d2ce7d06899f40571a366faba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394402"
---
# <a name="ratingirelandmoviestype-enum-type"></a><span data-ttu-id="e14e6-103">ratingIrelandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e14e6-103">ratingIrelandMoviesType enum type</span></span>

> <span data-ttu-id="e14e6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e14e6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e14e6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e14e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e14e6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e14e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e14e6-107">电影分级在爱尔兰标签</span><span class="sxs-lookup"><span data-stu-id="e14e6-107">Movies rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="e14e6-108">成员</span><span class="sxs-lookup"><span data-stu-id="e14e6-108">Members</span></span>
|<span data-ttu-id="e14e6-109">成员</span><span class="sxs-lookup"><span data-stu-id="e14e6-109">Member</span></span>|<span data-ttu-id="e14e6-110">值</span><span class="sxs-lookup"><span data-stu-id="e14e6-110">Value</span></span>|<span data-ttu-id="e14e6-111">说明</span><span class="sxs-lookup"><span data-stu-id="e14e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e14e6-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="e14e6-112">allAllowed</span></span>|<span data-ttu-id="e14e6-113">0</span><span class="sxs-lookup"><span data-stu-id="e14e6-113">0</span></span>|<span data-ttu-id="e14e6-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="e14e6-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="e14e6-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="e14e6-115">allBlocked</span></span>|<span data-ttu-id="e14e6-116">1</span><span class="sxs-lookup"><span data-stu-id="e14e6-116">1</span></span>|<span data-ttu-id="e14e6-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="e14e6-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="e14e6-118">常规</span><span class="sxs-lookup"><span data-stu-id="e14e6-118">general</span></span>|<span data-ttu-id="e14e6-119">2</span><span class="sxs-lookup"><span data-stu-id="e14e6-119">2</span></span>|<span data-ttu-id="e14e6-120">适用于学校转期限的子级</span><span class="sxs-lookup"><span data-stu-id="e14e6-120">Suitable for children of school going age</span></span>|
|<span data-ttu-id="e14e6-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="e14e6-121">parentalGuidance</span></span>|<span data-ttu-id="e14e6-122">3</span><span class="sxs-lookup"><span data-stu-id="e14e6-122">3</span></span>|<span data-ttu-id="e14e6-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="e14e6-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="e14e6-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="e14e6-124">agesAbove12</span></span>|<span data-ttu-id="e14e6-125">4</span><span class="sxs-lookup"><span data-stu-id="e14e6-125">4</span></span>|<span data-ttu-id="e14e6-126">12A 分类是合适的查看为 12 或更低</span><span class="sxs-lookup"><span data-stu-id="e14e6-126">The 12A classification is suitable for viewers of 12 or older</span></span>|
|<span data-ttu-id="e14e6-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="e14e6-127">agesAbove15</span></span>|<span data-ttu-id="e14e6-128">5</span><span class="sxs-lookup"><span data-stu-id="e14e6-128">5</span></span>|<span data-ttu-id="e14e6-129">15A 分类是 15 的适用于观众或较旧</span><span class="sxs-lookup"><span data-stu-id="e14e6-129">The 15A classification is suitable for viewers of 15 or older</span></span>|
|<span data-ttu-id="e14e6-130">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="e14e6-130">agesAbove16</span></span>|<span data-ttu-id="e14e6-131">6</span><span class="sxs-lookup"><span data-stu-id="e14e6-131">6</span></span>|<span data-ttu-id="e14e6-132">16 分类是 16 的适用于观众或较旧</span><span class="sxs-lookup"><span data-stu-id="e14e6-132">The 16 classification is suitable for viewers of 16 or older</span></span>|
|<span data-ttu-id="e14e6-133">成人</span><span class="sxs-lookup"><span data-stu-id="e14e6-133">adults</span></span>|<span data-ttu-id="e14e6-134">7</span><span class="sxs-lookup"><span data-stu-id="e14e6-134">7</span></span>|<span data-ttu-id="e14e6-135">仅适于成人 18 分类</span><span class="sxs-lookup"><span data-stu-id="e14e6-135">The 18 classification, suitable only for adults</span></span>|




