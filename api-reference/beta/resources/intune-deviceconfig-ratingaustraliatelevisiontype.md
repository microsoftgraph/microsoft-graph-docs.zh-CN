---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69fdd926d02a2ae150f10a0d911854538a5d2f69
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368357"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="d86ae-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d86ae-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="d86ae-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d86ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d86ae-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d86ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d86ae-106">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="d86ae-106">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="d86ae-107">成员</span><span class="sxs-lookup"><span data-stu-id="d86ae-107">Members</span></span>
|<span data-ttu-id="d86ae-108">成员</span><span class="sxs-lookup"><span data-stu-id="d86ae-108">Member</span></span>|<span data-ttu-id="d86ae-109">值</span><span class="sxs-lookup"><span data-stu-id="d86ae-109">Value</span></span>|<span data-ttu-id="d86ae-110">说明</span><span class="sxs-lookup"><span data-stu-id="d86ae-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d86ae-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="d86ae-111">allAllowed</span></span>|<span data-ttu-id="d86ae-112">0</span><span class="sxs-lookup"><span data-stu-id="d86ae-112">0</span></span>|<span data-ttu-id="d86ae-113">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="d86ae-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="d86ae-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="d86ae-114">allBlocked</span></span>|<span data-ttu-id="d86ae-115">1</span><span class="sxs-lookup"><span data-stu-id="d86ae-115">1</span></span>|<span data-ttu-id="d86ae-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="d86ae-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="d86ae-117">preschoolers</span><span class="sxs-lookup"><span data-stu-id="d86ae-117">preschoolers</span></span>|<span data-ttu-id="d86ae-118">双面</span><span class="sxs-lookup"><span data-stu-id="d86ae-118">2</span></span>|<span data-ttu-id="d86ae-119">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="d86ae-119">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="d86ae-120">children</span><span class="sxs-lookup"><span data-stu-id="d86ae-120">children</span></span>|<span data-ttu-id="d86ae-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d86ae-121">3</span></span>|<span data-ttu-id="d86ae-122">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="d86ae-122">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="d86ae-123">概要</span><span class="sxs-lookup"><span data-stu-id="d86ae-123">general</span></span>|<span data-ttu-id="d86ae-124">4</span><span class="sxs-lookup"><span data-stu-id="d86ae-124">4</span></span>|<span data-ttu-id="d86ae-125">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="d86ae-125">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="d86ae-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="d86ae-126">parentalGuidance</span></span>|<span data-ttu-id="d86ae-127">5</span><span class="sxs-lookup"><span data-stu-id="d86ae-127">5</span></span>|<span data-ttu-id="d86ae-128">对于年轻人查看者, 建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="d86ae-128">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="d86ae-129">成熟</span><span class="sxs-lookup"><span data-stu-id="d86ae-129">mature</span></span>|<span data-ttu-id="d86ae-130">型</span><span class="sxs-lookup"><span data-stu-id="d86ae-130">6</span></span>|<span data-ttu-id="d86ae-131">对于超过15的查看者, 建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="d86ae-131">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="d86ae-132">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="d86ae-132">agesAbove15</span></span>|<span data-ttu-id="d86ae-133">步</span><span class="sxs-lookup"><span data-stu-id="d86ae-133">7</span></span>|<span data-ttu-id="d86ae-134">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="d86ae-134">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="d86ae-135">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="d86ae-135">agesAbove15AdultViolence</span></span>|<span data-ttu-id="d86ae-136">utf-8</span><span class="sxs-lookup"><span data-stu-id="d86ae-136">8</span></span>|<span data-ttu-id="d86ae-137">AV15 + 分类不适用于15岁以上的观众, 特别是成人</span><span class="sxs-lookup"><span data-stu-id="d86ae-137">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



