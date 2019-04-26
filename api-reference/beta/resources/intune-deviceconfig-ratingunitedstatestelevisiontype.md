---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国的电视内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e280ad851e9d53b8c1dc2d000419d8aaa2d9c6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555218"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="7f1bd-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7f1bd-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="7f1bd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f1bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f1bd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f1bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f1bd-106">美国的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="7f1bd-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="7f1bd-107">成员</span><span class="sxs-lookup"><span data-stu-id="7f1bd-107">Members</span></span>
|<span data-ttu-id="7f1bd-108">成员</span><span class="sxs-lookup"><span data-stu-id="7f1bd-108">Member</span></span>|<span data-ttu-id="7f1bd-109">值</span><span class="sxs-lookup"><span data-stu-id="7f1bd-109">Value</span></span>|<span data-ttu-id="7f1bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="7f1bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f1bd-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="7f1bd-111">allAllowed</span></span>|<span data-ttu-id="7f1bd-112">0</span><span class="sxs-lookup"><span data-stu-id="7f1bd-112">0</span></span>|<span data-ttu-id="7f1bd-113">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="7f1bd-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="7f1bd-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="7f1bd-114">allBlocked</span></span>|<span data-ttu-id="7f1bd-115">1</span><span class="sxs-lookup"><span data-stu-id="7f1bd-115">1</span></span>|<span data-ttu-id="7f1bd-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="7f1bd-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="7f1bd-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="7f1bd-117">childrenAll</span></span>|<span data-ttu-id="7f1bd-118">2 </span><span class="sxs-lookup"><span data-stu-id="7f1bd-118">2</span></span>|<span data-ttu-id="7f1bd-119">TV-Y, 所有子项</span><span class="sxs-lookup"><span data-stu-id="7f1bd-119">TV-Y, all children</span></span>|
|<span data-ttu-id="7f1bd-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="7f1bd-120">childrenAbove7</span></span>|<span data-ttu-id="7f1bd-121">3 </span><span class="sxs-lookup"><span data-stu-id="7f1bd-121">3</span></span>|<span data-ttu-id="7f1bd-122">电视-Y7, 儿童年龄7及更高版本</span><span class="sxs-lookup"><span data-stu-id="7f1bd-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="7f1bd-123">概要</span><span class="sxs-lookup"><span data-stu-id="7f1bd-123">general</span></span>|<span data-ttu-id="7f1bd-124">4 </span><span class="sxs-lookup"><span data-stu-id="7f1bd-124">4</span></span>|<span data-ttu-id="7f1bd-125">TV-G, 适用于所有年龄</span><span class="sxs-lookup"><span data-stu-id="7f1bd-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="7f1bd-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="7f1bd-126">parentalGuidance</span></span>|<span data-ttu-id="7f1bd-127">5 </span><span class="sxs-lookup"><span data-stu-id="7f1bd-127">5</span></span>|<span data-ttu-id="7f1bd-128">TV PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="7f1bd-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="7f1bd-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="7f1bd-129">childrenAbove14</span></span>|<span data-ttu-id="7f1bd-130">6 </span><span class="sxs-lookup"><span data-stu-id="7f1bd-130">6</span></span>|<span data-ttu-id="7f1bd-131">电视-14, 儿童年龄14及更高版本</span><span class="sxs-lookup"><span data-stu-id="7f1bd-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="7f1bd-132">成人</span><span class="sxs-lookup"><span data-stu-id="7f1bd-132">adults</span></span>|<span data-ttu-id="7f1bd-133">7 </span><span class="sxs-lookup"><span data-stu-id="7f1bd-133">7</span></span>|<span data-ttu-id="7f1bd-134">仅限成人的电视-MA</span><span class="sxs-lookup"><span data-stu-id="7f1bd-134">TV-MA, adults only</span></span>|





