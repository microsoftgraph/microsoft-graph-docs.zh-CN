---
title: ratingCanadaTelevisionType 枚举类型
description: 在加拿大 TV 内容评级标签
ms.openlocfilehash: 636a59e9bbb4c6ce09a9118b912cdd9c6be8440b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007958"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="d9347-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d9347-103">ratingCanadaTelevisionType enum type</span></span>

> <span data-ttu-id="d9347-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9347-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9347-105">在加拿大 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="d9347-105">TV content rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="d9347-106">成员</span><span class="sxs-lookup"><span data-stu-id="d9347-106">Members</span></span>
|<span data-ttu-id="d9347-107">成员</span><span class="sxs-lookup"><span data-stu-id="d9347-107">Member</span></span>|<span data-ttu-id="d9347-108">值</span><span class="sxs-lookup"><span data-stu-id="d9347-108">Value</span></span>|<span data-ttu-id="d9347-109">说明</span><span class="sxs-lookup"><span data-stu-id="d9347-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9347-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="d9347-110">allAllowed</span></span>|<span data-ttu-id="d9347-111">0</span><span class="sxs-lookup"><span data-stu-id="d9347-111">0</span></span>|<span data-ttu-id="d9347-112">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="d9347-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="d9347-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="d9347-113">allBlocked</span></span>|<span data-ttu-id="d9347-114">1</span><span class="sxs-lookup"><span data-stu-id="d9347-114">1</span></span>|<span data-ttu-id="d9347-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="d9347-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="d9347-116">children</span><span class="sxs-lookup"><span data-stu-id="d9347-116">children</span></span>|<span data-ttu-id="d9347-117">2</span><span class="sxs-lookup"><span data-stu-id="d9347-117">2</span></span>|<span data-ttu-id="d9347-118">C 分类适合子级岁 2 到步骤 7 年</span><span class="sxs-lookup"><span data-stu-id="d9347-118">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="d9347-119">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="d9347-119">childrenAbove8</span></span>|<span data-ttu-id="d9347-120">3</span><span class="sxs-lookup"><span data-stu-id="d9347-120">3</span></span>|<span data-ttu-id="d9347-121">C8 分类适合子级老化 8 +</span><span class="sxs-lookup"><span data-stu-id="d9347-121">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="d9347-122">常规</span><span class="sxs-lookup"><span data-stu-id="d9347-122">general</span></span>|<span data-ttu-id="d9347-123">4</span><span class="sxs-lookup"><span data-stu-id="d9347-123">4</span></span>|<span data-ttu-id="d9347-124">G 分类是适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="d9347-124">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="d9347-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="d9347-125">parentalGuidance</span></span>|<span data-ttu-id="d9347-126">5</span><span class="sxs-lookup"><span data-stu-id="d9347-126">5</span></span>|<span data-ttu-id="d9347-127">PG，家长的指南</span><span class="sxs-lookup"><span data-stu-id="d9347-127">PG, Parental Guidance</span></span>|
|<span data-ttu-id="d9347-128">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="d9347-128">agesAbove14</span></span>|<span data-ttu-id="d9347-129">6</span><span class="sxs-lookup"><span data-stu-id="d9347-129">6</span></span>|<span data-ttu-id="d9347-130">14 + 分类供查看岁 14 及较早</span><span class="sxs-lookup"><span data-stu-id="d9347-130">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="d9347-131">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="d9347-131">agesAbove18</span></span>|<span data-ttu-id="d9347-132">7</span><span class="sxs-lookup"><span data-stu-id="d9347-132">7</span></span>|<span data-ttu-id="d9347-133">18 + 分类供查看岁 18 及较早</span><span class="sxs-lookup"><span data-stu-id="d9347-133">The 18+ classification is intended for viewers ages 18 and older</span></span>|



