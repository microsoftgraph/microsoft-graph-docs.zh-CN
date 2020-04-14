---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国的电视内容评级标签
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 99311d93dd7be12b23325cb01294a257d8c759ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444951"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="ebbac-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ebbac-103">ratingUnitedStatesTelevisionType enum type</span></span>

<span data-ttu-id="ebbac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebbac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebbac-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebbac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebbac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebbac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebbac-107">美国的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="ebbac-107">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="ebbac-108">成员</span><span class="sxs-lookup"><span data-stu-id="ebbac-108">Members</span></span>
|<span data-ttu-id="ebbac-109">成员</span><span class="sxs-lookup"><span data-stu-id="ebbac-109">Member</span></span>|<span data-ttu-id="ebbac-110">值</span><span class="sxs-lookup"><span data-stu-id="ebbac-110">Value</span></span>|<span data-ttu-id="ebbac-111">说明</span><span class="sxs-lookup"><span data-stu-id="ebbac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebbac-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="ebbac-112">allAllowed</span></span>|<span data-ttu-id="ebbac-113">0</span><span class="sxs-lookup"><span data-stu-id="ebbac-113">0</span></span>|<span data-ttu-id="ebbac-114">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="ebbac-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="ebbac-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="ebbac-115">allBlocked</span></span>|<span data-ttu-id="ebbac-116">1</span><span class="sxs-lookup"><span data-stu-id="ebbac-116">1</span></span>|<span data-ttu-id="ebbac-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="ebbac-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="ebbac-118">childrenAll</span><span class="sxs-lookup"><span data-stu-id="ebbac-118">childrenAll</span></span>|<span data-ttu-id="ebbac-119">双面</span><span class="sxs-lookup"><span data-stu-id="ebbac-119">2</span></span>|<span data-ttu-id="ebbac-120">TV-Y，所有子项</span><span class="sxs-lookup"><span data-stu-id="ebbac-120">TV-Y, all children</span></span>|
|<span data-ttu-id="ebbac-121">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="ebbac-121">childrenAbove7</span></span>|<span data-ttu-id="ebbac-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ebbac-122">3</span></span>|<span data-ttu-id="ebbac-123">电视-Y7，儿童年龄7及更高版本</span><span class="sxs-lookup"><span data-stu-id="ebbac-123">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="ebbac-124">概要</span><span class="sxs-lookup"><span data-stu-id="ebbac-124">general</span></span>|<span data-ttu-id="ebbac-125">4 </span><span class="sxs-lookup"><span data-stu-id="ebbac-125">4</span></span>|<span data-ttu-id="ebbac-126">TV-G，适用于所有年龄</span><span class="sxs-lookup"><span data-stu-id="ebbac-126">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="ebbac-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="ebbac-127">parentalGuidance</span></span>|<span data-ttu-id="ebbac-128">5 </span><span class="sxs-lookup"><span data-stu-id="ebbac-128">5</span></span>|<span data-ttu-id="ebbac-129">TV PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="ebbac-129">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="ebbac-130">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="ebbac-130">childrenAbove14</span></span>|<span data-ttu-id="ebbac-131">6 </span><span class="sxs-lookup"><span data-stu-id="ebbac-131">6</span></span>|<span data-ttu-id="ebbac-132">电视-14，儿童年龄14及更高版本</span><span class="sxs-lookup"><span data-stu-id="ebbac-132">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="ebbac-133">成人</span><span class="sxs-lookup"><span data-stu-id="ebbac-133">adults</span></span>|<span data-ttu-id="ebbac-134">7 </span><span class="sxs-lookup"><span data-stu-id="ebbac-134">7</span></span>|<span data-ttu-id="ebbac-135">仅限成人的电视-MA</span><span class="sxs-lookup"><span data-stu-id="ebbac-135">TV-MA, adults only</span></span>|



