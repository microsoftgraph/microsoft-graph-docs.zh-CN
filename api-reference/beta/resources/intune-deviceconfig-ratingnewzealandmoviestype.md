---
title: ratingNewZealandMoviesType 枚举类型
description: 新西兰的电影评级标签
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5ac2acd28f0114b69f7f9c508cb3538ebf36fa81
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445010"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="8076b-103">ratingNewZealandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8076b-103">ratingNewZealandMoviesType enum type</span></span>

<span data-ttu-id="8076b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8076b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8076b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8076b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8076b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8076b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8076b-107">新西兰的电影评级标签</span><span class="sxs-lookup"><span data-stu-id="8076b-107">Movies rating labels in New Zealand</span></span>

## <a name="members"></a><span data-ttu-id="8076b-108">成员</span><span class="sxs-lookup"><span data-stu-id="8076b-108">Members</span></span>
|<span data-ttu-id="8076b-109">成员</span><span class="sxs-lookup"><span data-stu-id="8076b-109">Member</span></span>|<span data-ttu-id="8076b-110">值</span><span class="sxs-lookup"><span data-stu-id="8076b-110">Value</span></span>|<span data-ttu-id="8076b-111">说明</span><span class="sxs-lookup"><span data-stu-id="8076b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8076b-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="8076b-112">allAllowed</span></span>|<span data-ttu-id="8076b-113">0</span><span class="sxs-lookup"><span data-stu-id="8076b-113">0</span></span>|<span data-ttu-id="8076b-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="8076b-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="8076b-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="8076b-115">allBlocked</span></span>|<span data-ttu-id="8076b-116">1</span><span class="sxs-lookup"><span data-stu-id="8076b-116">1</span></span>|<span data-ttu-id="8076b-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="8076b-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="8076b-118">概要</span><span class="sxs-lookup"><span data-stu-id="8076b-118">general</span></span>|<span data-ttu-id="8076b-119">双面</span><span class="sxs-lookup"><span data-stu-id="8076b-119">2</span></span>|<span data-ttu-id="8076b-120">适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="8076b-120">Suitable for general audience</span></span>|
|<span data-ttu-id="8076b-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="8076b-121">parentalGuidance</span></span>|<span data-ttu-id="8076b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="8076b-122">3</span></span>|<span data-ttu-id="8076b-123">PG 分类建议家长指南</span><span class="sxs-lookup"><span data-stu-id="8076b-123">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="8076b-124">成熟</span><span class="sxs-lookup"><span data-stu-id="8076b-124">mature</span></span>|<span data-ttu-id="8076b-125">4 </span><span class="sxs-lookup"><span data-stu-id="8076b-125">4</span></span>|<span data-ttu-id="8076b-126">M 分类适用于成熟受众</span><span class="sxs-lookup"><span data-stu-id="8076b-126">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="8076b-127">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="8076b-127">agesAbove13</span></span>|<span data-ttu-id="8076b-128">5 </span><span class="sxs-lookup"><span data-stu-id="8076b-128">5</span></span>|<span data-ttu-id="8076b-129">R13 分类限制为13年以上及以上的人员</span><span class="sxs-lookup"><span data-stu-id="8076b-129">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="8076b-130">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="8076b-130">agesAbove15</span></span>|<span data-ttu-id="8076b-131">6 </span><span class="sxs-lookup"><span data-stu-id="8076b-131">6</span></span>|<span data-ttu-id="8076b-132">R15 分类限制为在15年和以上的人员</span><span class="sxs-lookup"><span data-stu-id="8076b-132">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="8076b-133">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="8076b-133">agesAbove16</span></span>|<span data-ttu-id="8076b-134">7 </span><span class="sxs-lookup"><span data-stu-id="8076b-134">7</span></span>|<span data-ttu-id="8076b-135">R16 分类限制为16年以上及以上的人员</span><span class="sxs-lookup"><span data-stu-id="8076b-135">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="8076b-136">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="8076b-136">agesAbove18</span></span>|<span data-ttu-id="8076b-137">8 </span><span class="sxs-lookup"><span data-stu-id="8076b-137">8</span></span>|<span data-ttu-id="8076b-138">R18 分类限制为18年以上及以上的人员</span><span class="sxs-lookup"><span data-stu-id="8076b-138">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="8076b-139">受限</span><span class="sxs-lookup"><span data-stu-id="8076b-139">restricted</span></span>|<span data-ttu-id="8076b-140">9 </span><span class="sxs-lookup"><span data-stu-id="8076b-140">9</span></span>|<span data-ttu-id="8076b-141">将 R 分类限制为特定访问群体</span><span class="sxs-lookup"><span data-stu-id="8076b-141">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="8076b-142">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="8076b-142">agesAbove16Restricted</span></span>|<span data-ttu-id="8076b-143">10 </span><span class="sxs-lookup"><span data-stu-id="8076b-143">10</span></span>|<span data-ttu-id="8076b-144">RP16 分类要求在16下有一个父或成年人的查看者</span><span class="sxs-lookup"><span data-stu-id="8076b-144">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|



