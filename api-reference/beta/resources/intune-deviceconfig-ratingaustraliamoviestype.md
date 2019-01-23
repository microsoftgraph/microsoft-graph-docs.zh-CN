---
title: ratingAustraliaMoviesType 枚举类型
description: 电影分级中澳大利亚标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ee94e37275d0a97729ea3de12264067ecf1e2d3d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408409"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="9961b-103">ratingAustraliaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9961b-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="9961b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9961b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9961b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9961b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9961b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9961b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9961b-107">电影分级中澳大利亚标签</span><span class="sxs-lookup"><span data-stu-id="9961b-107">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="9961b-108">成员</span><span class="sxs-lookup"><span data-stu-id="9961b-108">Members</span></span>
|<span data-ttu-id="9961b-109">成员</span><span class="sxs-lookup"><span data-stu-id="9961b-109">Member</span></span>|<span data-ttu-id="9961b-110">值</span><span class="sxs-lookup"><span data-stu-id="9961b-110">Value</span></span>|<span data-ttu-id="9961b-111">说明</span><span class="sxs-lookup"><span data-stu-id="9961b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9961b-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="9961b-112">allAllowed</span></span>|<span data-ttu-id="9961b-113">0</span><span class="sxs-lookup"><span data-stu-id="9961b-113">0</span></span>|<span data-ttu-id="9961b-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="9961b-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="9961b-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="9961b-115">allBlocked</span></span>|<span data-ttu-id="9961b-116">1</span><span class="sxs-lookup"><span data-stu-id="9961b-116">1</span></span>|<span data-ttu-id="9961b-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="9961b-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="9961b-118">常规</span><span class="sxs-lookup"><span data-stu-id="9961b-118">general</span></span>|<span data-ttu-id="9961b-119">2</span><span class="sxs-lookup"><span data-stu-id="9961b-119">2</span></span>|<span data-ttu-id="9961b-120">G 分类是适用于所有人</span><span class="sxs-lookup"><span data-stu-id="9961b-120">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="9961b-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="9961b-121">parentalGuidance</span></span>|<span data-ttu-id="9961b-122">3</span><span class="sxs-lookup"><span data-stu-id="9961b-122">3</span></span>|<span data-ttu-id="9961b-123">PG 建议查看下的 15 与父项或监护人指南</span><span class="sxs-lookup"><span data-stu-id="9961b-123">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="9961b-124">成熟的</span><span class="sxs-lookup"><span data-stu-id="9961b-124">mature</span></span>|<span data-ttu-id="9961b-125">4</span><span class="sxs-lookup"><span data-stu-id="9961b-125">4</span></span>|<span data-ttu-id="9961b-126">M 分类不建议为查看者在 15</span><span class="sxs-lookup"><span data-stu-id="9961b-126">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="9961b-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="9961b-127">agesAbove15</span></span>|<span data-ttu-id="9961b-128">5</span><span class="sxs-lookup"><span data-stu-id="9961b-128">5</span></span>|<span data-ttu-id="9961b-129">MA15 + 分类不适用于查看在 15</span><span class="sxs-lookup"><span data-stu-id="9961b-129">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="9961b-130">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="9961b-130">agesAbove18</span></span>|<span data-ttu-id="9961b-131">6</span><span class="sxs-lookup"><span data-stu-id="9961b-131">6</span></span>|<span data-ttu-id="9961b-132">R18 + 分类不适用于查看下 18</span><span class="sxs-lookup"><span data-stu-id="9961b-132">The R18+ classification is not suitable for viewers under 18</span></span>|




