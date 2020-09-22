---
title: ratingAustraliaMoviesType 枚举类型
description: 澳大利亚的电影评级标签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5da509794ef3597892441e3186c6ba7a8fd1f68f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997261"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="3f26f-103">ratingAustraliaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3f26f-103">ratingAustraliaMoviesType enum type</span></span>

<span data-ttu-id="3f26f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f26f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f26f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f26f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f26f-106">澳大利亚的电影评级标签</span><span class="sxs-lookup"><span data-stu-id="3f26f-106">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="3f26f-107">成员</span><span class="sxs-lookup"><span data-stu-id="3f26f-107">Members</span></span>
|<span data-ttu-id="3f26f-108">成员</span><span class="sxs-lookup"><span data-stu-id="3f26f-108">Member</span></span>|<span data-ttu-id="3f26f-109">值</span><span class="sxs-lookup"><span data-stu-id="3f26f-109">Value</span></span>|<span data-ttu-id="3f26f-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f26f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f26f-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="3f26f-111">allAllowed</span></span>|<span data-ttu-id="3f26f-112">0</span><span class="sxs-lookup"><span data-stu-id="3f26f-112">0</span></span>|<span data-ttu-id="3f26f-113">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="3f26f-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="3f26f-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="3f26f-114">allBlocked</span></span>|<span data-ttu-id="3f26f-115">1 </span><span class="sxs-lookup"><span data-stu-id="3f26f-115">1</span></span>|<span data-ttu-id="3f26f-116">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="3f26f-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="3f26f-117">概要</span><span class="sxs-lookup"><span data-stu-id="3f26f-117">general</span></span>|<span data-ttu-id="3f26f-118">2 </span><span class="sxs-lookup"><span data-stu-id="3f26f-118">2</span></span>|<span data-ttu-id="3f26f-119">G 分类适用于所有人</span><span class="sxs-lookup"><span data-stu-id="3f26f-119">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="3f26f-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="3f26f-120">parentalGuidance</span></span>|<span data-ttu-id="3f26f-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3f26f-121">3</span></span>|<span data-ttu-id="3f26f-122">PG 推荐查看者为15的人，并提供来自家长或监护人的指导</span><span class="sxs-lookup"><span data-stu-id="3f26f-122">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="3f26f-123">成熟</span><span class="sxs-lookup"><span data-stu-id="3f26f-123">mature</span></span>|<span data-ttu-id="3f26f-124">4 </span><span class="sxs-lookup"><span data-stu-id="3f26f-124">4</span></span>|<span data-ttu-id="3f26f-125">不建议在15下对查看器使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="3f26f-125">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="3f26f-126">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="3f26f-126">agesAbove15</span></span>|<span data-ttu-id="3f26f-127">5 </span><span class="sxs-lookup"><span data-stu-id="3f26f-127">5</span></span>|<span data-ttu-id="3f26f-128">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="3f26f-128">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="3f26f-129">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="3f26f-129">agesAbove18</span></span>|<span data-ttu-id="3f26f-130">6 </span><span class="sxs-lookup"><span data-stu-id="3f26f-130">6</span></span>|<span data-ttu-id="3f26f-131">R18 + 分类不适用于18岁以上的观众</span><span class="sxs-lookup"><span data-stu-id="3f26f-131">The R18+ classification is not suitable for viewers under 18</span></span>|









