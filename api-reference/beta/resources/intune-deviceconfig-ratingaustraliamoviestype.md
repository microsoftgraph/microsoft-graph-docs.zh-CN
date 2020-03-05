---
title: ratingAustraliaMoviesType 枚举类型
description: 澳大利亚的电影评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ff3461620a9b94d02d2026b6d3ec2c9267e2b89c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529525"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="43475-103">ratingAustraliaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="43475-103">ratingAustraliaMoviesType enum type</span></span>

<span data-ttu-id="43475-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="43475-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43475-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43475-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43475-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43475-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43475-107">澳大利亚的电影评级标签</span><span class="sxs-lookup"><span data-stu-id="43475-107">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="43475-108">成员</span><span class="sxs-lookup"><span data-stu-id="43475-108">Members</span></span>
|<span data-ttu-id="43475-109">成员</span><span class="sxs-lookup"><span data-stu-id="43475-109">Member</span></span>|<span data-ttu-id="43475-110">值</span><span class="sxs-lookup"><span data-stu-id="43475-110">Value</span></span>|<span data-ttu-id="43475-111">说明</span><span class="sxs-lookup"><span data-stu-id="43475-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43475-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="43475-112">allAllowed</span></span>|<span data-ttu-id="43475-113">0</span><span class="sxs-lookup"><span data-stu-id="43475-113">0</span></span>|<span data-ttu-id="43475-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="43475-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="43475-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="43475-115">allBlocked</span></span>|<span data-ttu-id="43475-116">1 </span><span class="sxs-lookup"><span data-stu-id="43475-116">1</span></span>|<span data-ttu-id="43475-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="43475-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="43475-118">概要</span><span class="sxs-lookup"><span data-stu-id="43475-118">general</span></span>|<span data-ttu-id="43475-119">2 </span><span class="sxs-lookup"><span data-stu-id="43475-119">2</span></span>|<span data-ttu-id="43475-120">G 分类适用于所有人</span><span class="sxs-lookup"><span data-stu-id="43475-120">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="43475-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="43475-121">parentalGuidance</span></span>|<span data-ttu-id="43475-122">3 </span><span class="sxs-lookup"><span data-stu-id="43475-122">3</span></span>|<span data-ttu-id="43475-123">PG 推荐查看者为15的人，并提供来自家长或监护人的指导</span><span class="sxs-lookup"><span data-stu-id="43475-123">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="43475-124">成熟</span><span class="sxs-lookup"><span data-stu-id="43475-124">mature</span></span>|<span data-ttu-id="43475-125">4 </span><span class="sxs-lookup"><span data-stu-id="43475-125">4</span></span>|<span data-ttu-id="43475-126">不建议在15下对查看器使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="43475-126">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="43475-127">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="43475-127">agesAbove15</span></span>|<span data-ttu-id="43475-128">5 </span><span class="sxs-lookup"><span data-stu-id="43475-128">5</span></span>|<span data-ttu-id="43475-129">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="43475-129">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="43475-130">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="43475-130">agesAbove18</span></span>|<span data-ttu-id="43475-131">6 </span><span class="sxs-lookup"><span data-stu-id="43475-131">6</span></span>|<span data-ttu-id="43475-132">R18 + 分类不适用于18岁以上的观众</span><span class="sxs-lookup"><span data-stu-id="43475-132">The R18+ classification is not suitable for viewers under 18</span></span>|



