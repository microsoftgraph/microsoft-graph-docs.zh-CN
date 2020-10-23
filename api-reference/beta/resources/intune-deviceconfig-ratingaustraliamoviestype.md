---
title: ratingAustraliaMoviesType 枚举类型
description: 澳大利亚的电影评级标签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5485acfd815ea59c50b9c8a51980c14fe0796fb2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722892"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="ac399-103">ratingAustraliaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ac399-103">ratingAustraliaMoviesType enum type</span></span>

<span data-ttu-id="ac399-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac399-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac399-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ac399-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac399-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac399-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac399-107">澳大利亚的电影评级标签</span><span class="sxs-lookup"><span data-stu-id="ac399-107">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="ac399-108">成员</span><span class="sxs-lookup"><span data-stu-id="ac399-108">Members</span></span>
|<span data-ttu-id="ac399-109">成员</span><span class="sxs-lookup"><span data-stu-id="ac399-109">Member</span></span>|<span data-ttu-id="ac399-110">值</span><span class="sxs-lookup"><span data-stu-id="ac399-110">Value</span></span>|<span data-ttu-id="ac399-111">说明</span><span class="sxs-lookup"><span data-stu-id="ac399-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac399-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="ac399-112">allAllowed</span></span>|<span data-ttu-id="ac399-113">0</span><span class="sxs-lookup"><span data-stu-id="ac399-113">0</span></span>|<span data-ttu-id="ac399-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="ac399-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="ac399-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="ac399-115">allBlocked</span></span>|<span data-ttu-id="ac399-116">1</span><span class="sxs-lookup"><span data-stu-id="ac399-116">1</span></span>|<span data-ttu-id="ac399-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="ac399-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="ac399-118">概要</span><span class="sxs-lookup"><span data-stu-id="ac399-118">general</span></span>|<span data-ttu-id="ac399-119">双面</span><span class="sxs-lookup"><span data-stu-id="ac399-119">2</span></span>|<span data-ttu-id="ac399-120">G 分类适用于所有人</span><span class="sxs-lookup"><span data-stu-id="ac399-120">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="ac399-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="ac399-121">parentalGuidance</span></span>|<span data-ttu-id="ac399-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ac399-122">3</span></span>|<span data-ttu-id="ac399-123">PG 推荐查看者为15的人，并提供来自家长或监护人的指导</span><span class="sxs-lookup"><span data-stu-id="ac399-123">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="ac399-124">成熟</span><span class="sxs-lookup"><span data-stu-id="ac399-124">mature</span></span>|<span data-ttu-id="ac399-125">4 </span><span class="sxs-lookup"><span data-stu-id="ac399-125">4</span></span>|<span data-ttu-id="ac399-126">不建议在15下对查看器使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="ac399-126">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="ac399-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="ac399-127">agesAbove15</span></span>|<span data-ttu-id="ac399-128">5 </span><span class="sxs-lookup"><span data-stu-id="ac399-128">5</span></span>|<span data-ttu-id="ac399-129">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="ac399-129">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="ac399-130">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="ac399-130">agesAbove18</span></span>|<span data-ttu-id="ac399-131">6 </span><span class="sxs-lookup"><span data-stu-id="ac399-131">6</span></span>|<span data-ttu-id="ac399-132">R18 + 分类不适用于18岁以上的观众</span><span class="sxs-lookup"><span data-stu-id="ac399-132">The R18+ classification is not suitable for viewers under 18</span></span>|





