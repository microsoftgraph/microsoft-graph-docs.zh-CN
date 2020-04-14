---
title: ratingGermanyMoviesType 枚举类型
description: 德国的电影评分标签
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d45b1328f3a08adb5925e2b582707b24fd1d7be4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445084"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="18d60-103">ratingGermanyMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="18d60-103">ratingGermanyMoviesType enum type</span></span>

<span data-ttu-id="18d60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18d60-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18d60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18d60-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18d60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d60-107">德国的电影评分标签</span><span class="sxs-lookup"><span data-stu-id="18d60-107">Movies rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="18d60-108">成员</span><span class="sxs-lookup"><span data-stu-id="18d60-108">Members</span></span>
|<span data-ttu-id="18d60-109">成员</span><span class="sxs-lookup"><span data-stu-id="18d60-109">Member</span></span>|<span data-ttu-id="18d60-110">值</span><span class="sxs-lookup"><span data-stu-id="18d60-110">Value</span></span>|<span data-ttu-id="18d60-111">说明</span><span class="sxs-lookup"><span data-stu-id="18d60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d60-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="18d60-112">allAllowed</span></span>|<span data-ttu-id="18d60-113">0</span><span class="sxs-lookup"><span data-stu-id="18d60-113">0</span></span>|<span data-ttu-id="18d60-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="18d60-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="18d60-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="18d60-115">allBlocked</span></span>|<span data-ttu-id="18d60-116">1</span><span class="sxs-lookup"><span data-stu-id="18d60-116">1</span></span>|<span data-ttu-id="18d60-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="18d60-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="18d60-118">概要</span><span class="sxs-lookup"><span data-stu-id="18d60-118">general</span></span>|<span data-ttu-id="18d60-119">双面</span><span class="sxs-lookup"><span data-stu-id="18d60-119">2</span></span>|<span data-ttu-id="18d60-120">Ab 0 Jahren，无期限限制</span><span class="sxs-lookup"><span data-stu-id="18d60-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="18d60-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="18d60-121">agesAbove6</span></span>|<span data-ttu-id="18d60-122">第三章</span><span class="sxs-lookup"><span data-stu-id="18d60-122">3</span></span>|<span data-ttu-id="18d60-123">Ab 6 Jahren，年龄6及更早</span><span class="sxs-lookup"><span data-stu-id="18d60-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="18d60-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="18d60-124">agesAbove12</span></span>|<span data-ttu-id="18d60-125">4 </span><span class="sxs-lookup"><span data-stu-id="18d60-125">4</span></span>|<span data-ttu-id="18d60-126">Ab 12 Jahren，12岁及更早</span><span class="sxs-lookup"><span data-stu-id="18d60-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="18d60-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="18d60-127">agesAbove16</span></span>|<span data-ttu-id="18d60-128">5 </span><span class="sxs-lookup"><span data-stu-id="18d60-128">5</span></span>|<span data-ttu-id="18d60-129">Ab 16 Jahren，超过16岁及以上</span><span class="sxs-lookup"><span data-stu-id="18d60-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="18d60-130">成人</span><span class="sxs-lookup"><span data-stu-id="18d60-130">adults</span></span>|<span data-ttu-id="18d60-131">6 </span><span class="sxs-lookup"><span data-stu-id="18d60-131">6</span></span>|<span data-ttu-id="18d60-132">Ab 18 Jahren，仅成人</span><span class="sxs-lookup"><span data-stu-id="18d60-132">Ab 18 Jahren, adults only</span></span>|



