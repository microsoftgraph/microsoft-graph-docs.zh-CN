---
title: ratingCanadaMoviesType 枚举类型
description: 电影分级加拿大标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5f35289348dbe94b5be3aa5a1d96709de8e8869
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398406"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="4b766-103">ratingCanadaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4b766-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="4b766-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4b766-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b766-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4b766-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b766-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b766-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b766-107">电影分级加拿大标签</span><span class="sxs-lookup"><span data-stu-id="4b766-107">Movies rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="4b766-108">成员</span><span class="sxs-lookup"><span data-stu-id="4b766-108">Members</span></span>
|<span data-ttu-id="4b766-109">成员</span><span class="sxs-lookup"><span data-stu-id="4b766-109">Member</span></span>|<span data-ttu-id="4b766-110">值</span><span class="sxs-lookup"><span data-stu-id="4b766-110">Value</span></span>|<span data-ttu-id="4b766-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b766-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b766-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="4b766-112">allAllowed</span></span>|<span data-ttu-id="4b766-113">0</span><span class="sxs-lookup"><span data-stu-id="4b766-113">0</span></span>|<span data-ttu-id="4b766-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="4b766-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="4b766-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="4b766-115">allBlocked</span></span>|<span data-ttu-id="4b766-116">1</span><span class="sxs-lookup"><span data-stu-id="4b766-116">1</span></span>|<span data-ttu-id="4b766-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="4b766-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="4b766-118">常规</span><span class="sxs-lookup"><span data-stu-id="4b766-118">general</span></span>|<span data-ttu-id="4b766-119">2</span><span class="sxs-lookup"><span data-stu-id="4b766-119">2</span></span>|<span data-ttu-id="4b766-120">G 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="4b766-120">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="4b766-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="4b766-121">parentalGuidance</span></span>|<span data-ttu-id="4b766-122">3</span><span class="sxs-lookup"><span data-stu-id="4b766-122">3</span></span>|<span data-ttu-id="4b766-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="4b766-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="4b766-124">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="4b766-124">agesAbove14</span></span>|<span data-ttu-id="4b766-125">4</span><span class="sxs-lookup"><span data-stu-id="4b766-125">4</span></span>|<span data-ttu-id="4b766-126">14A 分类适于上面 14 或更低的查看者</span><span class="sxs-lookup"><span data-stu-id="4b766-126">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="4b766-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="4b766-127">agesAbove18</span></span>|<span data-ttu-id="4b766-128">5</span><span class="sxs-lookup"><span data-stu-id="4b766-128">5</span></span>|<span data-ttu-id="4b766-129">18A 分类适于上面 18 或更低的查看者</span><span class="sxs-lookup"><span data-stu-id="4b766-129">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="4b766-130">受限制</span><span class="sxs-lookup"><span data-stu-id="4b766-130">restricted</span></span>|<span data-ttu-id="4b766-131">6</span><span class="sxs-lookup"><span data-stu-id="4b766-131">6</span></span>|<span data-ttu-id="4b766-132">R 分类是限制为 18 年及较早</span><span class="sxs-lookup"><span data-stu-id="4b766-132">The R classification is restricted to 18 years and older</span></span>|




