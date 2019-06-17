---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国的电视内容评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d99114d8ead877b5bd9fee58e0a52e1ad9b288e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986709"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="63e6b-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="63e6b-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="63e6b-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63e6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63e6b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63e6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e6b-106">美国的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="63e6b-106">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="63e6b-107">成员</span><span class="sxs-lookup"><span data-stu-id="63e6b-107">Members</span></span>
|<span data-ttu-id="63e6b-108">成员</span><span class="sxs-lookup"><span data-stu-id="63e6b-108">Member</span></span>|<span data-ttu-id="63e6b-109">值</span><span class="sxs-lookup"><span data-stu-id="63e6b-109">Value</span></span>|<span data-ttu-id="63e6b-110">说明</span><span class="sxs-lookup"><span data-stu-id="63e6b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63e6b-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="63e6b-111">allAllowed</span></span>|<span data-ttu-id="63e6b-112">0</span><span class="sxs-lookup"><span data-stu-id="63e6b-112">0</span></span>|<span data-ttu-id="63e6b-113">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="63e6b-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="63e6b-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="63e6b-114">allBlocked</span></span>|<span data-ttu-id="63e6b-115">1</span><span class="sxs-lookup"><span data-stu-id="63e6b-115">1</span></span>|<span data-ttu-id="63e6b-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="63e6b-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="63e6b-117">childrenAll</span><span class="sxs-lookup"><span data-stu-id="63e6b-117">childrenAll</span></span>|<span data-ttu-id="63e6b-118">双面</span><span class="sxs-lookup"><span data-stu-id="63e6b-118">2</span></span>|<span data-ttu-id="63e6b-119">TV-Y, 所有子项</span><span class="sxs-lookup"><span data-stu-id="63e6b-119">TV-Y, all children</span></span>|
|<span data-ttu-id="63e6b-120">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="63e6b-120">childrenAbove7</span></span>|<span data-ttu-id="63e6b-121">第三章</span><span class="sxs-lookup"><span data-stu-id="63e6b-121">3</span></span>|<span data-ttu-id="63e6b-122">电视-Y7, 儿童年龄7及更高版本</span><span class="sxs-lookup"><span data-stu-id="63e6b-122">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="63e6b-123">概要</span><span class="sxs-lookup"><span data-stu-id="63e6b-123">general</span></span>|<span data-ttu-id="63e6b-124">4</span><span class="sxs-lookup"><span data-stu-id="63e6b-124">4</span></span>|<span data-ttu-id="63e6b-125">TV-G, 适用于所有年龄</span><span class="sxs-lookup"><span data-stu-id="63e6b-125">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="63e6b-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="63e6b-126">parentalGuidance</span></span>|<span data-ttu-id="63e6b-127">5</span><span class="sxs-lookup"><span data-stu-id="63e6b-127">5</span></span>|<span data-ttu-id="63e6b-128">TV PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="63e6b-128">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="63e6b-129">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="63e6b-129">childrenAbove14</span></span>|<span data-ttu-id="63e6b-130">型</span><span class="sxs-lookup"><span data-stu-id="63e6b-130">6</span></span>|<span data-ttu-id="63e6b-131">电视-14, 儿童年龄14及更高版本</span><span class="sxs-lookup"><span data-stu-id="63e6b-131">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="63e6b-132">成人</span><span class="sxs-lookup"><span data-stu-id="63e6b-132">adults</span></span>|<span data-ttu-id="63e6b-133">步</span><span class="sxs-lookup"><span data-stu-id="63e6b-133">7</span></span>|<span data-ttu-id="63e6b-134">仅限成人的电视-MA</span><span class="sxs-lookup"><span data-stu-id="63e6b-134">TV-MA, adults only</span></span>|





