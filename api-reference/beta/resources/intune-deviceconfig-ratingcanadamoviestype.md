---
title: ratingCanadaMoviesType 枚举类型
description: 电影分级加拿大标签
ms.openlocfilehash: f490b785b2471fdcbd8a3e0ccc88599734197f2e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048878"
---
# <a name="ratingcanadamoviestype-enum-type"></a><span data-ttu-id="00afa-103">ratingCanadaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="00afa-103">ratingCanadaMoviesType enum type</span></span>

> <span data-ttu-id="00afa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00afa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00afa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00afa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00afa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00afa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00afa-107">电影分级加拿大标签</span><span class="sxs-lookup"><span data-stu-id="00afa-107">Movies rating labels in Canada</span></span>
## <a name="members"></a><span data-ttu-id="00afa-108">成员</span><span class="sxs-lookup"><span data-stu-id="00afa-108">Members</span></span>
|<span data-ttu-id="00afa-109">成员</span><span class="sxs-lookup"><span data-stu-id="00afa-109">Member</span></span>|<span data-ttu-id="00afa-110">值</span><span class="sxs-lookup"><span data-stu-id="00afa-110">Value</span></span>|<span data-ttu-id="00afa-111">说明</span><span class="sxs-lookup"><span data-stu-id="00afa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00afa-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="00afa-112">allAllowed</span></span>|<span data-ttu-id="00afa-113">0</span><span class="sxs-lookup"><span data-stu-id="00afa-113">0</span></span>|<span data-ttu-id="00afa-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="00afa-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="00afa-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="00afa-115">allBlocked</span></span>|<span data-ttu-id="00afa-116">1</span><span class="sxs-lookup"><span data-stu-id="00afa-116">1</span></span>|<span data-ttu-id="00afa-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="00afa-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="00afa-118">常规</span><span class="sxs-lookup"><span data-stu-id="00afa-118">general</span></span>|<span data-ttu-id="00afa-119">2</span><span class="sxs-lookup"><span data-stu-id="00afa-119">2</span></span>|<span data-ttu-id="00afa-120">G 分类是适用于所有岁</span><span class="sxs-lookup"><span data-stu-id="00afa-120">The G classification is suitable for all ages</span></span>|
|<span data-ttu-id="00afa-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="00afa-121">parentalGuidance</span></span>|<span data-ttu-id="00afa-122">3</span><span class="sxs-lookup"><span data-stu-id="00afa-122">3</span></span>|<span data-ttu-id="00afa-123">PG 分类建议家长的指南</span><span class="sxs-lookup"><span data-stu-id="00afa-123">The PG classification advises parental guidance</span></span>|
|<span data-ttu-id="00afa-124">agesAbove14</span><span class="sxs-lookup"><span data-stu-id="00afa-124">agesAbove14</span></span>|<span data-ttu-id="00afa-125">4</span><span class="sxs-lookup"><span data-stu-id="00afa-125">4</span></span>|<span data-ttu-id="00afa-126">14A 分类适于上面 14 或更低的查看者</span><span class="sxs-lookup"><span data-stu-id="00afa-126">The 14A classification is suitable for viewers above 14 or older</span></span>|
|<span data-ttu-id="00afa-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="00afa-127">agesAbove18</span></span>|<span data-ttu-id="00afa-128">5</span><span class="sxs-lookup"><span data-stu-id="00afa-128">5</span></span>|<span data-ttu-id="00afa-129">18A 分类适于上面 18 或更低的查看者</span><span class="sxs-lookup"><span data-stu-id="00afa-129">The 18A classification is suitable for viewers above 18 or older</span></span>|
|<span data-ttu-id="00afa-130">受限制</span><span class="sxs-lookup"><span data-stu-id="00afa-130">restricted</span></span>|<span data-ttu-id="00afa-131">6</span><span class="sxs-lookup"><span data-stu-id="00afa-131">6</span></span>|<span data-ttu-id="00afa-132">R 分类是限制为 18 年及较早</span><span class="sxs-lookup"><span data-stu-id="00afa-132">The R classification is restricted to 18 years and older</span></span>|





