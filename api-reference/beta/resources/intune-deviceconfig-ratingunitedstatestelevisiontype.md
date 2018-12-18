---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国 TV 内容评级标签
author: tfitzmac
ms.openlocfilehash: 40066b365a6b4d1dc2fb86be6d7940328a977faa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360835"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="88f9f-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="88f9f-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="88f9f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88f9f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88f9f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88f9f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88f9f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="88f9f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88f9f-107">美国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="88f9f-107">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="88f9f-108">成员</span><span class="sxs-lookup"><span data-stu-id="88f9f-108">Members</span></span>
|<span data-ttu-id="88f9f-109">成员</span><span class="sxs-lookup"><span data-stu-id="88f9f-109">Member</span></span>|<span data-ttu-id="88f9f-110">值</span><span class="sxs-lookup"><span data-stu-id="88f9f-110">Value</span></span>|<span data-ttu-id="88f9f-111">说明</span><span class="sxs-lookup"><span data-stu-id="88f9f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88f9f-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="88f9f-112">allAllowed</span></span>|<span data-ttu-id="88f9f-113">0</span><span class="sxs-lookup"><span data-stu-id="88f9f-113">0</span></span>|<span data-ttu-id="88f9f-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="88f9f-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="88f9f-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="88f9f-115">allBlocked</span></span>|<span data-ttu-id="88f9f-116">1</span><span class="sxs-lookup"><span data-stu-id="88f9f-116">1</span></span>|<span data-ttu-id="88f9f-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="88f9f-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="88f9f-118">childrenAll</span><span class="sxs-lookup"><span data-stu-id="88f9f-118">childrenAll</span></span>|<span data-ttu-id="88f9f-119">2</span><span class="sxs-lookup"><span data-stu-id="88f9f-119">2</span></span>|<span data-ttu-id="88f9f-120">TV-Y，所有子级</span><span class="sxs-lookup"><span data-stu-id="88f9f-120">TV-Y, all children</span></span>|
|<span data-ttu-id="88f9f-121">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="88f9f-121">childrenAbove7</span></span>|<span data-ttu-id="88f9f-122">3</span><span class="sxs-lookup"><span data-stu-id="88f9f-122">3</span></span>|<span data-ttu-id="88f9f-123">TV-Y7 子级 age 7 及以上</span><span class="sxs-lookup"><span data-stu-id="88f9f-123">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="88f9f-124">常规</span><span class="sxs-lookup"><span data-stu-id="88f9f-124">general</span></span>|<span data-ttu-id="88f9f-125">4</span><span class="sxs-lookup"><span data-stu-id="88f9f-125">4</span></span>|<span data-ttu-id="88f9f-126">TV G，适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="88f9f-126">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="88f9f-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="88f9f-127">parentalGuidance</span></span>|<span data-ttu-id="88f9f-128">5</span><span class="sxs-lookup"><span data-stu-id="88f9f-128">5</span></span>|<span data-ttu-id="88f9f-129">TV PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="88f9f-129">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="88f9f-130">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="88f9f-130">childrenAbove14</span></span>|<span data-ttu-id="88f9f-131">6</span><span class="sxs-lookup"><span data-stu-id="88f9f-131">6</span></span>|<span data-ttu-id="88f9f-132">TV-14 子级 age 14 及以上</span><span class="sxs-lookup"><span data-stu-id="88f9f-132">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="88f9f-133">成人</span><span class="sxs-lookup"><span data-stu-id="88f9f-133">adults</span></span>|<span data-ttu-id="88f9f-134">7</span><span class="sxs-lookup"><span data-stu-id="88f9f-134">7</span></span>|<span data-ttu-id="88f9f-135">TV MA，仅成人</span><span class="sxs-lookup"><span data-stu-id="88f9f-135">TV-MA, adults only</span></span>|





