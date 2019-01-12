---
title: ratingAustraliaMoviesType 枚举类型
description: 电影分级中澳大利亚标签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fa54cbae04b27c7b0159ec2693cfb6a708063789
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946705"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="9f57b-103">ratingAustraliaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9f57b-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="9f57b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9f57b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f57b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9f57b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f57b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9f57b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f57b-107">电影分级中澳大利亚标签</span><span class="sxs-lookup"><span data-stu-id="9f57b-107">Movies rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="9f57b-108">成员</span><span class="sxs-lookup"><span data-stu-id="9f57b-108">Members</span></span>
|<span data-ttu-id="9f57b-109">成员</span><span class="sxs-lookup"><span data-stu-id="9f57b-109">Member</span></span>|<span data-ttu-id="9f57b-110">值</span><span class="sxs-lookup"><span data-stu-id="9f57b-110">Value</span></span>|<span data-ttu-id="9f57b-111">Description</span><span class="sxs-lookup"><span data-stu-id="9f57b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f57b-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="9f57b-112">allAllowed</span></span>|<span data-ttu-id="9f57b-113">0</span><span class="sxs-lookup"><span data-stu-id="9f57b-113">0</span></span>|<span data-ttu-id="9f57b-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="9f57b-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="9f57b-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="9f57b-115">allBlocked</span></span>|<span data-ttu-id="9f57b-116">1</span><span class="sxs-lookup"><span data-stu-id="9f57b-116">1</span></span>|<span data-ttu-id="9f57b-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="9f57b-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="9f57b-118">常规</span><span class="sxs-lookup"><span data-stu-id="9f57b-118">general</span></span>|<span data-ttu-id="9f57b-119">2</span><span class="sxs-lookup"><span data-stu-id="9f57b-119">2</span></span>|<span data-ttu-id="9f57b-120">G 分类是适用于所有人</span><span class="sxs-lookup"><span data-stu-id="9f57b-120">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="9f57b-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="9f57b-121">parentalGuidance</span></span>|<span data-ttu-id="9f57b-122">3</span><span class="sxs-lookup"><span data-stu-id="9f57b-122">3</span></span>|<span data-ttu-id="9f57b-123">PG 建议查看下的 15 与父项或监护人指南</span><span class="sxs-lookup"><span data-stu-id="9f57b-123">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="9f57b-124">成熟的</span><span class="sxs-lookup"><span data-stu-id="9f57b-124">mature</span></span>|<span data-ttu-id="9f57b-125">4</span><span class="sxs-lookup"><span data-stu-id="9f57b-125">4</span></span>|<span data-ttu-id="9f57b-126">M 分类不建议为查看者在 15</span><span class="sxs-lookup"><span data-stu-id="9f57b-126">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="9f57b-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="9f57b-127">agesAbove15</span></span>|<span data-ttu-id="9f57b-128">5</span><span class="sxs-lookup"><span data-stu-id="9f57b-128">5</span></span>|<span data-ttu-id="9f57b-129">MA15 + 分类不适用于查看在 15</span><span class="sxs-lookup"><span data-stu-id="9f57b-129">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="9f57b-130">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="9f57b-130">agesAbove18</span></span>|<span data-ttu-id="9f57b-131">6</span><span class="sxs-lookup"><span data-stu-id="9f57b-131">6</span></span>|<span data-ttu-id="9f57b-132">R18 + 分类不适用于查看下 18</span><span class="sxs-lookup"><span data-stu-id="9f57b-132">The R18+ classification is not suitable for viewers under 18</span></span>|





