---
title: ratingCanadaTelevisionType 枚举类型
description: 加拿大的电视内容评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7c8fe4c99a6201bd17913f19a3594d3f138a44a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995754"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="81a46-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="81a46-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="81a46-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81a46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81a46-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81a46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a46-106">加拿大的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="81a46-106">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="81a46-107">成员</span><span class="sxs-lookup"><span data-stu-id="81a46-107">Members</span></span>
|<span data-ttu-id="81a46-108">成员</span><span class="sxs-lookup"><span data-stu-id="81a46-108">Member</span></span>|<span data-ttu-id="81a46-109">值</span><span class="sxs-lookup"><span data-stu-id="81a46-109">Value</span></span>|<span data-ttu-id="81a46-110">说明</span><span class="sxs-lookup"><span data-stu-id="81a46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a46-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="81a46-111">allAllowed</span></span>|<span data-ttu-id="81a46-112">0</span><span class="sxs-lookup"><span data-stu-id="81a46-112">0</span></span>|<span data-ttu-id="81a46-113">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="81a46-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="81a46-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="81a46-114">allBlocked</span></span>|<span data-ttu-id="81a46-115">1</span><span class="sxs-lookup"><span data-stu-id="81a46-115">1</span></span>|<span data-ttu-id="81a46-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="81a46-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="81a46-117">children</span><span class="sxs-lookup"><span data-stu-id="81a46-117">children</span></span>|<span data-ttu-id="81a46-118">双面</span><span class="sxs-lookup"><span data-stu-id="81a46-118">2</span></span>|<span data-ttu-id="81a46-119">C 分类适用于2到7年的儿童年龄</span><span class="sxs-lookup"><span data-stu-id="81a46-119">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="81a46-120">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="81a46-120">childrenAbove8</span></span>|<span data-ttu-id="81a46-121">第三章</span><span class="sxs-lookup"><span data-stu-id="81a46-121">3</span></span>|<span data-ttu-id="81a46-122">C8 分类适用于仅有8岁以上的儿童</span><span class="sxs-lookup"><span data-stu-id="81a46-122">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="81a46-123">概要</span><span class="sxs-lookup"><span data-stu-id="81a46-123">general</span></span>|<span data-ttu-id="81a46-124">4</span><span class="sxs-lookup"><span data-stu-id="81a46-124">4</span></span>|<span data-ttu-id="81a46-125">G 分类适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="81a46-125">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="81a46-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="81a46-126">parentalGuidance</span></span>|<span data-ttu-id="81a46-127">5</span><span class="sxs-lookup"><span data-stu-id="81a46-127">5</span></span>|<span data-ttu-id="81a46-128">PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="81a46-128">PG, Parental Guidance</span></span>|
|<span data-ttu-id="81a46-129">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="81a46-129">agesAbove14</span></span>|<span data-ttu-id="81a46-130">型</span><span class="sxs-lookup"><span data-stu-id="81a46-130">6</span></span>|<span data-ttu-id="81a46-131">14 + 分类适用于14岁及更早的查看者</span><span class="sxs-lookup"><span data-stu-id="81a46-131">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="81a46-132">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="81a46-132">agesAbove18</span></span>|<span data-ttu-id="81a46-133">步</span><span class="sxs-lookup"><span data-stu-id="81a46-133">7</span></span>|<span data-ttu-id="81a46-134">18个以上的分类适用于18岁及更早的查看者</span><span class="sxs-lookup"><span data-stu-id="81a46-134">The 18+ classification is intended for viewers ages 18 and older</span></span>|





