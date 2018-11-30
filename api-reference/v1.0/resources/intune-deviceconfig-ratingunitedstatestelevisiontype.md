---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国 TV 内容评级标签
ms.openlocfilehash: bb0a977294d8236205b6d6bdf6311db75e377951
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011581"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="5989e-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5989e-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="5989e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5989e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5989e-105">美国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="5989e-105">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="5989e-106">成员</span><span class="sxs-lookup"><span data-stu-id="5989e-106">Members</span></span>
|<span data-ttu-id="5989e-107">成员</span><span class="sxs-lookup"><span data-stu-id="5989e-107">Member</span></span>|<span data-ttu-id="5989e-108">值</span><span class="sxs-lookup"><span data-stu-id="5989e-108">Value</span></span>|<span data-ttu-id="5989e-109">说明</span><span class="sxs-lookup"><span data-stu-id="5989e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5989e-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="5989e-110">allAllowed</span></span>|<span data-ttu-id="5989e-111">0</span><span class="sxs-lookup"><span data-stu-id="5989e-111">0</span></span>|<span data-ttu-id="5989e-112">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="5989e-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="5989e-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="5989e-113">allBlocked</span></span>|<span data-ttu-id="5989e-114">1</span><span class="sxs-lookup"><span data-stu-id="5989e-114">1</span></span>|<span data-ttu-id="5989e-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="5989e-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="5989e-116">childrenAll</span><span class="sxs-lookup"><span data-stu-id="5989e-116">childrenAll</span></span>|<span data-ttu-id="5989e-117">2</span><span class="sxs-lookup"><span data-stu-id="5989e-117">2</span></span>|<span data-ttu-id="5989e-118">TV-Y，所有子级</span><span class="sxs-lookup"><span data-stu-id="5989e-118">TV-Y, all children</span></span>|
|<span data-ttu-id="5989e-119">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="5989e-119">childrenAbove7</span></span>|<span data-ttu-id="5989e-120">3</span><span class="sxs-lookup"><span data-stu-id="5989e-120">3</span></span>|<span data-ttu-id="5989e-121">TV-Y7 子级 age 7 及以上</span><span class="sxs-lookup"><span data-stu-id="5989e-121">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="5989e-122">常规</span><span class="sxs-lookup"><span data-stu-id="5989e-122">general</span></span>|<span data-ttu-id="5989e-123">4</span><span class="sxs-lookup"><span data-stu-id="5989e-123">4</span></span>|<span data-ttu-id="5989e-124">TV G，适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="5989e-124">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="5989e-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="5989e-125">parentalGuidance</span></span>|<span data-ttu-id="5989e-126">5</span><span class="sxs-lookup"><span data-stu-id="5989e-126">5</span></span>|<span data-ttu-id="5989e-127">TV PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="5989e-127">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="5989e-128">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="5989e-128">childrenAbove14</span></span>|<span data-ttu-id="5989e-129">6</span><span class="sxs-lookup"><span data-stu-id="5989e-129">6</span></span>|<span data-ttu-id="5989e-130">TV-14 子级 age 14 及以上</span><span class="sxs-lookup"><span data-stu-id="5989e-130">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="5989e-131">成人</span><span class="sxs-lookup"><span data-stu-id="5989e-131">adults</span></span>|<span data-ttu-id="5989e-132">7</span><span class="sxs-lookup"><span data-stu-id="5989e-132">7</span></span>|<span data-ttu-id="5989e-133">TV MA，仅成人</span><span class="sxs-lookup"><span data-stu-id="5989e-133">TV-MA, adults only</span></span>|



