---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国 TV 内容评级标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 405aad7e63d1c323503dde0b0bd8829702a7dcaf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403355"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="c012a-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c012a-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="c012a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c012a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c012a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c012a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c012a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c012a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c012a-107">美国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="c012a-107">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="c012a-108">成员</span><span class="sxs-lookup"><span data-stu-id="c012a-108">Members</span></span>
|<span data-ttu-id="c012a-109">成员</span><span class="sxs-lookup"><span data-stu-id="c012a-109">Member</span></span>|<span data-ttu-id="c012a-110">值</span><span class="sxs-lookup"><span data-stu-id="c012a-110">Value</span></span>|<span data-ttu-id="c012a-111">说明</span><span class="sxs-lookup"><span data-stu-id="c012a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c012a-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="c012a-112">allAllowed</span></span>|<span data-ttu-id="c012a-113">0</span><span class="sxs-lookup"><span data-stu-id="c012a-113">0</span></span>|<span data-ttu-id="c012a-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="c012a-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="c012a-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="c012a-115">allBlocked</span></span>|<span data-ttu-id="c012a-116">1</span><span class="sxs-lookup"><span data-stu-id="c012a-116">1</span></span>|<span data-ttu-id="c012a-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="c012a-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="c012a-118">childrenAll</span><span class="sxs-lookup"><span data-stu-id="c012a-118">childrenAll</span></span>|<span data-ttu-id="c012a-119">2</span><span class="sxs-lookup"><span data-stu-id="c012a-119">2</span></span>|<span data-ttu-id="c012a-120">TV-Y，所有子级</span><span class="sxs-lookup"><span data-stu-id="c012a-120">TV-Y, all children</span></span>|
|<span data-ttu-id="c012a-121">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="c012a-121">childrenAbove7</span></span>|<span data-ttu-id="c012a-122">3</span><span class="sxs-lookup"><span data-stu-id="c012a-122">3</span></span>|<span data-ttu-id="c012a-123">TV-Y7 子级 age 7 及以上</span><span class="sxs-lookup"><span data-stu-id="c012a-123">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="c012a-124">常规</span><span class="sxs-lookup"><span data-stu-id="c012a-124">general</span></span>|<span data-ttu-id="c012a-125">4</span><span class="sxs-lookup"><span data-stu-id="c012a-125">4</span></span>|<span data-ttu-id="c012a-126">TV G，适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="c012a-126">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="c012a-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="c012a-127">parentalGuidance</span></span>|<span data-ttu-id="c012a-128">5</span><span class="sxs-lookup"><span data-stu-id="c012a-128">5</span></span>|<span data-ttu-id="c012a-129">TV PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="c012a-129">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="c012a-130">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="c012a-130">childrenAbove14</span></span>|<span data-ttu-id="c012a-131">6</span><span class="sxs-lookup"><span data-stu-id="c012a-131">6</span></span>|<span data-ttu-id="c012a-132">TV-14 子级 age 14 及以上</span><span class="sxs-lookup"><span data-stu-id="c012a-132">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="c012a-133">成人</span><span class="sxs-lookup"><span data-stu-id="c012a-133">adults</span></span>|<span data-ttu-id="c012a-134">7</span><span class="sxs-lookup"><span data-stu-id="c012a-134">7</span></span>|<span data-ttu-id="c012a-135">TV MA，仅成人</span><span class="sxs-lookup"><span data-stu-id="c012a-135">TV-MA, adults only</span></span>|




