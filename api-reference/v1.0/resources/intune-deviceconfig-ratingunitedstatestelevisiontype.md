---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国 TV 内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 562caf44391eabc400d0296602d7e359d683983c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969469"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="13f92-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="13f92-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="13f92-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="13f92-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13f92-105">美国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="13f92-105">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="13f92-106">成员</span><span class="sxs-lookup"><span data-stu-id="13f92-106">Members</span></span>
|<span data-ttu-id="13f92-107">成员</span><span class="sxs-lookup"><span data-stu-id="13f92-107">Member</span></span>|<span data-ttu-id="13f92-108">值</span><span class="sxs-lookup"><span data-stu-id="13f92-108">Value</span></span>|<span data-ttu-id="13f92-109">说明</span><span class="sxs-lookup"><span data-stu-id="13f92-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13f92-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="13f92-110">allAllowed</span></span>|<span data-ttu-id="13f92-111">0</span><span class="sxs-lookup"><span data-stu-id="13f92-111">0</span></span>|<span data-ttu-id="13f92-112">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="13f92-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="13f92-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="13f92-113">allBlocked</span></span>|<span data-ttu-id="13f92-114">1</span><span class="sxs-lookup"><span data-stu-id="13f92-114">1</span></span>|<span data-ttu-id="13f92-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="13f92-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="13f92-116">childrenAll</span><span class="sxs-lookup"><span data-stu-id="13f92-116">childrenAll</span></span>|<span data-ttu-id="13f92-117">2</span><span class="sxs-lookup"><span data-stu-id="13f92-117">2</span></span>|<span data-ttu-id="13f92-118">TV-Y，所有子级</span><span class="sxs-lookup"><span data-stu-id="13f92-118">TV-Y, all children</span></span>|
|<span data-ttu-id="13f92-119">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="13f92-119">childrenAbove7</span></span>|<span data-ttu-id="13f92-120">3</span><span class="sxs-lookup"><span data-stu-id="13f92-120">3</span></span>|<span data-ttu-id="13f92-121">TV-Y7 子级 age 7 及以上</span><span class="sxs-lookup"><span data-stu-id="13f92-121">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="13f92-122">常规</span><span class="sxs-lookup"><span data-stu-id="13f92-122">general</span></span>|<span data-ttu-id="13f92-123">4</span><span class="sxs-lookup"><span data-stu-id="13f92-123">4</span></span>|<span data-ttu-id="13f92-124">TV G，适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="13f92-124">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="13f92-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="13f92-125">parentalGuidance</span></span>|<span data-ttu-id="13f92-126">5</span><span class="sxs-lookup"><span data-stu-id="13f92-126">5</span></span>|<span data-ttu-id="13f92-127">TV PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="13f92-127">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="13f92-128">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="13f92-128">childrenAbove14</span></span>|<span data-ttu-id="13f92-129">6</span><span class="sxs-lookup"><span data-stu-id="13f92-129">6</span></span>|<span data-ttu-id="13f92-130">TV-14 子级 age 14 及以上</span><span class="sxs-lookup"><span data-stu-id="13f92-130">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="13f92-131">成人</span><span class="sxs-lookup"><span data-stu-id="13f92-131">adults</span></span>|<span data-ttu-id="13f92-132">7</span><span class="sxs-lookup"><span data-stu-id="13f92-132">7</span></span>|<span data-ttu-id="13f92-133">TV MA，仅成人</span><span class="sxs-lookup"><span data-stu-id="13f92-133">TV-MA, adults only</span></span>|



