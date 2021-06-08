---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国的电视内容分级标签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e8a6d05199879cc1037561081ac9ada110114d5b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759978"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="39ae6-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="39ae6-103">ratingUnitedStatesTelevisionType enum type</span></span>

<span data-ttu-id="39ae6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39ae6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39ae6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39ae6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39ae6-106">美国的电视内容分级标签</span><span class="sxs-lookup"><span data-stu-id="39ae6-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="39ae6-107">成员</span><span class="sxs-lookup"><span data-stu-id="39ae6-107">Members</span></span>
|<span data-ttu-id="39ae6-108">成员</span><span class="sxs-lookup"><span data-stu-id="39ae6-108">Member</span></span>|<span data-ttu-id="39ae6-109">值</span><span class="sxs-lookup"><span data-stu-id="39ae6-109">Value</span></span>|<span data-ttu-id="39ae6-110">说明</span><span class="sxs-lookup"><span data-stu-id="39ae6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ae6-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="39ae6-111">allAllowed</span></span>|<span data-ttu-id="39ae6-112">0</span><span class="sxs-lookup"><span data-stu-id="39ae6-112">0</span></span>|<span data-ttu-id="39ae6-113">默认值，允许所有电视显示内容</span><span class="sxs-lookup"><span data-stu-id="39ae6-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="39ae6-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="39ae6-114">allBlocked</span></span>|<span data-ttu-id="39ae6-115">1</span><span class="sxs-lookup"><span data-stu-id="39ae6-115">1</span></span>|<span data-ttu-id="39ae6-116">不允许任何电视展示内容</span><span class="sxs-lookup"><span data-stu-id="39ae6-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="39ae6-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="39ae6-117">childrenAll</span></span>|<span data-ttu-id="39ae6-118">2</span><span class="sxs-lookup"><span data-stu-id="39ae6-118">2</span></span>|<span data-ttu-id="39ae6-119">TV-Y，所有子级</span><span class="sxs-lookup"><span data-stu-id="39ae6-119">TV-Y, all children</span></span>|
|<span data-ttu-id="39ae6-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="39ae6-120">childrenAbove7</span></span>|<span data-ttu-id="39ae6-121">3</span><span class="sxs-lookup"><span data-stu-id="39ae6-121">3</span></span>|<span data-ttu-id="39ae6-122">TV-Y7，7 岁以下的儿童及以上</span><span class="sxs-lookup"><span data-stu-id="39ae6-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="39ae6-123">general</span><span class="sxs-lookup"><span data-stu-id="39ae6-123">general</span></span>|<span data-ttu-id="39ae6-124">4 </span><span class="sxs-lookup"><span data-stu-id="39ae6-124">4</span></span>|<span data-ttu-id="39ae6-125">TV-G，适合所有年龄</span><span class="sxs-lookup"><span data-stu-id="39ae6-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="39ae6-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="39ae6-126">parentalGuidance</span></span>|<span data-ttu-id="39ae6-127">5 </span><span class="sxs-lookup"><span data-stu-id="39ae6-127">5</span></span>|<span data-ttu-id="39ae6-128">TV-PG， 家长指南</span><span class="sxs-lookup"><span data-stu-id="39ae6-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="39ae6-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="39ae6-129">childrenAbove14</span></span>|<span data-ttu-id="39ae6-130">6 </span><span class="sxs-lookup"><span data-stu-id="39ae6-130">6</span></span>|<span data-ttu-id="39ae6-131">TV-14，14 岁以下的儿童及以上</span><span class="sxs-lookup"><span data-stu-id="39ae6-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="39ae6-132">一些</span><span class="sxs-lookup"><span data-stu-id="39ae6-132">adults</span></span>|<span data-ttu-id="39ae6-133">7 </span><span class="sxs-lookup"><span data-stu-id="39ae6-133">7</span></span>|<span data-ttu-id="39ae6-134">TV-MA，仅限成人</span><span class="sxs-lookup"><span data-stu-id="39ae6-134">TV-MA, adults only</span></span>|




