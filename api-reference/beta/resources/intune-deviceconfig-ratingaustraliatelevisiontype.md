---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e86cc187f2047ac0636be0040c04763fdc4f6ec7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525948"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="5db99-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5db99-103">ratingAustraliaTelevisionType enum type</span></span>

<span data-ttu-id="5db99-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5db99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5db99-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5db99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5db99-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5db99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5db99-107">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="5db99-107">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="5db99-108">成员</span><span class="sxs-lookup"><span data-stu-id="5db99-108">Members</span></span>
|<span data-ttu-id="5db99-109">成员</span><span class="sxs-lookup"><span data-stu-id="5db99-109">Member</span></span>|<span data-ttu-id="5db99-110">值</span><span class="sxs-lookup"><span data-stu-id="5db99-110">Value</span></span>|<span data-ttu-id="5db99-111">说明</span><span class="sxs-lookup"><span data-stu-id="5db99-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5db99-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="5db99-112">allAllowed</span></span>|<span data-ttu-id="5db99-113">0</span><span class="sxs-lookup"><span data-stu-id="5db99-113">0</span></span>|<span data-ttu-id="5db99-114">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="5db99-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="5db99-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="5db99-115">allBlocked</span></span>|<span data-ttu-id="5db99-116">1 </span><span class="sxs-lookup"><span data-stu-id="5db99-116">1</span></span>|<span data-ttu-id="5db99-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="5db99-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="5db99-118">preschoolers</span><span class="sxs-lookup"><span data-stu-id="5db99-118">preschoolers</span></span>|<span data-ttu-id="5db99-119">2 </span><span class="sxs-lookup"><span data-stu-id="5db99-119">2</span></span>|<span data-ttu-id="5db99-120">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="5db99-120">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="5db99-121">children</span><span class="sxs-lookup"><span data-stu-id="5db99-121">children</span></span>|<span data-ttu-id="5db99-122">3 </span><span class="sxs-lookup"><span data-stu-id="5db99-122">3</span></span>|<span data-ttu-id="5db99-123">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="5db99-123">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="5db99-124">概要</span><span class="sxs-lookup"><span data-stu-id="5db99-124">general</span></span>|<span data-ttu-id="5db99-125">4 </span><span class="sxs-lookup"><span data-stu-id="5db99-125">4</span></span>|<span data-ttu-id="5db99-126">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="5db99-126">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="5db99-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="5db99-127">parentalGuidance</span></span>|<span data-ttu-id="5db99-128">5 </span><span class="sxs-lookup"><span data-stu-id="5db99-128">5</span></span>|<span data-ttu-id="5db99-129">对于年轻人查看者，建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="5db99-129">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="5db99-130">成熟</span><span class="sxs-lookup"><span data-stu-id="5db99-130">mature</span></span>|<span data-ttu-id="5db99-131">6 </span><span class="sxs-lookup"><span data-stu-id="5db99-131">6</span></span>|<span data-ttu-id="5db99-132">对于超过15的查看者，建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="5db99-132">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="5db99-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="5db99-133">agesAbove15</span></span>|<span data-ttu-id="5db99-134">7 </span><span class="sxs-lookup"><span data-stu-id="5db99-134">7</span></span>|<span data-ttu-id="5db99-135">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="5db99-135">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="5db99-136">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="5db99-136">agesAbove15AdultViolence</span></span>|<span data-ttu-id="5db99-137">8 </span><span class="sxs-lookup"><span data-stu-id="5db99-137">8</span></span>|<span data-ttu-id="5db99-138">AV15 + 分类不适用于15岁以上的观众，特别是成人</span><span class="sxs-lookup"><span data-stu-id="5db99-138">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



