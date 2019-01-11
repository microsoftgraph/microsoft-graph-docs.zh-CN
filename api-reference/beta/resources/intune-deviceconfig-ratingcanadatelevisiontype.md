---
title: ratingCanadaTelevisionType 枚举类型
description: 在加拿大 TV 内容评级标签
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ae8eb2232b2efcf38c26ecd6d0a5f3c830913e36
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890207"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="24372-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="24372-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="24372-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="24372-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24372-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="24372-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24372-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="24372-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24372-107">在加拿大 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="24372-107">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="24372-108">成员</span><span class="sxs-lookup"><span data-stu-id="24372-108">Members</span></span>
|<span data-ttu-id="24372-109">成员</span><span class="sxs-lookup"><span data-stu-id="24372-109">Member</span></span>|<span data-ttu-id="24372-110">值</span><span class="sxs-lookup"><span data-stu-id="24372-110">Value</span></span>|<span data-ttu-id="24372-111">Description</span><span class="sxs-lookup"><span data-stu-id="24372-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24372-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="24372-112">allAllowed</span></span>|<span data-ttu-id="24372-113">0</span><span class="sxs-lookup"><span data-stu-id="24372-113">0</span></span>|<span data-ttu-id="24372-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="24372-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="24372-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="24372-115">allBlocked</span></span>|<span data-ttu-id="24372-116">1</span><span class="sxs-lookup"><span data-stu-id="24372-116">1</span></span>|<span data-ttu-id="24372-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="24372-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="24372-118">children</span><span class="sxs-lookup"><span data-stu-id="24372-118">children</span></span>|<span data-ttu-id="24372-119">2</span><span class="sxs-lookup"><span data-stu-id="24372-119">2</span></span>|<span data-ttu-id="24372-120">C 分类适合子级岁 2 到步骤 7 年</span><span class="sxs-lookup"><span data-stu-id="24372-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="24372-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="24372-121">childrenAbove8</span></span>|<span data-ttu-id="24372-122">3</span><span class="sxs-lookup"><span data-stu-id="24372-122">3</span></span>|<span data-ttu-id="24372-123">C8 分类适合子级老化 8 +</span><span class="sxs-lookup"><span data-stu-id="24372-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="24372-124">常规</span><span class="sxs-lookup"><span data-stu-id="24372-124">general</span></span>|<span data-ttu-id="24372-125">4</span><span class="sxs-lookup"><span data-stu-id="24372-125">4</span></span>|<span data-ttu-id="24372-126">G 分类是适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="24372-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="24372-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="24372-127">parentalGuidance</span></span>|<span data-ttu-id="24372-128">5</span><span class="sxs-lookup"><span data-stu-id="24372-128">5</span></span>|<span data-ttu-id="24372-129">PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="24372-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="24372-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="24372-130">agesAbove14</span></span>|<span data-ttu-id="24372-131">6</span><span class="sxs-lookup"><span data-stu-id="24372-131">6</span></span>|<span data-ttu-id="24372-132">14 + 分类供查看岁 14 及较早</span><span class="sxs-lookup"><span data-stu-id="24372-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="24372-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="24372-133">agesAbove18</span></span>|<span data-ttu-id="24372-134">7</span><span class="sxs-lookup"><span data-stu-id="24372-134">7</span></span>|<span data-ttu-id="24372-135">18 + 分类供查看岁 18 及较早</span><span class="sxs-lookup"><span data-stu-id="24372-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|





