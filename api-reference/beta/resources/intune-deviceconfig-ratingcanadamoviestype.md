---
title: ratingCanadaMoviesType 枚举类型
description: 加拿大的电影评分标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f8b77afa68bfd27e50e96f6463aa64b8c7d88ad0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529516"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="dbf77-103">ratingCanadaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dbf77-103">ratingCanadaMoviesType enum type</span></span>

<span data-ttu-id="dbf77-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dbf77-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbf77-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dbf77-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbf77-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dbf77-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbf77-107">加拿大的电影评分标签</span><span class="sxs-lookup"><span data-stu-id="dbf77-107">Movies rating labels in Canada</span></span>

## <a name="members"></a><span data-ttu-id="dbf77-108">成员</span><span class="sxs-lookup"><span data-stu-id="dbf77-108">Members</span></span>
|<span data-ttu-id="dbf77-109">成员</span><span class="sxs-lookup"><span data-stu-id="dbf77-109">Member</span></span>|<span data-ttu-id="dbf77-110">值</span><span class="sxs-lookup"><span data-stu-id="dbf77-110">Value</span></span>|<span data-ttu-id="dbf77-111">说明</span><span class="sxs-lookup"><span data-stu-id="dbf77-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbf77-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="dbf77-112">allAllowed</span></span>|<span data-ttu-id="dbf77-113">0</span><span class="sxs-lookup"><span data-stu-id="dbf77-113">0</span></span>|<span data-ttu-id="dbf77-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="dbf77-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="dbf77-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="dbf77-115">allBlocked</span></span>|<span data-ttu-id="dbf77-116">1 </span><span class="sxs-lookup"><span data-stu-id="dbf77-116">1</span></span>|<span data-ttu-id="dbf77-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="dbf77-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="dbf77-118">概要</span><span class="sxs-lookup"><span data-stu-id="dbf77-118">general</span></span>|<span data-ttu-id="dbf77-119">2 </span><span class="sxs-lookup"><span data-stu-id="dbf77-119">2</span></span>|<span data-ttu-id="dbf77-120">G 分类适用于所有年龄段</span><span class="sxs-lookup"><span data-stu-id="dbf77-120">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="dbf77-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="dbf77-121">parentalGuidance</span></span>|<span data-ttu-id="dbf77-122">3 </span><span class="sxs-lookup"><span data-stu-id="dbf77-122">3</span></span>|<span data-ttu-id="dbf77-123">PG 分类建议家长指导</span><span class="sxs-lookup"><span data-stu-id="dbf77-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="dbf77-124">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="dbf77-124">agesAbove14</span></span>|<span data-ttu-id="dbf77-125">4 </span><span class="sxs-lookup"><span data-stu-id="dbf77-125">4</span></span>|<span data-ttu-id="dbf77-126">14A 分类适用于14岁以上或更早的观众</span><span class="sxs-lookup"><span data-stu-id="dbf77-126">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="dbf77-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="dbf77-127">agesAbove18</span></span>|<span data-ttu-id="dbf77-128">5 </span><span class="sxs-lookup"><span data-stu-id="dbf77-128">5</span></span>|<span data-ttu-id="dbf77-129">18A 分类适用于18岁以上或更早的观众</span><span class="sxs-lookup"><span data-stu-id="dbf77-129">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="dbf77-130">受限</span><span class="sxs-lookup"><span data-stu-id="dbf77-130">restricted</span></span>|<span data-ttu-id="dbf77-131">6 </span><span class="sxs-lookup"><span data-stu-id="dbf77-131">6</span></span>|<span data-ttu-id="dbf77-132">R 分类限制为18年和更早</span><span class="sxs-lookup"><span data-stu-id="dbf77-132">The R classification is restricted to 18 years and older</span></span>|



