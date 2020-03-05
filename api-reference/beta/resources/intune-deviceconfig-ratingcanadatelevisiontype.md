---
title: ratingCanadaTelevisionType 枚举类型
description: 加拿大的电视内容评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5bf11f21cec3f75c1aa15c051e2bd1400ce5ac44
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525941"
---
# <a name="ratingcanadatelevisiontype-enum-type"></a><span data-ttu-id="eb81e-103">ratingCanadaTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="eb81e-103">ratingCanadaTelevisionType enum type</span></span>

<span data-ttu-id="eb81e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="eb81e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb81e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb81e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb81e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb81e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb81e-107">加拿大的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="eb81e-107">TV content rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="eb81e-108">成员</span><span class="sxs-lookup"><span data-stu-id="eb81e-108">Members</span></span>
|<span data-ttu-id="eb81e-109">成员</span><span class="sxs-lookup"><span data-stu-id="eb81e-109">Member</span></span>|<span data-ttu-id="eb81e-110">值</span><span class="sxs-lookup"><span data-stu-id="eb81e-110">Value</span></span>|<span data-ttu-id="eb81e-111">说明</span><span class="sxs-lookup"><span data-stu-id="eb81e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb81e-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="eb81e-112">allAllowed</span></span>|<span data-ttu-id="eb81e-113">0</span><span class="sxs-lookup"><span data-stu-id="eb81e-113">0</span></span>|<span data-ttu-id="eb81e-114">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="eb81e-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="eb81e-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="eb81e-115">allBlocked</span></span>|<span data-ttu-id="eb81e-116">1 </span><span class="sxs-lookup"><span data-stu-id="eb81e-116">1</span></span>|<span data-ttu-id="eb81e-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="eb81e-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="eb81e-118">children</span><span class="sxs-lookup"><span data-stu-id="eb81e-118">children</span></span>|<span data-ttu-id="eb81e-119">2 </span><span class="sxs-lookup"><span data-stu-id="eb81e-119">2</span></span>|<span data-ttu-id="eb81e-120">C 分类适用于2到7年的儿童年龄</span><span class="sxs-lookup"><span data-stu-id="eb81e-120">The C classification is suitable for children ages of 2 to 7 years</span></span>|
|<span data-ttu-id="eb81e-121">childrenAbove8</span><span class="sxs-lookup"><span data-stu-id="eb81e-121">childrenAbove8</span></span>|<span data-ttu-id="eb81e-122">3 </span><span class="sxs-lookup"><span data-stu-id="eb81e-122">3</span></span>|<span data-ttu-id="eb81e-123">C8 分类适用于仅有8岁以上的儿童</span><span class="sxs-lookup"><span data-stu-id="eb81e-123">The C8 classification is suitable for children ages 8+</span></span>|
|<span data-ttu-id="eb81e-124">概要</span><span class="sxs-lookup"><span data-stu-id="eb81e-124">general</span></span>|<span data-ttu-id="eb81e-125">4 </span><span class="sxs-lookup"><span data-stu-id="eb81e-125">4</span></span>|<span data-ttu-id="eb81e-126">G 分类适用于常规访问群体</span><span class="sxs-lookup"><span data-stu-id="eb81e-126">The G classification is suitable for general audience</span></span>|
|<span data-ttu-id="eb81e-127">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="eb81e-127">parentalGuidance</span></span>|<span data-ttu-id="eb81e-128">5 </span><span class="sxs-lookup"><span data-stu-id="eb81e-128">5</span></span>|<span data-ttu-id="eb81e-129">PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="eb81e-129">PG, Parental Guidance</span></span>|
|<span data-ttu-id="eb81e-130">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="eb81e-130">agesAbove14</span></span>|<span data-ttu-id="eb81e-131">6 </span><span class="sxs-lookup"><span data-stu-id="eb81e-131">6</span></span>|<span data-ttu-id="eb81e-132">14 + 分类适用于14岁及更早的查看者</span><span class="sxs-lookup"><span data-stu-id="eb81e-132">The 14+ classification is intended for viewers ages 14 and older</span></span>|
|<span data-ttu-id="eb81e-133">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="eb81e-133">agesAbove18</span></span>|<span data-ttu-id="eb81e-134">7 </span><span class="sxs-lookup"><span data-stu-id="eb81e-134">7</span></span>|<span data-ttu-id="eb81e-135">18个以上的分类适用于18岁及更早的查看者</span><span class="sxs-lookup"><span data-stu-id="eb81e-135">The 18+ classification is intended for viewers ages 18 and older</span></span>|



