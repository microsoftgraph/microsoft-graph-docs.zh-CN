---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚中的 TV 内容评级标签
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 176e1d863fd2aa94ea48a2bf8aab515228ac31ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844686"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="da641-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="da641-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="da641-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="da641-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da641-105">澳大利亚中的 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="da641-105">TV content rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="da641-106">成员</span><span class="sxs-lookup"><span data-stu-id="da641-106">Members</span></span>
|<span data-ttu-id="da641-107">成员</span><span class="sxs-lookup"><span data-stu-id="da641-107">Member</span></span>|<span data-ttu-id="da641-108">值</span><span class="sxs-lookup"><span data-stu-id="da641-108">Value</span></span>|<span data-ttu-id="da641-109">Description</span><span class="sxs-lookup"><span data-stu-id="da641-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da641-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="da641-110">allAllowed</span></span>|<span data-ttu-id="da641-111">0</span><span class="sxs-lookup"><span data-stu-id="da641-111">0</span></span>|<span data-ttu-id="da641-112">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="da641-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="da641-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="da641-113">allBlocked</span></span>|<span data-ttu-id="da641-114">1</span><span class="sxs-lookup"><span data-stu-id="da641-114">1</span></span>|<span data-ttu-id="da641-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="da641-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="da641-116">preschoolers</span><span class="sxs-lookup"><span data-stu-id="da641-116">preschoolers</span></span>|<span data-ttu-id="da641-117">2</span><span class="sxs-lookup"><span data-stu-id="da641-117">2</span></span>|<span data-ttu-id="da641-118">P 分类供 preschoolers</span><span class="sxs-lookup"><span data-stu-id="da641-118">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="da641-119">children</span><span class="sxs-lookup"><span data-stu-id="da641-119">children</span></span>|<span data-ttu-id="da641-120">3</span><span class="sxs-lookup"><span data-stu-id="da641-120">3</span></span>|<span data-ttu-id="da641-121">C 分类供子级下 14</span><span class="sxs-lookup"><span data-stu-id="da641-121">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="da641-122">常规</span><span class="sxs-lookup"><span data-stu-id="da641-122">general</span></span>|<span data-ttu-id="da641-123">4</span><span class="sxs-lookup"><span data-stu-id="da641-123">4</span></span>|<span data-ttu-id="da641-124">G 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="da641-124">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="da641-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="da641-125">parentalGuidance</span></span>|<span data-ttu-id="da641-126">5</span><span class="sxs-lookup"><span data-stu-id="da641-126">5</span></span>|<span data-ttu-id="da641-127">PG 分类建议为年轻的查看者</span><span class="sxs-lookup"><span data-stu-id="da641-127">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="da641-128">成熟的</span><span class="sxs-lookup"><span data-stu-id="da641-128">mature</span></span>|<span data-ttu-id="da641-129">6</span><span class="sxs-lookup"><span data-stu-id="da641-129">6</span></span>|<span data-ttu-id="da641-130">M 分类建议为查看者超过 15</span><span class="sxs-lookup"><span data-stu-id="da641-130">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="da641-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="da641-131">agesAbove15</span></span>|<span data-ttu-id="da641-132">7</span><span class="sxs-lookup"><span data-stu-id="da641-132">7</span></span>|<span data-ttu-id="da641-133">MA15 + 分类不适用于查看在 15</span><span class="sxs-lookup"><span data-stu-id="da641-133">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="da641-134">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="da641-134">agesAbove15AdultViolence</span></span>|<span data-ttu-id="da641-135">8</span><span class="sxs-lookup"><span data-stu-id="da641-135">8</span></span>|<span data-ttu-id="da641-136">AV15 + 分类不适合下 15，成人暴力特有的查看者</span><span class="sxs-lookup"><span data-stu-id="da641-136">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



