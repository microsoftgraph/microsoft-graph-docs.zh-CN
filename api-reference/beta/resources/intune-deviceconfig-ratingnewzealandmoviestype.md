---
title: ratingNewZealandMoviesType 枚举类型
description: 电影分级新西兰标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b60bb2d443763115bb547c254ab086b171033658
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402942"
---
# <a name="ratingnewzealandmoviestype-enum-type"></a><span data-ttu-id="4b030-103">ratingNewZealandMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4b030-103">ratingNewZealandMoviesType enum type</span></span>

> <span data-ttu-id="4b030-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4b030-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b030-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4b030-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b030-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b030-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b030-107">电影分级新西兰标签</span><span class="sxs-lookup"><span data-stu-id="4b030-107">Movies rating labels in New Zealand</span></span>

## <a name="members"></a><span data-ttu-id="4b030-108">成员</span><span class="sxs-lookup"><span data-stu-id="4b030-108">Members</span></span>
|<span data-ttu-id="4b030-109">成员</span><span class="sxs-lookup"><span data-stu-id="4b030-109">Member</span></span>|<span data-ttu-id="4b030-110">值</span><span class="sxs-lookup"><span data-stu-id="4b030-110">Value</span></span>|<span data-ttu-id="4b030-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b030-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b030-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="4b030-112">allAllowed</span></span>|<span data-ttu-id="4b030-113">0</span><span class="sxs-lookup"><span data-stu-id="4b030-113">0</span></span>|<span data-ttu-id="4b030-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="4b030-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="4b030-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="4b030-115">allBlocked</span></span>|<span data-ttu-id="4b030-116">1</span><span class="sxs-lookup"><span data-stu-id="4b030-116">1</span></span>|<span data-ttu-id="4b030-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="4b030-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="4b030-118">常规</span><span class="sxs-lookup"><span data-stu-id="4b030-118">general</span></span>|<span data-ttu-id="4b030-119">2</span><span class="sxs-lookup"><span data-stu-id="4b030-119">2</span></span>|<span data-ttu-id="4b030-120">适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="4b030-120">Suitable for general audience</span></span>|
|<span data-ttu-id="4b030-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="4b030-121">parentalGuidance</span></span>|<span data-ttu-id="4b030-122">3</span><span class="sxs-lookup"><span data-stu-id="4b030-122">3</span></span>|<span data-ttu-id="4b030-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="4b030-123">The PG classification recommends parental guidance</span></span>|
|<span data-ttu-id="4b030-124">成熟的</span><span class="sxs-lookup"><span data-stu-id="4b030-124">mature</span></span>|<span data-ttu-id="4b030-125">4</span><span class="sxs-lookup"><span data-stu-id="4b030-125">4</span></span>|<span data-ttu-id="4b030-126">M 分类适合成熟的访问群体</span><span class="sxs-lookup"><span data-stu-id="4b030-126">The M classification is suitable for mature audience</span></span>|
|<span data-ttu-id="4b030-127">agesAbove13</span><span class="sxs-lookup"><span data-stu-id="4b030-127">agesAbove13</span></span>|<span data-ttu-id="4b030-128">5</span><span class="sxs-lookup"><span data-stu-id="4b030-128">5</span></span>|<span data-ttu-id="4b030-129">R13 分类是人员 13 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="4b030-129">The R13 classification is restricted to persons 13 years and over</span></span>|
|<span data-ttu-id="4b030-130">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="4b030-130">agesAbove15</span></span>|<span data-ttu-id="4b030-131">6</span><span class="sxs-lookup"><span data-stu-id="4b030-131">6</span></span>|<span data-ttu-id="4b030-132">R15 分类是人员 15 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="4b030-132">The R15 classification is restricted to persons 15 years and over</span></span>|
|<span data-ttu-id="4b030-133">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="4b030-133">agesAbove16</span></span>|<span data-ttu-id="4b030-134">7</span><span class="sxs-lookup"><span data-stu-id="4b030-134">7</span></span>|<span data-ttu-id="4b030-135">R16 分类是人员 16 年和通过限制</span><span class="sxs-lookup"><span data-stu-id="4b030-135">The R16 classification is restricted to persons 16 years and over</span></span>|
|<span data-ttu-id="4b030-136">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="4b030-136">agesAbove18</span></span>|<span data-ttu-id="4b030-137">8</span><span class="sxs-lookup"><span data-stu-id="4b030-137">8</span></span>|<span data-ttu-id="4b030-138">R18 分类是人员年满 18 周岁与通过限制</span><span class="sxs-lookup"><span data-stu-id="4b030-138">The R18 classification is restricted to persons 18 years and over</span></span>|
|<span data-ttu-id="4b030-139">受限制</span><span class="sxs-lookup"><span data-stu-id="4b030-139">restricted</span></span>|<span data-ttu-id="4b030-140">9</span><span class="sxs-lookup"><span data-stu-id="4b030-140">9</span></span>|<span data-ttu-id="4b030-141">R 分类被限制为特定访问群体</span><span class="sxs-lookup"><span data-stu-id="4b030-141">The R classification is restricted to a certain audience</span></span>|
|<span data-ttu-id="4b030-142">agesAbove16Restricted</span><span class="sxs-lookup"><span data-stu-id="4b030-142">agesAbove16Restricted</span></span>|<span data-ttu-id="4b030-143">10</span><span class="sxs-lookup"><span data-stu-id="4b030-143">10</span></span>|<span data-ttu-id="4b030-144">RP16 分类需要查看在由父或成人附带的 16</span><span class="sxs-lookup"><span data-stu-id="4b030-144">The RP16 classification requires viewers under 16 accompanied by a parent or an adult</span></span>|




