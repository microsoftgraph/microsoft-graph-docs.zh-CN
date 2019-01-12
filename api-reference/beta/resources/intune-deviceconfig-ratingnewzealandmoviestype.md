---
title: ratingNewZealandMoviesType 枚举类型
description: 电影分级新西兰标签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 47f66e28992136104f9fc3317e470278001fb14e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952550"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="1a266-103">ratingNewZealandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1a266-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="1a266-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1a266-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a266-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a266-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a266-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1a266-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a266-107">电影分级新西兰标签</span><span class="sxs-lookup"><span data-stu-id="1a266-107">Movies rating labels in New Zealand</span></span>
## <a name="members"></a><span data-ttu-id="1a266-108">成员</span><span class="sxs-lookup"><span data-stu-id="1a266-108">Members</span></span>
|<span data-ttu-id="1a266-109">成员</span><span class="sxs-lookup"><span data-stu-id="1a266-109">Member</span></span>|<span data-ttu-id="1a266-110">值</span><span class="sxs-lookup"><span data-stu-id="1a266-110">Value</span></span>|<span data-ttu-id="1a266-111">Description</span><span class="sxs-lookup"><span data-stu-id="1a266-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a266-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="1a266-112">allAllowed</span></span>|<span data-ttu-id="1a266-113">0</span><span class="sxs-lookup"><span data-stu-id="1a266-113">0</span></span>|<span data-ttu-id="1a266-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="1a266-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="1a266-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="1a266-115">allBlocked</span></span>|<span data-ttu-id="1a266-116">1</span><span class="sxs-lookup"><span data-stu-id="1a266-116">1</span></span>|<span data-ttu-id="1a266-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="1a266-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="1a266-118">常规</span><span class="sxs-lookup"><span data-stu-id="1a266-118">general</span></span>|<span data-ttu-id="1a266-119">2</span><span class="sxs-lookup"><span data-stu-id="1a266-119">2</span></span>|<span data-ttu-id="1a266-120">适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="1a266-120">Suitable for general audience</span></span>|
|<span data-ttu-id="1a266-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="1a266-121">parentalGuidance</span></span>|<span data-ttu-id="1a266-122">3</span><span class="sxs-lookup"><span data-stu-id="1a266-122">3</span></span>|<span data-ttu-id="1a266-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="1a266-123">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="1a266-124">成熟的</span><span class="sxs-lookup"><span data-stu-id="1a266-124">mature</span></span>|<span data-ttu-id="1a266-125">4</span><span class="sxs-lookup"><span data-stu-id="1a266-125">4</span></span>|<span data-ttu-id="1a266-126">M 分类适合成熟的访问群体</span><span class="sxs-lookup"><span data-stu-id="1a266-126">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="1a266-127">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="1a266-127">agesAbove13</span></span>|<span data-ttu-id="1a266-128">5</span><span class="sxs-lookup"><span data-stu-id="1a266-128">5</span></span>|<span data-ttu-id="1a266-129">R13 分类是人员 13 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="1a266-129">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="1a266-130">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="1a266-130">agesAbove15</span></span>|<span data-ttu-id="1a266-131">6</span><span class="sxs-lookup"><span data-stu-id="1a266-131">6</span></span>|<span data-ttu-id="1a266-132">R15 分类是人员 15 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="1a266-132">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="1a266-133">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="1a266-133">agesAbove16</span></span>|<span data-ttu-id="1a266-134">7</span><span class="sxs-lookup"><span data-stu-id="1a266-134">7</span></span>|<span data-ttu-id="1a266-135">R16 分类是人员 16 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="1a266-135">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="1a266-136">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="1a266-136">agesAbove18</span></span>|<span data-ttu-id="1a266-137">8</span><span class="sxs-lookup"><span data-stu-id="1a266-137">8</span></span>|<span data-ttu-id="1a266-138">R18 分类是人员年满 18 周岁与通过限制</span><span class="sxs-lookup"><span data-stu-id="1a266-138">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="1a266-139">受限制</span><span class="sxs-lookup"><span data-stu-id="1a266-139">restricted</span></span>|<span data-ttu-id="1a266-140">9</span><span class="sxs-lookup"><span data-stu-id="1a266-140">9</span></span>|<span data-ttu-id="1a266-141">R 分类被限制为特定访问群体</span><span class="sxs-lookup"><span data-stu-id="1a266-141">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="1a266-142">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="1a266-142">agesAbove16Restricted</span></span>|<span data-ttu-id="1a266-143">10</span><span class="sxs-lookup"><span data-stu-id="1a266-143">10</span></span>|<span data-ttu-id="1a266-144">RP16 分类需要查看在由父或成人附带的 16</span><span class="sxs-lookup"><span data-stu-id="1a266-144">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|





