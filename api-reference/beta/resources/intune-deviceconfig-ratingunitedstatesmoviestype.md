---
title: ratingUnitedStatesMoviesType 枚举类型
description: 美国的电影评分标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b32de63fe5b559b76a0de0ca2471230c8f637406
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944843"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="b2a79-103">ratingUnitedStatesMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b2a79-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="b2a79-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2a79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2a79-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2a79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2a79-106">美国的电影评分标签</span><span class="sxs-lookup"><span data-stu-id="b2a79-106">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="b2a79-107">成员</span><span class="sxs-lookup"><span data-stu-id="b2a79-107">Members</span></span>
|<span data-ttu-id="b2a79-108">成员</span><span class="sxs-lookup"><span data-stu-id="b2a79-108">Member</span></span>|<span data-ttu-id="b2a79-109">值</span><span class="sxs-lookup"><span data-stu-id="b2a79-109">Value</span></span>|<span data-ttu-id="b2a79-110">说明</span><span class="sxs-lookup"><span data-stu-id="b2a79-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2a79-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="b2a79-111">allAllowed</span></span>|<span data-ttu-id="b2a79-112">0</span><span class="sxs-lookup"><span data-stu-id="b2a79-112">0</span></span>|<span data-ttu-id="b2a79-113">默认值, 允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="b2a79-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="b2a79-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="b2a79-114">allBlocked</span></span>|<span data-ttu-id="b2a79-115">1</span><span class="sxs-lookup"><span data-stu-id="b2a79-115">1</span></span>|<span data-ttu-id="b2a79-116">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="b2a79-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="b2a79-117">概要</span><span class="sxs-lookup"><span data-stu-id="b2a79-117">general</span></span>|<span data-ttu-id="b2a79-118">双面</span><span class="sxs-lookup"><span data-stu-id="b2a79-118">2</span></span>|<span data-ttu-id="b2a79-119">G, 许可的所有年龄段</span><span class="sxs-lookup"><span data-stu-id="b2a79-119">G, all ages admitted</span></span>|
|<span data-ttu-id="b2a79-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="b2a79-120">parentalGuidance</span></span>|<span data-ttu-id="b2a79-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b2a79-121">3</span></span>|<span data-ttu-id="b2a79-122">PG, 某些材料可能不适用于儿童</span><span class="sxs-lookup"><span data-stu-id="b2a79-122">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="b2a79-123">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="b2a79-123">parentalGuidance13</span></span>|<span data-ttu-id="b2a79-124">4</span><span class="sxs-lookup"><span data-stu-id="b2a79-124">4</span></span>|<span data-ttu-id="b2a79-125">PG13, 某些材料可能不适用于13岁以下的儿童</span><span class="sxs-lookup"><span data-stu-id="b2a79-125">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="b2a79-126">受限</span><span class="sxs-lookup"><span data-stu-id="b2a79-126">restricted</span></span>|<span data-ttu-id="b2a79-127">5</span><span class="sxs-lookup"><span data-stu-id="b2a79-127">5</span></span>|<span data-ttu-id="b2a79-128">R, 17 下的查看者需要伴随父或成人监护人</span><span class="sxs-lookup"><span data-stu-id="b2a79-128">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="b2a79-129">成人</span><span class="sxs-lookup"><span data-stu-id="b2a79-129">adults</span></span>|<span data-ttu-id="b2a79-130">型</span><span class="sxs-lookup"><span data-stu-id="b2a79-130">6</span></span>|<span data-ttu-id="b2a79-131">NC17, 仅成人</span><span class="sxs-lookup"><span data-stu-id="b2a79-131">NC17, adults only</span></span>|




