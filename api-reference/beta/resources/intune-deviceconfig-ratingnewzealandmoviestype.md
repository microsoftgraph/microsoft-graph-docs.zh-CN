---
title: ratingNewZealandMoviesType 枚举类型
description: 电影分级新西兰标签
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 220348375503cca6ab42a9573b8ed5b5850192e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884019"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="d53bf-103">ratingNewZealandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d53bf-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="d53bf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d53bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d53bf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d53bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d53bf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d53bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d53bf-107">电影分级新西兰标签</span><span class="sxs-lookup"><span data-stu-id="d53bf-107">Movies rating labels in New Zealand</span></span>
## <a name="members"></a><span data-ttu-id="d53bf-108">成员</span><span class="sxs-lookup"><span data-stu-id="d53bf-108">Members</span></span>
|<span data-ttu-id="d53bf-109">成员</span><span class="sxs-lookup"><span data-stu-id="d53bf-109">Member</span></span>|<span data-ttu-id="d53bf-110">值</span><span class="sxs-lookup"><span data-stu-id="d53bf-110">Value</span></span>|<span data-ttu-id="d53bf-111">Description</span><span class="sxs-lookup"><span data-stu-id="d53bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d53bf-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="d53bf-112">allAllowed</span></span>|<span data-ttu-id="d53bf-113">0</span><span class="sxs-lookup"><span data-stu-id="d53bf-113">0</span></span>|<span data-ttu-id="d53bf-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="d53bf-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="d53bf-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="d53bf-115">allBlocked</span></span>|<span data-ttu-id="d53bf-116">1</span><span class="sxs-lookup"><span data-stu-id="d53bf-116">1</span></span>|<span data-ttu-id="d53bf-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="d53bf-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="d53bf-118">常规</span><span class="sxs-lookup"><span data-stu-id="d53bf-118">general</span></span>|<span data-ttu-id="d53bf-119">2</span><span class="sxs-lookup"><span data-stu-id="d53bf-119">2</span></span>|<span data-ttu-id="d53bf-120">适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="d53bf-120">Suitable for general audience</span></span>|
|<span data-ttu-id="d53bf-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="d53bf-121">parentalGuidance</span></span>|<span data-ttu-id="d53bf-122">3</span><span class="sxs-lookup"><span data-stu-id="d53bf-122">3</span></span>|<span data-ttu-id="d53bf-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="d53bf-123">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="d53bf-124">成熟的</span><span class="sxs-lookup"><span data-stu-id="d53bf-124">mature</span></span>|<span data-ttu-id="d53bf-125">4</span><span class="sxs-lookup"><span data-stu-id="d53bf-125">4</span></span>|<span data-ttu-id="d53bf-126">M 分类适合成熟的访问群体</span><span class="sxs-lookup"><span data-stu-id="d53bf-126">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="d53bf-127">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="d53bf-127">agesAbove13</span></span>|<span data-ttu-id="d53bf-128">5</span><span class="sxs-lookup"><span data-stu-id="d53bf-128">5</span></span>|<span data-ttu-id="d53bf-129">R13 分类是人员 13 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="d53bf-129">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="d53bf-130">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="d53bf-130">agesAbove15</span></span>|<span data-ttu-id="d53bf-131">6</span><span class="sxs-lookup"><span data-stu-id="d53bf-131">6</span></span>|<span data-ttu-id="d53bf-132">R15 分类是人员 15 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="d53bf-132">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="d53bf-133">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="d53bf-133">agesAbove16</span></span>|<span data-ttu-id="d53bf-134">7</span><span class="sxs-lookup"><span data-stu-id="d53bf-134">7</span></span>|<span data-ttu-id="d53bf-135">R16 分类是人员 16 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="d53bf-135">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="d53bf-136">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="d53bf-136">agesAbove18</span></span>|<span data-ttu-id="d53bf-137">8</span><span class="sxs-lookup"><span data-stu-id="d53bf-137">8</span></span>|<span data-ttu-id="d53bf-138">R18 分类是人员年满 18 周岁与通过限制</span><span class="sxs-lookup"><span data-stu-id="d53bf-138">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="d53bf-139">受限制</span><span class="sxs-lookup"><span data-stu-id="d53bf-139">restricted</span></span>|<span data-ttu-id="d53bf-140">9</span><span class="sxs-lookup"><span data-stu-id="d53bf-140">9</span></span>|<span data-ttu-id="d53bf-141">R 分类被限制为特定访问群体</span><span class="sxs-lookup"><span data-stu-id="d53bf-141">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="d53bf-142">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="d53bf-142">agesAbove16Restricted</span></span>|<span data-ttu-id="d53bf-143">10</span><span class="sxs-lookup"><span data-stu-id="d53bf-143">10</span></span>|<span data-ttu-id="d53bf-144">RP16 分类需要查看在由父或成人附带的 16</span><span class="sxs-lookup"><span data-stu-id="d53bf-144">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|





