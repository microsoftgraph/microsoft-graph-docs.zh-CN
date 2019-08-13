---
title: ratingAustraliaMoviesType 枚举类型
description: 澳大利亚的电影评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 638c87c8ae9175f63efe7cb9e91db72ab11edd8a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368371"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="a6dc8-103">ratingAustraliaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a6dc8-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="a6dc8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6dc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6dc8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6dc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6dc8-106">澳大利亚的电影评级标签</span><span class="sxs-lookup"><span data-stu-id="a6dc8-106">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="a6dc8-107">成员</span><span class="sxs-lookup"><span data-stu-id="a6dc8-107">Members</span></span>
|<span data-ttu-id="a6dc8-108">成员</span><span class="sxs-lookup"><span data-stu-id="a6dc8-108">Member</span></span>|<span data-ttu-id="a6dc8-109">值</span><span class="sxs-lookup"><span data-stu-id="a6dc8-109">Value</span></span>|<span data-ttu-id="a6dc8-110">说明</span><span class="sxs-lookup"><span data-stu-id="a6dc8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6dc8-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="a6dc8-111">allAllowed</span></span>|<span data-ttu-id="a6dc8-112">0</span><span class="sxs-lookup"><span data-stu-id="a6dc8-112">0</span></span>|<span data-ttu-id="a6dc8-113">默认值, 允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="a6dc8-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="a6dc8-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="a6dc8-114">allBlocked</span></span>|<span data-ttu-id="a6dc8-115">1</span><span class="sxs-lookup"><span data-stu-id="a6dc8-115">1</span></span>|<span data-ttu-id="a6dc8-116">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="a6dc8-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="a6dc8-117">概要</span><span class="sxs-lookup"><span data-stu-id="a6dc8-117">general</span></span>|<span data-ttu-id="a6dc8-118">双面</span><span class="sxs-lookup"><span data-stu-id="a6dc8-118">2</span></span>|<span data-ttu-id="a6dc8-119">G 分类适用于所有人</span><span class="sxs-lookup"><span data-stu-id="a6dc8-119">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="a6dc8-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="a6dc8-120">parentalGuidance</span></span>|<span data-ttu-id="a6dc8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="a6dc8-121">3</span></span>|<span data-ttu-id="a6dc8-122">PG 推荐查看者为15的人, 并提供来自家长或监护人的指导</span><span class="sxs-lookup"><span data-stu-id="a6dc8-122">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="a6dc8-123">成熟</span><span class="sxs-lookup"><span data-stu-id="a6dc8-123">mature</span></span>|<span data-ttu-id="a6dc8-124">4</span><span class="sxs-lookup"><span data-stu-id="a6dc8-124">4</span></span>|<span data-ttu-id="a6dc8-125">不建议在15下对查看器使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="a6dc8-125">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="a6dc8-126">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="a6dc8-126">agesAbove15</span></span>|<span data-ttu-id="a6dc8-127">5</span><span class="sxs-lookup"><span data-stu-id="a6dc8-127">5</span></span>|<span data-ttu-id="a6dc8-128">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="a6dc8-128">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="a6dc8-129">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="a6dc8-129">agesAbove18</span></span>|<span data-ttu-id="a6dc8-130">型</span><span class="sxs-lookup"><span data-stu-id="a6dc8-130">6</span></span>|<span data-ttu-id="a6dc8-131">R18 + 分类不适用于18岁以上的观众</span><span class="sxs-lookup"><span data-stu-id="a6dc8-131">The R18+ classification is not suitable for viewers under 18</span></span>|



