---
title: ratingAustraliaTelevisionType 枚举类型
description: 澳大利亚电视内容分级标签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f7b1b3a820044ee7be701d6554acb501565b8a98
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760235"
---
# <a name="ratingaustraliatelevisiontype-enum-type"></a><span data-ttu-id="70bee-103">ratingAustraliaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="70bee-103">ratingAustraliaTelevisionType enum type</span></span>

<span data-ttu-id="70bee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70bee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70bee-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="70bee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70bee-106">澳大利亚电视内容分级标签</span><span class="sxs-lookup"><span data-stu-id="70bee-106">TV content rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="70bee-107">成员</span><span class="sxs-lookup"><span data-stu-id="70bee-107">Members</span></span>
|<span data-ttu-id="70bee-108">成员</span><span class="sxs-lookup"><span data-stu-id="70bee-108">Member</span></span>|<span data-ttu-id="70bee-109">值</span><span class="sxs-lookup"><span data-stu-id="70bee-109">Value</span></span>|<span data-ttu-id="70bee-110">说明</span><span class="sxs-lookup"><span data-stu-id="70bee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70bee-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="70bee-111">allAllowed</span></span>|<span data-ttu-id="70bee-112">0</span><span class="sxs-lookup"><span data-stu-id="70bee-112">0</span></span>|<span data-ttu-id="70bee-113">默认值，允许所有电视显示内容</span><span class="sxs-lookup"><span data-stu-id="70bee-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="70bee-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="70bee-114">allBlocked</span></span>|<span data-ttu-id="70bee-115">1</span><span class="sxs-lookup"><span data-stu-id="70bee-115">1</span></span>|<span data-ttu-id="70bee-116">不允许任何电视展示内容</span><span class="sxs-lookup"><span data-stu-id="70bee-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="70bee-117">一些</span><span class="sxs-lookup"><span data-stu-id="70bee-117">preschoolers</span></span>|<span data-ttu-id="70bee-118">2</span><span class="sxs-lookup"><span data-stu-id="70bee-118">2</span></span>|<span data-ttu-id="70bee-119">P 分类适用于分类者</span><span class="sxs-lookup"><span data-stu-id="70bee-119">The P classification is intended for preschoolers</span></span>|
|<span data-ttu-id="70bee-120">children</span><span class="sxs-lookup"><span data-stu-id="70bee-120">children</span></span>|<span data-ttu-id="70bee-121">3</span><span class="sxs-lookup"><span data-stu-id="70bee-121">3</span></span>|<span data-ttu-id="70bee-122">C 分类适用于 14 以下的子级</span><span class="sxs-lookup"><span data-stu-id="70bee-122">The C classification is intended for children under 14</span></span>|
|<span data-ttu-id="70bee-123">general</span><span class="sxs-lookup"><span data-stu-id="70bee-123">general</span></span>|<span data-ttu-id="70bee-124">4 </span><span class="sxs-lookup"><span data-stu-id="70bee-124">4</span></span>|<span data-ttu-id="70bee-125">G 分类适用于所有年龄</span><span class="sxs-lookup"><span data-stu-id="70bee-125">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="70bee-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="70bee-126">parentalGuidance</span></span>|<span data-ttu-id="70bee-127">5 </span><span class="sxs-lookup"><span data-stu-id="70bee-127">5</span></span>|<span data-ttu-id="70bee-128">建议让年青查看者使用 PG 分类</span><span class="sxs-lookup"><span data-stu-id="70bee-128">The PG classification is recommended for young viewers</span></span>|
|<span data-ttu-id="70bee-129">到期</span><span class="sxs-lookup"><span data-stu-id="70bee-129">mature</span></span>|<span data-ttu-id="70bee-130">6 </span><span class="sxs-lookup"><span data-stu-id="70bee-130">6</span></span>|<span data-ttu-id="70bee-131">建议超过 15 的查看者使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="70bee-131">The M classification is recommended for viewers over 15</span></span>|
|<span data-ttu-id="70bee-132">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="70bee-132">agesAbove15</span></span>|<span data-ttu-id="70bee-133">7 </span><span class="sxs-lookup"><span data-stu-id="70bee-133">7</span></span>|<span data-ttu-id="70bee-134">MA15+ 分类不适合 15 以下的查看者</span><span class="sxs-lookup"><span data-stu-id="70bee-134">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="70bee-135">agesAbove15AdultViolence</span><span class="sxs-lookup"><span data-stu-id="70bee-135">agesAbove15AdultViolence</span></span>|<span data-ttu-id="70bee-136">8 </span><span class="sxs-lookup"><span data-stu-id="70bee-136">8</span></span>|<span data-ttu-id="70bee-137">AV15+ 分类不适用于 15- 成人特定暴力的查看器</span><span class="sxs-lookup"><span data-stu-id="70bee-137">The AV15+ classification is not suitable for viewers under 15, adult violence-specific</span></span>|




