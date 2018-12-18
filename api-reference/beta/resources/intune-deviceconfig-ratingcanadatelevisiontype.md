---
title: ratingCanadaTelevisionType 枚举类型
description: 在加拿大 TV 内容评级标签
author: tfitzmac
ms.openlocfilehash: fdd587a5a0917aea9a8ec028f30b13d1548e6981
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316945"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="e4030-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e4030-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="e4030-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e4030-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4030-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e4030-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4030-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e4030-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4030-107">在加拿大 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="e4030-107">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="e4030-108">成员</span><span class="sxs-lookup"><span data-stu-id="e4030-108">Members</span></span>
|<span data-ttu-id="e4030-109">成员</span><span class="sxs-lookup"><span data-stu-id="e4030-109">Member</span></span>|<span data-ttu-id="e4030-110">值</span><span class="sxs-lookup"><span data-stu-id="e4030-110">Value</span></span>|<span data-ttu-id="e4030-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4030-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4030-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="e4030-112">allAllowed</span></span>|<span data-ttu-id="e4030-113">0</span><span class="sxs-lookup"><span data-stu-id="e4030-113">0</span></span>|<span data-ttu-id="e4030-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="e4030-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="e4030-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="e4030-115">allBlocked</span></span>|<span data-ttu-id="e4030-116">1</span><span class="sxs-lookup"><span data-stu-id="e4030-116">1</span></span>|<span data-ttu-id="e4030-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="e4030-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="e4030-118">children</span><span class="sxs-lookup"><span data-stu-id="e4030-118">children</span></span>|<span data-ttu-id="e4030-119">2</span><span class="sxs-lookup"><span data-stu-id="e4030-119">2</span></span>|<span data-ttu-id="e4030-120">C 分类适合子级岁 2 到步骤 7 年</span><span class="sxs-lookup"><span data-stu-id="e4030-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="e4030-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="e4030-121">childrenAbove8</span></span>|<span data-ttu-id="e4030-122">3</span><span class="sxs-lookup"><span data-stu-id="e4030-122">3</span></span>|<span data-ttu-id="e4030-123">C8 分类适合子级老化 8 +</span><span class="sxs-lookup"><span data-stu-id="e4030-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="e4030-124">常规</span><span class="sxs-lookup"><span data-stu-id="e4030-124">general</span></span>|<span data-ttu-id="e4030-125">4</span><span class="sxs-lookup"><span data-stu-id="e4030-125">4</span></span>|<span data-ttu-id="e4030-126">G 分类是适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="e4030-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="e4030-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="e4030-127">parentalGuidance</span></span>|<span data-ttu-id="e4030-128">5</span><span class="sxs-lookup"><span data-stu-id="e4030-128">5</span></span>|<span data-ttu-id="e4030-129">PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="e4030-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="e4030-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="e4030-130">agesAbove14</span></span>|<span data-ttu-id="e4030-131">6</span><span class="sxs-lookup"><span data-stu-id="e4030-131">6</span></span>|<span data-ttu-id="e4030-132">14 + 分类供查看岁 14 及较早</span><span class="sxs-lookup"><span data-stu-id="e4030-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="e4030-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="e4030-133">agesAbove18</span></span>|<span data-ttu-id="e4030-134">7</span><span class="sxs-lookup"><span data-stu-id="e4030-134">7</span></span>|<span data-ttu-id="e4030-135">18 + 分类供查看岁 18 及较早</span><span class="sxs-lookup"><span data-stu-id="e4030-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|





