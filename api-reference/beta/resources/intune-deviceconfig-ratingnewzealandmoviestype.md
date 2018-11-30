---
title: ratingNewZealandMoviesType 枚举类型
description: 电影分级新西兰标签
ms.openlocfilehash: eb32d047c4c24e2848e71ab7cc0947d57048d75d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041640"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="36cb3-103">ratingNewZealandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="36cb3-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="36cb3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="36cb3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36cb3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="36cb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36cb3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="36cb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36cb3-107">电影分级新西兰标签</span><span class="sxs-lookup"><span data-stu-id="36cb3-107">Movies rating labels in New Zealand</span></span>
## <a name="members"></a><span data-ttu-id="36cb3-108">成员</span><span class="sxs-lookup"><span data-stu-id="36cb3-108">Members</span></span>
|<span data-ttu-id="36cb3-109">成员</span><span class="sxs-lookup"><span data-stu-id="36cb3-109">Member</span></span>|<span data-ttu-id="36cb3-110">值</span><span class="sxs-lookup"><span data-stu-id="36cb3-110">Value</span></span>|<span data-ttu-id="36cb3-111">说明</span><span class="sxs-lookup"><span data-stu-id="36cb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36cb3-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="36cb3-112">allAllowed</span></span>|<span data-ttu-id="36cb3-113">0</span><span class="sxs-lookup"><span data-stu-id="36cb3-113">0</span></span>|<span data-ttu-id="36cb3-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="36cb3-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="36cb3-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="36cb3-115">allBlocked</span></span>|<span data-ttu-id="36cb3-116">1</span><span class="sxs-lookup"><span data-stu-id="36cb3-116">1</span></span>|<span data-ttu-id="36cb3-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="36cb3-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="36cb3-118">常规</span><span class="sxs-lookup"><span data-stu-id="36cb3-118">general</span></span>|<span data-ttu-id="36cb3-119">2</span><span class="sxs-lookup"><span data-stu-id="36cb3-119">2</span></span>|<span data-ttu-id="36cb3-120">适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="36cb3-120">Suitable for general audience</span></span>|
|<span data-ttu-id="36cb3-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="36cb3-121">parentalGuidance</span></span>|<span data-ttu-id="36cb3-122">3</span><span class="sxs-lookup"><span data-stu-id="36cb3-122">3</span></span>|<span data-ttu-id="36cb3-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="36cb3-123">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="36cb3-124">成熟的</span><span class="sxs-lookup"><span data-stu-id="36cb3-124">mature</span></span>|<span data-ttu-id="36cb3-125">4</span><span class="sxs-lookup"><span data-stu-id="36cb3-125">4</span></span>|<span data-ttu-id="36cb3-126">M 分类适合成熟的访问群体</span><span class="sxs-lookup"><span data-stu-id="36cb3-126">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="36cb3-127">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="36cb3-127">agesAbove13</span></span>|<span data-ttu-id="36cb3-128">5</span><span class="sxs-lookup"><span data-stu-id="36cb3-128">5</span></span>|<span data-ttu-id="36cb3-129">R13 分类是人员 13 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="36cb3-129">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="36cb3-130">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="36cb3-130">agesAbove15</span></span>|<span data-ttu-id="36cb3-131">6</span><span class="sxs-lookup"><span data-stu-id="36cb3-131">6</span></span>|<span data-ttu-id="36cb3-132">R15 分类是人员 15 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="36cb3-132">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="36cb3-133">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="36cb3-133">agesAbove16</span></span>|<span data-ttu-id="36cb3-134">7</span><span class="sxs-lookup"><span data-stu-id="36cb3-134">7</span></span>|<span data-ttu-id="36cb3-135">R16 分类是人员 16 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="36cb3-135">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="36cb3-136">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="36cb3-136">agesAbove18</span></span>|<span data-ttu-id="36cb3-137">8</span><span class="sxs-lookup"><span data-stu-id="36cb3-137">8</span></span>|<span data-ttu-id="36cb3-138">R18 分类是人员年满 18 周岁与通过限制</span><span class="sxs-lookup"><span data-stu-id="36cb3-138">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="36cb3-139">受限制</span><span class="sxs-lookup"><span data-stu-id="36cb3-139">restricted</span></span>|<span data-ttu-id="36cb3-140">9</span><span class="sxs-lookup"><span data-stu-id="36cb3-140">9</span></span>|<span data-ttu-id="36cb3-141">R 分类被限制为特定访问群体</span><span class="sxs-lookup"><span data-stu-id="36cb3-141">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="36cb3-142">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="36cb3-142">agesAbove16Restricted</span></span>|<span data-ttu-id="36cb3-143">10</span><span class="sxs-lookup"><span data-stu-id="36cb3-143">10</span></span>|<span data-ttu-id="36cb3-144">RP16 分类需要查看在由父或成人附带的 16</span><span class="sxs-lookup"><span data-stu-id="36cb3-144">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|





