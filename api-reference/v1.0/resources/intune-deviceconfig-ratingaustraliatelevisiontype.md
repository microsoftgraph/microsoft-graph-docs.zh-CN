---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚中的 TV 内容评级标签
author: tfitzmac
ms.openlocfilehash: 8444f7db49cc8a0453f58d4710334f0876e570c3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323056"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="30bf9-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="30bf9-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="30bf9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="30bf9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30bf9-105">澳大利亚中的 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="30bf9-105">TV content rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="30bf9-106">成员</span><span class="sxs-lookup"><span data-stu-id="30bf9-106">Members</span></span>
|<span data-ttu-id="30bf9-107">成员</span><span class="sxs-lookup"><span data-stu-id="30bf9-107">Member</span></span>|<span data-ttu-id="30bf9-108">值</span><span class="sxs-lookup"><span data-stu-id="30bf9-108">Value</span></span>|<span data-ttu-id="30bf9-109">说明</span><span class="sxs-lookup"><span data-stu-id="30bf9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30bf9-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="30bf9-110">allAllowed</span></span>|<span data-ttu-id="30bf9-111">0</span><span class="sxs-lookup"><span data-stu-id="30bf9-111">0</span></span>|<span data-ttu-id="30bf9-112">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="30bf9-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="30bf9-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="30bf9-113">allBlocked</span></span>|<span data-ttu-id="30bf9-114">1</span><span class="sxs-lookup"><span data-stu-id="30bf9-114">1</span></span>|<span data-ttu-id="30bf9-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="30bf9-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="30bf9-116">preschoolers</span><span class="sxs-lookup"><span data-stu-id="30bf9-116">preschoolers</span></span>|<span data-ttu-id="30bf9-117">2</span><span class="sxs-lookup"><span data-stu-id="30bf9-117">2</span></span>|<span data-ttu-id="30bf9-118">P 分类供 preschoolers</span><span class="sxs-lookup"><span data-stu-id="30bf9-118">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="30bf9-119">children</span><span class="sxs-lookup"><span data-stu-id="30bf9-119">children</span></span>|<span data-ttu-id="30bf9-120">3</span><span class="sxs-lookup"><span data-stu-id="30bf9-120">3</span></span>|<span data-ttu-id="30bf9-121">C 分类供子级下 14</span><span class="sxs-lookup"><span data-stu-id="30bf9-121">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="30bf9-122">常规</span><span class="sxs-lookup"><span data-stu-id="30bf9-122">general</span></span>|<span data-ttu-id="30bf9-123">4</span><span class="sxs-lookup"><span data-stu-id="30bf9-123">4</span></span>|<span data-ttu-id="30bf9-124">G 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="30bf9-124">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="30bf9-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="30bf9-125">parentalGuidance</span></span>|<span data-ttu-id="30bf9-126">5</span><span class="sxs-lookup"><span data-stu-id="30bf9-126">5</span></span>|<span data-ttu-id="30bf9-127">PG 分类建议为年轻的查看者</span><span class="sxs-lookup"><span data-stu-id="30bf9-127">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="30bf9-128">成熟的</span><span class="sxs-lookup"><span data-stu-id="30bf9-128">mature</span></span>|<span data-ttu-id="30bf9-129">6</span><span class="sxs-lookup"><span data-stu-id="30bf9-129">6</span></span>|<span data-ttu-id="30bf9-130">M 分类建议为查看者超过 15</span><span class="sxs-lookup"><span data-stu-id="30bf9-130">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="30bf9-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="30bf9-131">agesAbove15</span></span>|<span data-ttu-id="30bf9-132">7</span><span class="sxs-lookup"><span data-stu-id="30bf9-132">7</span></span>|<span data-ttu-id="30bf9-133">MA15 + 分类不适用于查看在 15</span><span class="sxs-lookup"><span data-stu-id="30bf9-133">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="30bf9-134">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="30bf9-134">agesAbove15AdultViolence</span></span>|<span data-ttu-id="30bf9-135">8</span><span class="sxs-lookup"><span data-stu-id="30bf9-135">8</span></span>|<span data-ttu-id="30bf9-136">AV15 + 分类不适合下 15，成人暴力特有的查看者</span><span class="sxs-lookup"><span data-stu-id="30bf9-136">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



