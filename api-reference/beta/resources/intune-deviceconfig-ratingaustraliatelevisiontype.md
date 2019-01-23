---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚中的 TV 内容评级标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 148e8c1bb12f8563261402b98e4ff0552e83f3f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392890"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="09c37-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="09c37-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="09c37-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="09c37-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="09c37-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="09c37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09c37-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09c37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09c37-107">澳大利亚中的 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="09c37-107">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="09c37-108">成员</span><span class="sxs-lookup"><span data-stu-id="09c37-108">Members</span></span>
|<span data-ttu-id="09c37-109">成员</span><span class="sxs-lookup"><span data-stu-id="09c37-109">Member</span></span>|<span data-ttu-id="09c37-110">值</span><span class="sxs-lookup"><span data-stu-id="09c37-110">Value</span></span>|<span data-ttu-id="09c37-111">说明</span><span class="sxs-lookup"><span data-stu-id="09c37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09c37-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="09c37-112">allAllowed</span></span>|<span data-ttu-id="09c37-113">0</span><span class="sxs-lookup"><span data-stu-id="09c37-113">0</span></span>|<span data-ttu-id="09c37-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="09c37-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="09c37-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="09c37-115">allBlocked</span></span>|<span data-ttu-id="09c37-116">1</span><span class="sxs-lookup"><span data-stu-id="09c37-116">1</span></span>|<span data-ttu-id="09c37-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="09c37-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="09c37-118">preschoolers</span><span class="sxs-lookup"><span data-stu-id="09c37-118">preschoolers</span></span>|<span data-ttu-id="09c37-119">2</span><span class="sxs-lookup"><span data-stu-id="09c37-119">2</span></span>|<span data-ttu-id="09c37-120">P 分类供 preschoolers</span><span class="sxs-lookup"><span data-stu-id="09c37-120">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="09c37-121">children</span><span class="sxs-lookup"><span data-stu-id="09c37-121">children</span></span>|<span data-ttu-id="09c37-122">3</span><span class="sxs-lookup"><span data-stu-id="09c37-122">3</span></span>|<span data-ttu-id="09c37-123">C 分类供子级下 14</span><span class="sxs-lookup"><span data-stu-id="09c37-123">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="09c37-124">常规</span><span class="sxs-lookup"><span data-stu-id="09c37-124">general</span></span>|<span data-ttu-id="09c37-125">4</span><span class="sxs-lookup"><span data-stu-id="09c37-125">4</span></span>|<span data-ttu-id="09c37-126">G 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="09c37-126">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="09c37-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="09c37-127">parentalGuidance</span></span>|<span data-ttu-id="09c37-128">5</span><span class="sxs-lookup"><span data-stu-id="09c37-128">5</span></span>|<span data-ttu-id="09c37-129">PG 分类建议为年轻的查看者</span><span class="sxs-lookup"><span data-stu-id="09c37-129">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="09c37-130">成熟的</span><span class="sxs-lookup"><span data-stu-id="09c37-130">mature</span></span>|<span data-ttu-id="09c37-131">6</span><span class="sxs-lookup"><span data-stu-id="09c37-131">6</span></span>|<span data-ttu-id="09c37-132">M 分类建议为查看者超过 15</span><span class="sxs-lookup"><span data-stu-id="09c37-132">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="09c37-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="09c37-133">agesAbove15</span></span>|<span data-ttu-id="09c37-134">7</span><span class="sxs-lookup"><span data-stu-id="09c37-134">7</span></span>|<span data-ttu-id="09c37-135">MA15 + 分类不适用于查看在 15</span><span class="sxs-lookup"><span data-stu-id="09c37-135">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="09c37-136">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="09c37-136">agesAbove15AdultViolence</span></span>|<span data-ttu-id="09c37-137">8</span><span class="sxs-lookup"><span data-stu-id="09c37-137">8</span></span>|<span data-ttu-id="09c37-138">AV15 + 分类不适合下 15，成人暴力特有的查看者</span><span class="sxs-lookup"><span data-stu-id="09c37-138">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|




