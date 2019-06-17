---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a33d4998e3e2949c6833d82110b7e24c574b0307
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995775"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="02153-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="02153-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="02153-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02153-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02153-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02153-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02153-106">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="02153-106">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="02153-107">成员</span><span class="sxs-lookup"><span data-stu-id="02153-107">Members</span></span>
|<span data-ttu-id="02153-108">成员</span><span class="sxs-lookup"><span data-stu-id="02153-108">Member</span></span>|<span data-ttu-id="02153-109">值</span><span class="sxs-lookup"><span data-stu-id="02153-109">Value</span></span>|<span data-ttu-id="02153-110">说明</span><span class="sxs-lookup"><span data-stu-id="02153-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02153-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="02153-111">allAllowed</span></span>|<span data-ttu-id="02153-112">0</span><span class="sxs-lookup"><span data-stu-id="02153-112">0</span></span>|<span data-ttu-id="02153-113">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="02153-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="02153-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="02153-114">allBlocked</span></span>|<span data-ttu-id="02153-115">1</span><span class="sxs-lookup"><span data-stu-id="02153-115">1</span></span>|<span data-ttu-id="02153-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="02153-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="02153-117">preschoolers</span><span class="sxs-lookup"><span data-stu-id="02153-117">preschoolers</span></span>|<span data-ttu-id="02153-118">双面</span><span class="sxs-lookup"><span data-stu-id="02153-118">2</span></span>|<span data-ttu-id="02153-119">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="02153-119">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="02153-120">children</span><span class="sxs-lookup"><span data-stu-id="02153-120">children</span></span>|<span data-ttu-id="02153-121">第三章</span><span class="sxs-lookup"><span data-stu-id="02153-121">3</span></span>|<span data-ttu-id="02153-122">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="02153-122">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="02153-123">概要</span><span class="sxs-lookup"><span data-stu-id="02153-123">general</span></span>|<span data-ttu-id="02153-124">4</span><span class="sxs-lookup"><span data-stu-id="02153-124">4</span></span>|<span data-ttu-id="02153-125">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="02153-125">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="02153-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="02153-126">parentalGuidance</span></span>|<span data-ttu-id="02153-127">5</span><span class="sxs-lookup"><span data-stu-id="02153-127">5</span></span>|<span data-ttu-id="02153-128">对于年轻人查看者, 建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="02153-128">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="02153-129">成熟</span><span class="sxs-lookup"><span data-stu-id="02153-129">mature</span></span>|<span data-ttu-id="02153-130">型</span><span class="sxs-lookup"><span data-stu-id="02153-130">6</span></span>|<span data-ttu-id="02153-131">对于超过15的查看者, 建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="02153-131">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="02153-132">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="02153-132">agesAbove15</span></span>|<span data-ttu-id="02153-133">步</span><span class="sxs-lookup"><span data-stu-id="02153-133">7</span></span>|<span data-ttu-id="02153-134">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="02153-134">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="02153-135">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="02153-135">agesAbove15AdultViolence</span></span>|<span data-ttu-id="02153-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="02153-136">8</span></span>|<span data-ttu-id="02153-137">AV15 + 分类不适用于15岁以上的观众, 特别是成人</span><span class="sxs-lookup"><span data-stu-id="02153-137">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|





