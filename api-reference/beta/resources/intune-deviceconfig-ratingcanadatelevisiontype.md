---
title: ratingCanadaTelevisionType 枚举类型
description: 在加拿大 TV 内容评级标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 174a6d893220f21bafaafdc03880801947c2cd25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415640"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="54ba7-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="54ba7-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="54ba7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="54ba7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54ba7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="54ba7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54ba7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54ba7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54ba7-107">在加拿大 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="54ba7-107">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="54ba7-108">成员</span><span class="sxs-lookup"><span data-stu-id="54ba7-108">Members</span></span>
|<span data-ttu-id="54ba7-109">成员</span><span class="sxs-lookup"><span data-stu-id="54ba7-109">Member</span></span>|<span data-ttu-id="54ba7-110">值</span><span class="sxs-lookup"><span data-stu-id="54ba7-110">Value</span></span>|<span data-ttu-id="54ba7-111">说明</span><span class="sxs-lookup"><span data-stu-id="54ba7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54ba7-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="54ba7-112">allAllowed</span></span>|<span data-ttu-id="54ba7-113">0</span><span class="sxs-lookup"><span data-stu-id="54ba7-113">0</span></span>|<span data-ttu-id="54ba7-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="54ba7-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="54ba7-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="54ba7-115">allBlocked</span></span>|<span data-ttu-id="54ba7-116">1</span><span class="sxs-lookup"><span data-stu-id="54ba7-116">1</span></span>|<span data-ttu-id="54ba7-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="54ba7-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="54ba7-118">children</span><span class="sxs-lookup"><span data-stu-id="54ba7-118">children</span></span>|<span data-ttu-id="54ba7-119">2</span><span class="sxs-lookup"><span data-stu-id="54ba7-119">2</span></span>|<span data-ttu-id="54ba7-120">C 分类适合子级岁 2 到步骤 7 年</span><span class="sxs-lookup"><span data-stu-id="54ba7-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="54ba7-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="54ba7-121">childrenAbove8</span></span>|<span data-ttu-id="54ba7-122">3</span><span class="sxs-lookup"><span data-stu-id="54ba7-122">3</span></span>|<span data-ttu-id="54ba7-123">C8 分类适合子级老化 8 +</span><span class="sxs-lookup"><span data-stu-id="54ba7-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="54ba7-124">常规</span><span class="sxs-lookup"><span data-stu-id="54ba7-124">general</span></span>|<span data-ttu-id="54ba7-125">4</span><span class="sxs-lookup"><span data-stu-id="54ba7-125">4</span></span>|<span data-ttu-id="54ba7-126">G 分类是适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="54ba7-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="54ba7-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="54ba7-127">parentalGuidance</span></span>|<span data-ttu-id="54ba7-128">5</span><span class="sxs-lookup"><span data-stu-id="54ba7-128">5</span></span>|<span data-ttu-id="54ba7-129">PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="54ba7-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="54ba7-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="54ba7-130">agesAbove14</span></span>|<span data-ttu-id="54ba7-131">6</span><span class="sxs-lookup"><span data-stu-id="54ba7-131">6</span></span>|<span data-ttu-id="54ba7-132">14 + 分类供查看岁 14 及较早</span><span class="sxs-lookup"><span data-stu-id="54ba7-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="54ba7-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="54ba7-133">agesAbove18</span></span>|<span data-ttu-id="54ba7-134">7</span><span class="sxs-lookup"><span data-stu-id="54ba7-134">7</span></span>|<span data-ttu-id="54ba7-135">18 + 分类供查看岁 18 及较早</span><span class="sxs-lookup"><span data-stu-id="54ba7-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|




