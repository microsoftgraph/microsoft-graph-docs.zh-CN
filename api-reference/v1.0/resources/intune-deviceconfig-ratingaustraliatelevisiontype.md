---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fc71a7dc5b5eaba65612090224928073bde8ba2b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355762"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="4ab93-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4ab93-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="4ab93-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ab93-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ab93-105">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="4ab93-105">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="4ab93-106">成员</span><span class="sxs-lookup"><span data-stu-id="4ab93-106">Members</span></span>
|<span data-ttu-id="4ab93-107">成员</span><span class="sxs-lookup"><span data-stu-id="4ab93-107">Member</span></span>|<span data-ttu-id="4ab93-108">值</span><span class="sxs-lookup"><span data-stu-id="4ab93-108">Value</span></span>|<span data-ttu-id="4ab93-109">说明</span><span class="sxs-lookup"><span data-stu-id="4ab93-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ab93-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="4ab93-110">allAllowed</span></span>|<span data-ttu-id="4ab93-111">0</span><span class="sxs-lookup"><span data-stu-id="4ab93-111">0</span></span>|<span data-ttu-id="4ab93-112">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="4ab93-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="4ab93-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="4ab93-113">allBlocked</span></span>|<span data-ttu-id="4ab93-114">1</span><span class="sxs-lookup"><span data-stu-id="4ab93-114">1</span></span>|<span data-ttu-id="4ab93-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="4ab93-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="4ab93-116">preschoolers</span><span class="sxs-lookup"><span data-stu-id="4ab93-116">preschoolers</span></span>|<span data-ttu-id="4ab93-117">双面</span><span class="sxs-lookup"><span data-stu-id="4ab93-117">2</span></span>|<span data-ttu-id="4ab93-118">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="4ab93-118">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="4ab93-119">children</span><span class="sxs-lookup"><span data-stu-id="4ab93-119">children</span></span>|<span data-ttu-id="4ab93-120">第三章</span><span class="sxs-lookup"><span data-stu-id="4ab93-120">3</span></span>|<span data-ttu-id="4ab93-121">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="4ab93-121">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="4ab93-122">概要</span><span class="sxs-lookup"><span data-stu-id="4ab93-122">general</span></span>|<span data-ttu-id="4ab93-123">4</span><span class="sxs-lookup"><span data-stu-id="4ab93-123">4</span></span>|<span data-ttu-id="4ab93-124">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="4ab93-124">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="4ab93-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="4ab93-125">parentalGuidance</span></span>|<span data-ttu-id="4ab93-126">5</span><span class="sxs-lookup"><span data-stu-id="4ab93-126">5</span></span>|<span data-ttu-id="4ab93-127">对于年轻人查看者，建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="4ab93-127">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="4ab93-128">成熟</span><span class="sxs-lookup"><span data-stu-id="4ab93-128">mature</span></span>|<span data-ttu-id="4ab93-129">型</span><span class="sxs-lookup"><span data-stu-id="4ab93-129">6</span></span>|<span data-ttu-id="4ab93-130">对于超过15的查看者，建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="4ab93-130">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="4ab93-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="4ab93-131">agesAbove15</span></span>|<span data-ttu-id="4ab93-132">步</span><span class="sxs-lookup"><span data-stu-id="4ab93-132">7</span></span>|<span data-ttu-id="4ab93-133">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="4ab93-133">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="4ab93-134">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="4ab93-134">agesAbove15AdultViolence</span></span>|<span data-ttu-id="4ab93-135">utf-8</span><span class="sxs-lookup"><span data-stu-id="4ab93-135">8</span></span>|<span data-ttu-id="4ab93-136">AV15 + 分类不适用于15岁以上的观众，特别是成人</span><span class="sxs-lookup"><span data-stu-id="4ab93-136">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|




