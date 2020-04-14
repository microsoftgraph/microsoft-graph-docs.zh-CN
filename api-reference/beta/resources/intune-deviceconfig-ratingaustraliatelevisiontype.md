---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e18b51c2a193cd7d75479cf15b0e505093cc2b9c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436980"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="17de5-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="17de5-103">ratingAustraliaTelevisionType enum type</span></span>

<span data-ttu-id="17de5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17de5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17de5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="17de5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17de5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17de5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17de5-107">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="17de5-107">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="17de5-108">成员</span><span class="sxs-lookup"><span data-stu-id="17de5-108">Members</span></span>
|<span data-ttu-id="17de5-109">成员</span><span class="sxs-lookup"><span data-stu-id="17de5-109">Member</span></span>|<span data-ttu-id="17de5-110">值</span><span class="sxs-lookup"><span data-stu-id="17de5-110">Value</span></span>|<span data-ttu-id="17de5-111">说明</span><span class="sxs-lookup"><span data-stu-id="17de5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17de5-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="17de5-112">allAllowed</span></span>|<span data-ttu-id="17de5-113">0</span><span class="sxs-lookup"><span data-stu-id="17de5-113">0</span></span>|<span data-ttu-id="17de5-114">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="17de5-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="17de5-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="17de5-115">allBlocked</span></span>|<span data-ttu-id="17de5-116">1</span><span class="sxs-lookup"><span data-stu-id="17de5-116">1</span></span>|<span data-ttu-id="17de5-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="17de5-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="17de5-118">preschoolers</span><span class="sxs-lookup"><span data-stu-id="17de5-118">preschoolers</span></span>|<span data-ttu-id="17de5-119">双面</span><span class="sxs-lookup"><span data-stu-id="17de5-119">2</span></span>|<span data-ttu-id="17de5-120">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="17de5-120">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="17de5-121">children</span><span class="sxs-lookup"><span data-stu-id="17de5-121">children</span></span>|<span data-ttu-id="17de5-122">第三章</span><span class="sxs-lookup"><span data-stu-id="17de5-122">3</span></span>|<span data-ttu-id="17de5-123">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="17de5-123">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="17de5-124">概要</span><span class="sxs-lookup"><span data-stu-id="17de5-124">general</span></span>|<span data-ttu-id="17de5-125">4 </span><span class="sxs-lookup"><span data-stu-id="17de5-125">4</span></span>|<span data-ttu-id="17de5-126">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="17de5-126">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="17de5-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="17de5-127">parentalGuidance</span></span>|<span data-ttu-id="17de5-128">5 </span><span class="sxs-lookup"><span data-stu-id="17de5-128">5</span></span>|<span data-ttu-id="17de5-129">对于年轻人查看者，建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="17de5-129">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="17de5-130">成熟</span><span class="sxs-lookup"><span data-stu-id="17de5-130">mature</span></span>|<span data-ttu-id="17de5-131">6 </span><span class="sxs-lookup"><span data-stu-id="17de5-131">6</span></span>|<span data-ttu-id="17de5-132">对于超过15的查看者，建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="17de5-132">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="17de5-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="17de5-133">agesAbove15</span></span>|<span data-ttu-id="17de5-134">7 </span><span class="sxs-lookup"><span data-stu-id="17de5-134">7</span></span>|<span data-ttu-id="17de5-135">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="17de5-135">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="17de5-136">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="17de5-136">agesAbove15AdultViolence</span></span>|<span data-ttu-id="17de5-137">8 </span><span class="sxs-lookup"><span data-stu-id="17de5-137">8</span></span>|<span data-ttu-id="17de5-138">AV15 + 分类不适用于15岁以上的观众，特别是成人</span><span class="sxs-lookup"><span data-stu-id="17de5-138">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



