---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c1aa9f7419d3eb49f22381dcea23ca901b39168e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701331"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="923c0-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="923c0-103">ratingAustraliaTelevisionType enum type</span></span>

<span data-ttu-id="923c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="923c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="923c0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="923c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="923c0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="923c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="923c0-107">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="923c0-107">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="923c0-108">成员</span><span class="sxs-lookup"><span data-stu-id="923c0-108">Members</span></span>
|<span data-ttu-id="923c0-109">成员</span><span class="sxs-lookup"><span data-stu-id="923c0-109">Member</span></span>|<span data-ttu-id="923c0-110">值</span><span class="sxs-lookup"><span data-stu-id="923c0-110">Value</span></span>|<span data-ttu-id="923c0-111">说明</span><span class="sxs-lookup"><span data-stu-id="923c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="923c0-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="923c0-112">allAllowed</span></span>|<span data-ttu-id="923c0-113">0</span><span class="sxs-lookup"><span data-stu-id="923c0-113">0</span></span>|<span data-ttu-id="923c0-114">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="923c0-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="923c0-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="923c0-115">allBlocked</span></span>|<span data-ttu-id="923c0-116">1</span><span class="sxs-lookup"><span data-stu-id="923c0-116">1</span></span>|<span data-ttu-id="923c0-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="923c0-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="923c0-118">preschoolers</span><span class="sxs-lookup"><span data-stu-id="923c0-118">preschoolers</span></span>|<span data-ttu-id="923c0-119">双面</span><span class="sxs-lookup"><span data-stu-id="923c0-119">2</span></span>|<span data-ttu-id="923c0-120">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="923c0-120">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="923c0-121">children</span><span class="sxs-lookup"><span data-stu-id="923c0-121">children</span></span>|<span data-ttu-id="923c0-122">第三章</span><span class="sxs-lookup"><span data-stu-id="923c0-122">3</span></span>|<span data-ttu-id="923c0-123">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="923c0-123">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="923c0-124">概要</span><span class="sxs-lookup"><span data-stu-id="923c0-124">general</span></span>|<span data-ttu-id="923c0-125">4 </span><span class="sxs-lookup"><span data-stu-id="923c0-125">4</span></span>|<span data-ttu-id="923c0-126">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="923c0-126">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="923c0-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="923c0-127">parentalGuidance</span></span>|<span data-ttu-id="923c0-128">5 </span><span class="sxs-lookup"><span data-stu-id="923c0-128">5</span></span>|<span data-ttu-id="923c0-129">对于年轻人查看者，建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="923c0-129">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="923c0-130">成熟</span><span class="sxs-lookup"><span data-stu-id="923c0-130">mature</span></span>|<span data-ttu-id="923c0-131">6 </span><span class="sxs-lookup"><span data-stu-id="923c0-131">6</span></span>|<span data-ttu-id="923c0-132">对于超过15的查看者，建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="923c0-132">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="923c0-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="923c0-133">agesAbove15</span></span>|<span data-ttu-id="923c0-134">7 </span><span class="sxs-lookup"><span data-stu-id="923c0-134">7</span></span>|<span data-ttu-id="923c0-135">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="923c0-135">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="923c0-136">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="923c0-136">agesAbove15AdultViolence</span></span>|<span data-ttu-id="923c0-137">8 </span><span class="sxs-lookup"><span data-stu-id="923c0-137">8</span></span>|<span data-ttu-id="923c0-138">AV15 + 分类不适用于15岁以上的观众，特别是成人</span><span class="sxs-lookup"><span data-stu-id="923c0-138">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|





