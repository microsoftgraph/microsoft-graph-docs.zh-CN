---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7043dfe436fc13ba86a5173a60305b7303c3e5df
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532409"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="22d5a-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="22d5a-103">ratingAustraliaTelevisionType enum type</span></span>

<span data-ttu-id="22d5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22d5a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22d5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22d5a-106">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="22d5a-106">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="22d5a-107">成员</span><span class="sxs-lookup"><span data-stu-id="22d5a-107">Members</span></span>
|<span data-ttu-id="22d5a-108">成员</span><span class="sxs-lookup"><span data-stu-id="22d5a-108">Member</span></span>|<span data-ttu-id="22d5a-109">值</span><span class="sxs-lookup"><span data-stu-id="22d5a-109">Value</span></span>|<span data-ttu-id="22d5a-110">说明</span><span class="sxs-lookup"><span data-stu-id="22d5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d5a-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="22d5a-111">allAllowed</span></span>|<span data-ttu-id="22d5a-112">0</span><span class="sxs-lookup"><span data-stu-id="22d5a-112">0</span></span>|<span data-ttu-id="22d5a-113">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="22d5a-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="22d5a-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="22d5a-114">allBlocked</span></span>|<span data-ttu-id="22d5a-115">1 </span><span class="sxs-lookup"><span data-stu-id="22d5a-115">1</span></span>|<span data-ttu-id="22d5a-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="22d5a-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="22d5a-117">preschoolers</span><span class="sxs-lookup"><span data-stu-id="22d5a-117">preschoolers</span></span>|<span data-ttu-id="22d5a-118">2 </span><span class="sxs-lookup"><span data-stu-id="22d5a-118">2</span></span>|<span data-ttu-id="22d5a-119">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="22d5a-119">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="22d5a-120">children</span><span class="sxs-lookup"><span data-stu-id="22d5a-120">children</span></span>|<span data-ttu-id="22d5a-121">3 </span><span class="sxs-lookup"><span data-stu-id="22d5a-121">3</span></span>|<span data-ttu-id="22d5a-122">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="22d5a-122">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="22d5a-123">概要</span><span class="sxs-lookup"><span data-stu-id="22d5a-123">general</span></span>|<span data-ttu-id="22d5a-124">4 </span><span class="sxs-lookup"><span data-stu-id="22d5a-124">4</span></span>|<span data-ttu-id="22d5a-125">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="22d5a-125">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="22d5a-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="22d5a-126">parentalGuidance</span></span>|<span data-ttu-id="22d5a-127">5 </span><span class="sxs-lookup"><span data-stu-id="22d5a-127">5</span></span>|<span data-ttu-id="22d5a-128">对于年轻人查看者，建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="22d5a-128">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="22d5a-129">成熟</span><span class="sxs-lookup"><span data-stu-id="22d5a-129">mature</span></span>|<span data-ttu-id="22d5a-130">6 </span><span class="sxs-lookup"><span data-stu-id="22d5a-130">6</span></span>|<span data-ttu-id="22d5a-131">对于超过15的查看者，建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="22d5a-131">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="22d5a-132">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="22d5a-132">agesAbove15</span></span>|<span data-ttu-id="22d5a-133">7 </span><span class="sxs-lookup"><span data-stu-id="22d5a-133">7</span></span>|<span data-ttu-id="22d5a-134">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="22d5a-134">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="22d5a-135">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="22d5a-135">agesAbove15AdultViolence</span></span>|<span data-ttu-id="22d5a-136">8 </span><span class="sxs-lookup"><span data-stu-id="22d5a-136">8</span></span>|<span data-ttu-id="22d5a-137">AV15 + 分类不适用于15岁以上的观众，特别是成人</span><span class="sxs-lookup"><span data-stu-id="22d5a-137">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|




