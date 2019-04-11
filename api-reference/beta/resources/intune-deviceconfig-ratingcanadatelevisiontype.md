---
title: ratingCanadaTelevisionType 枚举类型
description: 加拿大的电视内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fa3989f4fe1324f404a16603f357a81136e1d9e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806970"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="bed49-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bed49-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="bed49-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bed49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bed49-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bed49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bed49-106">加拿大的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="bed49-106">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="bed49-107">成员</span><span class="sxs-lookup"><span data-stu-id="bed49-107">Members</span></span>
|<span data-ttu-id="bed49-108">成员</span><span class="sxs-lookup"><span data-stu-id="bed49-108">Member</span></span>|<span data-ttu-id="bed49-109">值</span><span class="sxs-lookup"><span data-stu-id="bed49-109">Value</span></span>|<span data-ttu-id="bed49-110">说明</span><span class="sxs-lookup"><span data-stu-id="bed49-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bed49-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="bed49-111">allAllowed</span></span>|<span data-ttu-id="bed49-112">0</span><span class="sxs-lookup"><span data-stu-id="bed49-112">0</span></span>|<span data-ttu-id="bed49-113">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="bed49-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="bed49-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="bed49-114">allBlocked</span></span>|<span data-ttu-id="bed49-115">1</span><span class="sxs-lookup"><span data-stu-id="bed49-115">1</span></span>|<span data-ttu-id="bed49-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="bed49-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="bed49-117">children</span><span class="sxs-lookup"><span data-stu-id="bed49-117">children</span></span>|<span data-ttu-id="bed49-118">双面</span><span class="sxs-lookup"><span data-stu-id="bed49-118">2</span></span>|<span data-ttu-id="bed49-119">C 分类适用于2到7年的儿童年龄</span><span class="sxs-lookup"><span data-stu-id="bed49-119">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="bed49-120">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="bed49-120">childrenAbove8</span></span>|<span data-ttu-id="bed49-121">第三章</span><span class="sxs-lookup"><span data-stu-id="bed49-121">3</span></span>|<span data-ttu-id="bed49-122">C8 分类适用于仅有8岁以上的儿童</span><span class="sxs-lookup"><span data-stu-id="bed49-122">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="bed49-123">概要</span><span class="sxs-lookup"><span data-stu-id="bed49-123">general</span></span>|<span data-ttu-id="bed49-124">4</span><span class="sxs-lookup"><span data-stu-id="bed49-124">4</span></span>|<span data-ttu-id="bed49-125">G 分类适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="bed49-125">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="bed49-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="bed49-126">parentalGuidance</span></span>|<span data-ttu-id="bed49-127">5</span><span class="sxs-lookup"><span data-stu-id="bed49-127">5</span></span>|<span data-ttu-id="bed49-128">PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="bed49-128">PG, Parental Guidance</span></span>|
|<span data-ttu-id="bed49-129">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="bed49-129">agesAbove14</span></span>|<span data-ttu-id="bed49-130">型</span><span class="sxs-lookup"><span data-stu-id="bed49-130">6</span></span>|<span data-ttu-id="bed49-131">14 + 分类适用于14岁及更早的查看者</span><span class="sxs-lookup"><span data-stu-id="bed49-131">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="bed49-132">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="bed49-132">agesAbove18</span></span>|<span data-ttu-id="bed49-133">步</span><span class="sxs-lookup"><span data-stu-id="bed49-133">7</span></span>|<span data-ttu-id="bed49-134">18个以上的分类适用于18岁及更早的查看者</span><span class="sxs-lookup"><span data-stu-id="bed49-134">The 18+ classification is intended for viewers ages 18 and older</span></span>|





