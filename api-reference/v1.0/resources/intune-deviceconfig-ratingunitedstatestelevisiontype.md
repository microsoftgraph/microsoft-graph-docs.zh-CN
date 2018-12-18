---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国 TV 内容评级标签
author: tfitzmac
ms.openlocfilehash: 2b03a053851248bcd1238b2464c2a4f8879a5580
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328383"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="846c7-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="846c7-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="846c7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="846c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="846c7-105">美国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="846c7-105">TV content rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="846c7-106">成员</span><span class="sxs-lookup"><span data-stu-id="846c7-106">Members</span></span>
|<span data-ttu-id="846c7-107">成员</span><span class="sxs-lookup"><span data-stu-id="846c7-107">Member</span></span>|<span data-ttu-id="846c7-108">值</span><span class="sxs-lookup"><span data-stu-id="846c7-108">Value</span></span>|<span data-ttu-id="846c7-109">说明</span><span class="sxs-lookup"><span data-stu-id="846c7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="846c7-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="846c7-110">allAllowed</span></span>|<span data-ttu-id="846c7-111">0</span><span class="sxs-lookup"><span data-stu-id="846c7-111">0</span></span>|<span data-ttu-id="846c7-112">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="846c7-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="846c7-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="846c7-113">allBlocked</span></span>|<span data-ttu-id="846c7-114">1</span><span class="sxs-lookup"><span data-stu-id="846c7-114">1</span></span>|<span data-ttu-id="846c7-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="846c7-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="846c7-116">childrenAll</span><span class="sxs-lookup"><span data-stu-id="846c7-116">childrenAll</span></span>|<span data-ttu-id="846c7-117">2</span><span class="sxs-lookup"><span data-stu-id="846c7-117">2</span></span>|<span data-ttu-id="846c7-118">TV-Y，所有子级</span><span class="sxs-lookup"><span data-stu-id="846c7-118">TV-Y, all children</span></span>|
|<span data-ttu-id="846c7-119">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="846c7-119">childrenAbove7</span></span>|<span data-ttu-id="846c7-120">3</span><span class="sxs-lookup"><span data-stu-id="846c7-120">3</span></span>|<span data-ttu-id="846c7-121">TV-Y7 子级 age 7 及以上</span><span class="sxs-lookup"><span data-stu-id="846c7-121">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="846c7-122">常规</span><span class="sxs-lookup"><span data-stu-id="846c7-122">general</span></span>|<span data-ttu-id="846c7-123">4</span><span class="sxs-lookup"><span data-stu-id="846c7-123">4</span></span>|<span data-ttu-id="846c7-124">TV G，适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="846c7-124">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="846c7-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="846c7-125">parentalGuidance</span></span>|<span data-ttu-id="846c7-126">5</span><span class="sxs-lookup"><span data-stu-id="846c7-126">5</span></span>|<span data-ttu-id="846c7-127">TV PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="846c7-127">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="846c7-128">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="846c7-128">childrenAbove14</span></span>|<span data-ttu-id="846c7-129">6</span><span class="sxs-lookup"><span data-stu-id="846c7-129">6</span></span>|<span data-ttu-id="846c7-130">TV-14 子级 age 14 及以上</span><span class="sxs-lookup"><span data-stu-id="846c7-130">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="846c7-131">成人</span><span class="sxs-lookup"><span data-stu-id="846c7-131">adults</span></span>|<span data-ttu-id="846c7-132">7</span><span class="sxs-lookup"><span data-stu-id="846c7-132">7</span></span>|<span data-ttu-id="846c7-133">TV MA，仅成人</span><span class="sxs-lookup"><span data-stu-id="846c7-133">TV-MA, adults only</span></span>|



