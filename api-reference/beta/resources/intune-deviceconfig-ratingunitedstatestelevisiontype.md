---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国的电视内容评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 00e85b175552adf08dc518307950820fab22f753
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525892"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="67fb4-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="67fb4-103">ratingUnitedStatesTelevisionType enum type</span></span>

<span data-ttu-id="67fb4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="67fb4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67fb4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="67fb4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67fb4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67fb4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67fb4-107">美国的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="67fb4-107">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="67fb4-108">成员</span><span class="sxs-lookup"><span data-stu-id="67fb4-108">Members</span></span>
|<span data-ttu-id="67fb4-109">成员</span><span class="sxs-lookup"><span data-stu-id="67fb4-109">Member</span></span>|<span data-ttu-id="67fb4-110">值</span><span class="sxs-lookup"><span data-stu-id="67fb4-110">Value</span></span>|<span data-ttu-id="67fb4-111">说明</span><span class="sxs-lookup"><span data-stu-id="67fb4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67fb4-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="67fb4-112">allAllowed</span></span>|<span data-ttu-id="67fb4-113">0</span><span class="sxs-lookup"><span data-stu-id="67fb4-113">0</span></span>|<span data-ttu-id="67fb4-114">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="67fb4-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="67fb4-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="67fb4-115">allBlocked</span></span>|<span data-ttu-id="67fb4-116">1 </span><span class="sxs-lookup"><span data-stu-id="67fb4-116">1</span></span>|<span data-ttu-id="67fb4-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="67fb4-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="67fb4-118">childrenAll</span><span class="sxs-lookup"><span data-stu-id="67fb4-118">childrenAll</span></span>|<span data-ttu-id="67fb4-119">2 </span><span class="sxs-lookup"><span data-stu-id="67fb4-119">2</span></span>|<span data-ttu-id="67fb4-120">TV-Y，所有子项</span><span class="sxs-lookup"><span data-stu-id="67fb4-120">TV-Y, all children</span></span>|
|<span data-ttu-id="67fb4-121">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="67fb4-121">childrenAbove7</span></span>|<span data-ttu-id="67fb4-122">3 </span><span class="sxs-lookup"><span data-stu-id="67fb4-122">3</span></span>|<span data-ttu-id="67fb4-123">电视-Y7，儿童年龄7及更高版本</span><span class="sxs-lookup"><span data-stu-id="67fb4-123">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="67fb4-124">概要</span><span class="sxs-lookup"><span data-stu-id="67fb4-124">general</span></span>|<span data-ttu-id="67fb4-125">4 </span><span class="sxs-lookup"><span data-stu-id="67fb4-125">4</span></span>|<span data-ttu-id="67fb4-126">TV-G，适用于所有年龄</span><span class="sxs-lookup"><span data-stu-id="67fb4-126">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="67fb4-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="67fb4-127">parentalGuidance</span></span>|<span data-ttu-id="67fb4-128">5 </span><span class="sxs-lookup"><span data-stu-id="67fb4-128">5</span></span>|<span data-ttu-id="67fb4-129">TV PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="67fb4-129">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="67fb4-130">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="67fb4-130">childrenAbove14</span></span>|<span data-ttu-id="67fb4-131">6 </span><span class="sxs-lookup"><span data-stu-id="67fb4-131">6</span></span>|<span data-ttu-id="67fb4-132">电视-14，儿童年龄14及更高版本</span><span class="sxs-lookup"><span data-stu-id="67fb4-132">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="67fb4-133">成人</span><span class="sxs-lookup"><span data-stu-id="67fb4-133">adults</span></span>|<span data-ttu-id="67fb4-134">7 </span><span class="sxs-lookup"><span data-stu-id="67fb4-134">7</span></span>|<span data-ttu-id="67fb4-135">仅限成人的电视-MA</span><span class="sxs-lookup"><span data-stu-id="67fb4-135">TV-MA, adults only</span></span>|



