---
title: ratingNewZealandMoviesType 枚举类型
description: 电影分级新西兰标签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 19a49c19241446b0a3d5b53074b54dafd152ac8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986367"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="793fc-103">ratingNewZealandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="793fc-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="793fc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="793fc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="793fc-105">电影分级新西兰标签</span><span class="sxs-lookup"><span data-stu-id="793fc-105">Movies rating labels in New Zealand</span></span>
## <a name="members"></a><span data-ttu-id="793fc-106">成员</span><span class="sxs-lookup"><span data-stu-id="793fc-106">Members</span></span>
|<span data-ttu-id="793fc-107">成员</span><span class="sxs-lookup"><span data-stu-id="793fc-107">Member</span></span>|<span data-ttu-id="793fc-108">值</span><span class="sxs-lookup"><span data-stu-id="793fc-108">Value</span></span>|<span data-ttu-id="793fc-109">说明</span><span class="sxs-lookup"><span data-stu-id="793fc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="793fc-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="793fc-110">allAllowed</span></span>|<span data-ttu-id="793fc-111">0</span><span class="sxs-lookup"><span data-stu-id="793fc-111">0</span></span>|<span data-ttu-id="793fc-112">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="793fc-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="793fc-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="793fc-113">allBlocked</span></span>|<span data-ttu-id="793fc-114">1</span><span class="sxs-lookup"><span data-stu-id="793fc-114">1</span></span>|<span data-ttu-id="793fc-115">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="793fc-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="793fc-116">常规</span><span class="sxs-lookup"><span data-stu-id="793fc-116">general</span></span>|<span data-ttu-id="793fc-117">2</span><span class="sxs-lookup"><span data-stu-id="793fc-117">2</span></span>|<span data-ttu-id="793fc-118">适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="793fc-118">Suitable for general audience</span></span>|
|<span data-ttu-id="793fc-119">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="793fc-119">parentalGuidance</span></span>|<span data-ttu-id="793fc-120">3</span><span class="sxs-lookup"><span data-stu-id="793fc-120">3</span></span>|<span data-ttu-id="793fc-121">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="793fc-121">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="793fc-122">成熟的</span><span class="sxs-lookup"><span data-stu-id="793fc-122">mature</span></span>|<span data-ttu-id="793fc-123">4</span><span class="sxs-lookup"><span data-stu-id="793fc-123">4</span></span>|<span data-ttu-id="793fc-124">M 分类适合成熟的访问群体</span><span class="sxs-lookup"><span data-stu-id="793fc-124">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="793fc-125">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="793fc-125">agesAbove13</span></span>|<span data-ttu-id="793fc-126">5</span><span class="sxs-lookup"><span data-stu-id="793fc-126">5</span></span>|<span data-ttu-id="793fc-127">R13 分类是人员 13 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="793fc-127">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="793fc-128">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="793fc-128">agesAbove15</span></span>|<span data-ttu-id="793fc-129">6</span><span class="sxs-lookup"><span data-stu-id="793fc-129">6</span></span>|<span data-ttu-id="793fc-130">R15 分类是人员 15 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="793fc-130">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="793fc-131">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="793fc-131">agesAbove16</span></span>|<span data-ttu-id="793fc-132">7</span><span class="sxs-lookup"><span data-stu-id="793fc-132">7</span></span>|<span data-ttu-id="793fc-133">R16 分类是人员 16 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="793fc-133">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="793fc-134">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="793fc-134">agesAbove18</span></span>|<span data-ttu-id="793fc-135">8</span><span class="sxs-lookup"><span data-stu-id="793fc-135">8</span></span>|<span data-ttu-id="793fc-136">R18 分类是人员年满 18 周岁与通过限制</span><span class="sxs-lookup"><span data-stu-id="793fc-136">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="793fc-137">受限制</span><span class="sxs-lookup"><span data-stu-id="793fc-137">restricted</span></span>|<span data-ttu-id="793fc-138">9</span><span class="sxs-lookup"><span data-stu-id="793fc-138">9</span></span>|<span data-ttu-id="793fc-139">R 分类被限制为特定访问群体</span><span class="sxs-lookup"><span data-stu-id="793fc-139">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="793fc-140">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="793fc-140">agesAbove16Restricted</span></span>|<span data-ttu-id="793fc-141">10</span><span class="sxs-lookup"><span data-stu-id="793fc-141">10</span></span>|<span data-ttu-id="793fc-142">RP16 分类需要查看在由父或成人附带的 16</span><span class="sxs-lookup"><span data-stu-id="793fc-142">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|



