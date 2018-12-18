---
title: ratingAustraliaMoviesType 枚举类型
description: 电影分级中澳大利亚标签
author: tfitzmac
ms.openlocfilehash: d282b4c0e58fb0fb5141068d3d59a10052c83490
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307096"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="a786a-103">ratingAustraliaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a786a-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="a786a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a786a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a786a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a786a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a786a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a786a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a786a-107">电影分级中澳大利亚标签</span><span class="sxs-lookup"><span data-stu-id="a786a-107">Movies rating labels in Australia</span></span>
## <a name="members"></a><span data-ttu-id="a786a-108">成员</span><span class="sxs-lookup"><span data-stu-id="a786a-108">Members</span></span>
|<span data-ttu-id="a786a-109">成员</span><span class="sxs-lookup"><span data-stu-id="a786a-109">Member</span></span>|<span data-ttu-id="a786a-110">值</span><span class="sxs-lookup"><span data-stu-id="a786a-110">Value</span></span>|<span data-ttu-id="a786a-111">说明</span><span class="sxs-lookup"><span data-stu-id="a786a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a786a-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="a786a-112">allAllowed</span></span>|<span data-ttu-id="a786a-113">0</span><span class="sxs-lookup"><span data-stu-id="a786a-113">0</span></span>|<span data-ttu-id="a786a-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="a786a-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="a786a-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="a786a-115">allBlocked</span></span>|<span data-ttu-id="a786a-116">1</span><span class="sxs-lookup"><span data-stu-id="a786a-116">1</span></span>|<span data-ttu-id="a786a-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="a786a-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="a786a-118">常规</span><span class="sxs-lookup"><span data-stu-id="a786a-118">general</span></span>|<span data-ttu-id="a786a-119">2</span><span class="sxs-lookup"><span data-stu-id="a786a-119">2</span></span>|<span data-ttu-id="a786a-120">G 分类是适用于所有人</span><span class="sxs-lookup"><span data-stu-id="a786a-120">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="a786a-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="a786a-121">parentalGuidance</span></span>|<span data-ttu-id="a786a-122">3</span><span class="sxs-lookup"><span data-stu-id="a786a-122">3</span></span>|<span data-ttu-id="a786a-123">PG 建议查看下的 15 与父项或监护人指南</span><span class="sxs-lookup"><span data-stu-id="a786a-123">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="a786a-124">成熟的</span><span class="sxs-lookup"><span data-stu-id="a786a-124">mature</span></span>|<span data-ttu-id="a786a-125">4</span><span class="sxs-lookup"><span data-stu-id="a786a-125">4</span></span>|<span data-ttu-id="a786a-126">M 分类不建议为查看者在 15</span><span class="sxs-lookup"><span data-stu-id="a786a-126">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="a786a-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="a786a-127">agesAbove15</span></span>|<span data-ttu-id="a786a-128">5</span><span class="sxs-lookup"><span data-stu-id="a786a-128">5</span></span>|<span data-ttu-id="a786a-129">MA15 + 分类不适用于查看在 15</span><span class="sxs-lookup"><span data-stu-id="a786a-129">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="a786a-130">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="a786a-130">agesAbove18</span></span>|<span data-ttu-id="a786a-131">6</span><span class="sxs-lookup"><span data-stu-id="a786a-131">6</span></span>|<span data-ttu-id="a786a-132">R18 + 分类不适用于查看下 18</span><span class="sxs-lookup"><span data-stu-id="a786a-132">The R18+ classification is not suitable for viewers under 18</span></span>|





