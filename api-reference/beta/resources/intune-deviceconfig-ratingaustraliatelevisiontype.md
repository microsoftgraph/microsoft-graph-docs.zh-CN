---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a65d8b272e99a3a8432214b3ac51916bc6e9f50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566701"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="bd8b7-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bd8b7-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="bd8b7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd8b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd8b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd8b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd8b7-106">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="bd8b7-106">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="bd8b7-107">成员</span><span class="sxs-lookup"><span data-stu-id="bd8b7-107">Members</span></span>
|<span data-ttu-id="bd8b7-108">成员</span><span class="sxs-lookup"><span data-stu-id="bd8b7-108">Member</span></span>|<span data-ttu-id="bd8b7-109">值</span><span class="sxs-lookup"><span data-stu-id="bd8b7-109">Value</span></span>|<span data-ttu-id="bd8b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="bd8b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd8b7-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="bd8b7-111">allAllowed</span></span>|<span data-ttu-id="bd8b7-112">0</span><span class="sxs-lookup"><span data-stu-id="bd8b7-112">0</span></span>|<span data-ttu-id="bd8b7-113">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="bd8b7-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="bd8b7-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="bd8b7-114">allBlocked</span></span>|<span data-ttu-id="bd8b7-115">1</span><span class="sxs-lookup"><span data-stu-id="bd8b7-115">1</span></span>|<span data-ttu-id="bd8b7-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="bd8b7-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="bd8b7-117">preschoolers</span><span class="sxs-lookup"><span data-stu-id="bd8b7-117">preschoolers</span></span>|<span data-ttu-id="bd8b7-118">2 </span><span class="sxs-lookup"><span data-stu-id="bd8b7-118">2</span></span>|<span data-ttu-id="bd8b7-119">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="bd8b7-119">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="bd8b7-120">children</span><span class="sxs-lookup"><span data-stu-id="bd8b7-120">children</span></span>|<span data-ttu-id="bd8b7-121">3 </span><span class="sxs-lookup"><span data-stu-id="bd8b7-121">3</span></span>|<span data-ttu-id="bd8b7-122">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="bd8b7-122">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="bd8b7-123">概要</span><span class="sxs-lookup"><span data-stu-id="bd8b7-123">general</span></span>|<span data-ttu-id="bd8b7-124">4 </span><span class="sxs-lookup"><span data-stu-id="bd8b7-124">4</span></span>|<span data-ttu-id="bd8b7-125">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="bd8b7-125">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="bd8b7-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="bd8b7-126">parentalGuidance</span></span>|<span data-ttu-id="bd8b7-127">5 </span><span class="sxs-lookup"><span data-stu-id="bd8b7-127">5</span></span>|<span data-ttu-id="bd8b7-128">对于年轻人查看者, 建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="bd8b7-128">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="bd8b7-129">成熟</span><span class="sxs-lookup"><span data-stu-id="bd8b7-129">mature</span></span>|<span data-ttu-id="bd8b7-130">6 </span><span class="sxs-lookup"><span data-stu-id="bd8b7-130">6</span></span>|<span data-ttu-id="bd8b7-131">对于超过15的查看者, 建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="bd8b7-131">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="bd8b7-132">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="bd8b7-132">agesAbove15</span></span>|<span data-ttu-id="bd8b7-133">7 </span><span class="sxs-lookup"><span data-stu-id="bd8b7-133">7</span></span>|<span data-ttu-id="bd8b7-134">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="bd8b7-134">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="bd8b7-135">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="bd8b7-135">agesAbove15AdultViolence</span></span>|<span data-ttu-id="bd8b7-136">8 </span><span class="sxs-lookup"><span data-stu-id="bd8b7-136">8</span></span>|<span data-ttu-id="bd8b7-137">AV15 + 分类不适用于15岁以上的观众, 特别是成人</span><span class="sxs-lookup"><span data-stu-id="bd8b7-137">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|





