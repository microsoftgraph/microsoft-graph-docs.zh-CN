---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚的电视内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3db2989c7cc61eec2cbd736c336c222c23e9a5fe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560793"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="b1a32-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b1a32-103">ratingAustraliaTelevisionType enum type</span></span>

> <span data-ttu-id="b1a32-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1a32-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1a32-105">澳大利亚的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="b1a32-105">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="b1a32-106">成员</span><span class="sxs-lookup"><span data-stu-id="b1a32-106">Members</span></span>
|<span data-ttu-id="b1a32-107">成员</span><span class="sxs-lookup"><span data-stu-id="b1a32-107">Member</span></span>|<span data-ttu-id="b1a32-108">值</span><span class="sxs-lookup"><span data-stu-id="b1a32-108">Value</span></span>|<span data-ttu-id="b1a32-109">说明</span><span class="sxs-lookup"><span data-stu-id="b1a32-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a32-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="b1a32-110">allAllowed</span></span>|<span data-ttu-id="b1a32-111">0</span><span class="sxs-lookup"><span data-stu-id="b1a32-111">0</span></span>|<span data-ttu-id="b1a32-112">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="b1a32-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="b1a32-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="b1a32-113">allBlocked</span></span>|<span data-ttu-id="b1a32-114">1</span><span class="sxs-lookup"><span data-stu-id="b1a32-114">1</span></span>|<span data-ttu-id="b1a32-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="b1a32-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="b1a32-116">preschoolers</span><span class="sxs-lookup"><span data-stu-id="b1a32-116">preschoolers</span></span>|<span data-ttu-id="b1a32-117">2 </span><span class="sxs-lookup"><span data-stu-id="b1a32-117">2</span></span>|<span data-ttu-id="b1a32-118">P 分类适用于 preschoolers</span><span class="sxs-lookup"><span data-stu-id="b1a32-118">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="b1a32-119">children</span><span class="sxs-lookup"><span data-stu-id="b1a32-119">children</span></span>|<span data-ttu-id="b1a32-120">3 </span><span class="sxs-lookup"><span data-stu-id="b1a32-120">3</span></span>|<span data-ttu-id="b1a32-121">C 分类适用于14下的儿童</span><span class="sxs-lookup"><span data-stu-id="b1a32-121">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="b1a32-122">概要</span><span class="sxs-lookup"><span data-stu-id="b1a32-122">general</span></span>|<span data-ttu-id="b1a32-123">4 </span><span class="sxs-lookup"><span data-stu-id="b1a32-123">4</span></span>|<span data-ttu-id="b1a32-124">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="b1a32-124">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="b1a32-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="b1a32-125">parentalGuidance</span></span>|<span data-ttu-id="b1a32-126">5 </span><span class="sxs-lookup"><span data-stu-id="b1a32-126">5</span></span>|<span data-ttu-id="b1a32-127">对于年轻人查看者, 建议使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="b1a32-127">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="b1a32-128">成熟</span><span class="sxs-lookup"><span data-stu-id="b1a32-128">mature</span></span>|<span data-ttu-id="b1a32-129">6 </span><span class="sxs-lookup"><span data-stu-id="b1a32-129">6</span></span>|<span data-ttu-id="b1a32-130">对于超过15的查看者, 建议使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="b1a32-130">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="b1a32-131">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="b1a32-131">agesAbove15</span></span>|<span data-ttu-id="b1a32-132">7 </span><span class="sxs-lookup"><span data-stu-id="b1a32-132">7</span></span>|<span data-ttu-id="b1a32-133">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="b1a32-133">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="b1a32-134">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="b1a32-134">agesAbove15AdultViolence</span></span>|<span data-ttu-id="b1a32-135">8 </span><span class="sxs-lookup"><span data-stu-id="b1a32-135">8</span></span>|<span data-ttu-id="b1a32-136">AV15 + 分类不适用于15岁以上的观众, 特别是成人</span><span class="sxs-lookup"><span data-stu-id="b1a32-136">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|



