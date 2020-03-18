---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国的电视内容评级标签
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8503ff7db3ff7e1b3d4ba742e694032632054ae1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787633"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="f1430-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f1430-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="f1430-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1430-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1430-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1430-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1430-106">美国的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="f1430-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="f1430-107">成员</span><span class="sxs-lookup"><span data-stu-id="f1430-107">Members</span></span>
|<span data-ttu-id="f1430-108">成员</span><span class="sxs-lookup"><span data-stu-id="f1430-108">Member</span></span>|<span data-ttu-id="f1430-109">值</span><span class="sxs-lookup"><span data-stu-id="f1430-109">Value</span></span>|<span data-ttu-id="f1430-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1430-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1430-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f1430-111">allAllowed</span></span>|<span data-ttu-id="f1430-112">0</span><span class="sxs-lookup"><span data-stu-id="f1430-112">0</span></span>|<span data-ttu-id="f1430-113">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="f1430-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="f1430-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f1430-114">allBlocked</span></span>|<span data-ttu-id="f1430-115">1</span><span class="sxs-lookup"><span data-stu-id="f1430-115">1</span></span>|<span data-ttu-id="f1430-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="f1430-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="f1430-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="f1430-117">childrenAll</span></span>|<span data-ttu-id="f1430-118">双面</span><span class="sxs-lookup"><span data-stu-id="f1430-118">2</span></span>|<span data-ttu-id="f1430-119">TV-Y，所有子项</span><span class="sxs-lookup"><span data-stu-id="f1430-119">TV-Y, all children</span></span>|
|<span data-ttu-id="f1430-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="f1430-120">childrenAbove7</span></span>|<span data-ttu-id="f1430-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f1430-121">3</span></span>|<span data-ttu-id="f1430-122">电视-Y7，儿童年龄7及更高版本</span><span class="sxs-lookup"><span data-stu-id="f1430-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="f1430-123">概要</span><span class="sxs-lookup"><span data-stu-id="f1430-123">general</span></span>|<span data-ttu-id="f1430-124">4 </span><span class="sxs-lookup"><span data-stu-id="f1430-124">4</span></span>|<span data-ttu-id="f1430-125">TV-G，适用于所有年龄</span><span class="sxs-lookup"><span data-stu-id="f1430-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="f1430-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="f1430-126">parentalGuidance</span></span>|<span data-ttu-id="f1430-127">5 </span><span class="sxs-lookup"><span data-stu-id="f1430-127">5</span></span>|<span data-ttu-id="f1430-128">TV PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="f1430-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="f1430-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="f1430-129">childrenAbove14</span></span>|<span data-ttu-id="f1430-130">6 </span><span class="sxs-lookup"><span data-stu-id="f1430-130">6</span></span>|<span data-ttu-id="f1430-131">电视-14，儿童年龄14及更高版本</span><span class="sxs-lookup"><span data-stu-id="f1430-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="f1430-132">成人</span><span class="sxs-lookup"><span data-stu-id="f1430-132">adults</span></span>|<span data-ttu-id="f1430-133">7 </span><span class="sxs-lookup"><span data-stu-id="f1430-133">7</span></span>|<span data-ttu-id="f1430-134">仅限成人的电视-MA</span><span class="sxs-lookup"><span data-stu-id="f1430-134">TV-MA, adults only</span></span>|



