---
title: ratingCanadaTelevisionType 枚举类型
description: 加拿大的电视内容评级标签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0a033db304fa61a9823cc650344b2cc11e77855e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041426"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="f9ea8-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f9ea8-103">ratingCanadaTelevisionType enum type</span></span>

<span data-ttu-id="f9ea8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9ea8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9ea8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9ea8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ea8-106">加拿大的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="f9ea8-106">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="f9ea8-107">成员</span><span class="sxs-lookup"><span data-stu-id="f9ea8-107">Members</span></span>
|<span data-ttu-id="f9ea8-108">成员</span><span class="sxs-lookup"><span data-stu-id="f9ea8-108">Member</span></span>|<span data-ttu-id="f9ea8-109">值</span><span class="sxs-lookup"><span data-stu-id="f9ea8-109">Value</span></span>|<span data-ttu-id="f9ea8-110">说明</span><span class="sxs-lookup"><span data-stu-id="f9ea8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9ea8-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f9ea8-111">allAllowed</span></span>|<span data-ttu-id="f9ea8-112">0</span><span class="sxs-lookup"><span data-stu-id="f9ea8-112">0</span></span>|<span data-ttu-id="f9ea8-113">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="f9ea8-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="f9ea8-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f9ea8-114">allBlocked</span></span>|<span data-ttu-id="f9ea8-115">1 </span><span class="sxs-lookup"><span data-stu-id="f9ea8-115">1</span></span>|<span data-ttu-id="f9ea8-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="f9ea8-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="f9ea8-117">children</span><span class="sxs-lookup"><span data-stu-id="f9ea8-117">children</span></span>|<span data-ttu-id="f9ea8-118">2 </span><span class="sxs-lookup"><span data-stu-id="f9ea8-118">2</span></span>|<span data-ttu-id="f9ea8-119">C 分类适用于2到7年的儿童年龄</span><span class="sxs-lookup"><span data-stu-id="f9ea8-119">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="f9ea8-120">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="f9ea8-120">childrenAbove8</span></span>|<span data-ttu-id="f9ea8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f9ea8-121">3</span></span>|<span data-ttu-id="f9ea8-122">C8 分类适用于仅有8岁以上的儿童</span><span class="sxs-lookup"><span data-stu-id="f9ea8-122">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="f9ea8-123">概要</span><span class="sxs-lookup"><span data-stu-id="f9ea8-123">general</span></span>|<span data-ttu-id="f9ea8-124">4 </span><span class="sxs-lookup"><span data-stu-id="f9ea8-124">4</span></span>|<span data-ttu-id="f9ea8-125">G 分类适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="f9ea8-125">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="f9ea8-126">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="f9ea8-126">parentalGuidance</span></span>|<span data-ttu-id="f9ea8-127">5 </span><span class="sxs-lookup"><span data-stu-id="f9ea8-127">5</span></span>|<span data-ttu-id="f9ea8-128">PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="f9ea8-128">PG, Parental Guidance</span></span>|
|<span data-ttu-id="f9ea8-129">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="f9ea8-129">agesAbove14</span></span>|<span data-ttu-id="f9ea8-130">6 </span><span class="sxs-lookup"><span data-stu-id="f9ea8-130">6</span></span>|<span data-ttu-id="f9ea8-131">14 + 分类适用于14岁及更早的查看者</span><span class="sxs-lookup"><span data-stu-id="f9ea8-131">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="f9ea8-132">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="f9ea8-132">agesAbove18</span></span>|<span data-ttu-id="f9ea8-133">7 </span><span class="sxs-lookup"><span data-stu-id="f9ea8-133">7</span></span>|<span data-ttu-id="f9ea8-134">18个以上的分类适用于18岁及更早的查看者</span><span class="sxs-lookup"><span data-stu-id="f9ea8-134">The 18+ classification is intended for viewers ages 18 and older</span></span>|









