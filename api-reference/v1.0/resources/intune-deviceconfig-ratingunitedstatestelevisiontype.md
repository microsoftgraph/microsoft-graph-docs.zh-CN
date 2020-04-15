---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国的电视内容评级标签
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8be03ade213b25cba4346ad1c0aa53342171003c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472704"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="00449-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="00449-103">ratingUnitedStatesTelevisionType enum type</span></span>

<span data-ttu-id="00449-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00449-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00449-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="00449-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00449-106">美国的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="00449-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="00449-107">成员</span><span class="sxs-lookup"><span data-stu-id="00449-107">Members</span></span>
|<span data-ttu-id="00449-108">成员</span><span class="sxs-lookup"><span data-stu-id="00449-108">Member</span></span>|<span data-ttu-id="00449-109">值</span><span class="sxs-lookup"><span data-stu-id="00449-109">Value</span></span>|<span data-ttu-id="00449-110">说明</span><span class="sxs-lookup"><span data-stu-id="00449-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00449-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="00449-111">allAllowed</span></span>|<span data-ttu-id="00449-112">0</span><span class="sxs-lookup"><span data-stu-id="00449-112">0</span></span>|<span data-ttu-id="00449-113">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="00449-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="00449-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="00449-114">allBlocked</span></span>|<span data-ttu-id="00449-115">1</span><span class="sxs-lookup"><span data-stu-id="00449-115">1</span></span>|<span data-ttu-id="00449-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="00449-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="00449-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="00449-117">childrenAll</span></span>|<span data-ttu-id="00449-118">双面</span><span class="sxs-lookup"><span data-stu-id="00449-118">2</span></span>|<span data-ttu-id="00449-119">TV-Y，所有子项</span><span class="sxs-lookup"><span data-stu-id="00449-119">TV-Y, all children</span></span>|
|<span data-ttu-id="00449-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="00449-120">childrenAbove7</span></span>|<span data-ttu-id="00449-121">第三章</span><span class="sxs-lookup"><span data-stu-id="00449-121">3</span></span>|<span data-ttu-id="00449-122">电视-Y7，儿童年龄7及更高版本</span><span class="sxs-lookup"><span data-stu-id="00449-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="00449-123">概要</span><span class="sxs-lookup"><span data-stu-id="00449-123">general</span></span>|<span data-ttu-id="00449-124">4 </span><span class="sxs-lookup"><span data-stu-id="00449-124">4</span></span>|<span data-ttu-id="00449-125">TV-G，适用于所有年龄</span><span class="sxs-lookup"><span data-stu-id="00449-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="00449-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="00449-126">parentalGuidance</span></span>|<span data-ttu-id="00449-127">5 </span><span class="sxs-lookup"><span data-stu-id="00449-127">5</span></span>|<span data-ttu-id="00449-128">TV PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="00449-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="00449-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="00449-129">childrenAbove14</span></span>|<span data-ttu-id="00449-130">6 </span><span class="sxs-lookup"><span data-stu-id="00449-130">6</span></span>|<span data-ttu-id="00449-131">电视-14，儿童年龄14及更高版本</span><span class="sxs-lookup"><span data-stu-id="00449-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="00449-132">成人</span><span class="sxs-lookup"><span data-stu-id="00449-132">adults</span></span>|<span data-ttu-id="00449-133">7 </span><span class="sxs-lookup"><span data-stu-id="00449-133">7</span></span>|<span data-ttu-id="00449-134">仅限成人的电视-MA</span><span class="sxs-lookup"><span data-stu-id="00449-134">TV-MA, adults only</span></span>|







