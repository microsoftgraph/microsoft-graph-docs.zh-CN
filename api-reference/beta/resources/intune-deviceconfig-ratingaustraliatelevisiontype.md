---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚中的 TV 内容评级标签
ms.openlocfilehash: add9febca378dc2be766c0013ace5ed0987578fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041369"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="38e78-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="38e78-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="38e78-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="38e78-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38e78-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38e78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38e78-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="38e78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38e78-107">澳大利亚中的 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="38e78-107">TV content rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="38e78-108">成员</span><span class="sxs-lookup"><span data-stu-id="38e78-108">Members</span></span>
|<span data-ttu-id="38e78-109">成员</span><span class="sxs-lookup"><span data-stu-id="38e78-109">Member</span></span>|<span data-ttu-id="38e78-110">值</span><span class="sxs-lookup"><span data-stu-id="38e78-110">Value</span></span>|<span data-ttu-id="38e78-111">说明</span><span class="sxs-lookup"><span data-stu-id="38e78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38e78-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="38e78-112">allAllowed</span></span>|<span data-ttu-id="38e78-113">0</span><span class="sxs-lookup"><span data-stu-id="38e78-113">0</span></span>|<span data-ttu-id="38e78-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="38e78-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="38e78-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="38e78-115">allBlocked</span></span>|<span data-ttu-id="38e78-116">1</span><span class="sxs-lookup"><span data-stu-id="38e78-116">1</span></span>|<span data-ttu-id="38e78-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="38e78-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="38e78-118">preschoolers</span><span class="sxs-lookup"><span data-stu-id="38e78-118">preschoolers</span></span>|<span data-ttu-id="38e78-119">2</span><span class="sxs-lookup"><span data-stu-id="38e78-119">2</span></span>|<span data-ttu-id="38e78-120">P 分类供 preschoolers</span><span class="sxs-lookup"><span data-stu-id="38e78-120">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="38e78-121">children</span><span class="sxs-lookup"><span data-stu-id="38e78-121">children</span></span>|<span data-ttu-id="38e78-122">3</span><span class="sxs-lookup"><span data-stu-id="38e78-122">3</span></span>|<span data-ttu-id="38e78-123">C 分类供子级下 14</span><span class="sxs-lookup"><span data-stu-id="38e78-123">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="38e78-124">常规</span><span class="sxs-lookup"><span data-stu-id="38e78-124">general</span></span>|<span data-ttu-id="38e78-125">4</span><span class="sxs-lookup"><span data-stu-id="38e78-125">4</span></span>|<span data-ttu-id="38e78-126">G 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="38e78-126">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="38e78-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="38e78-127">parentalGuidance</span></span>|<span data-ttu-id="38e78-128">5</span><span class="sxs-lookup"><span data-stu-id="38e78-128">5</span></span>|<span data-ttu-id="38e78-129">PG 分类建议为年轻的查看者</span><span class="sxs-lookup"><span data-stu-id="38e78-129">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="38e78-130">成熟的</span><span class="sxs-lookup"><span data-stu-id="38e78-130">mature</span></span>|<span data-ttu-id="38e78-131">6</span><span class="sxs-lookup"><span data-stu-id="38e78-131">6</span></span>|<span data-ttu-id="38e78-132">M 分类建议为查看者超过 15</span><span class="sxs-lookup"><span data-stu-id="38e78-132">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="38e78-133">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="38e78-133">agesAbove15</span></span>|<span data-ttu-id="38e78-134">7</span><span class="sxs-lookup"><span data-stu-id="38e78-134">7</span></span>|<span data-ttu-id="38e78-135">MA15 + 分类不适用于查看在 15</span><span class="sxs-lookup"><span data-stu-id="38e78-135">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="38e78-136">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="38e78-136">agesAbove15AdultViolence</span></span>|<span data-ttu-id="38e78-137">8</span><span class="sxs-lookup"><span data-stu-id="38e78-137">8</span></span>|<span data-ttu-id="38e78-138">AV15 + 分类不适合下 15，成人暴力特有的查看者</span><span class="sxs-lookup"><span data-stu-id="38e78-138">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|





