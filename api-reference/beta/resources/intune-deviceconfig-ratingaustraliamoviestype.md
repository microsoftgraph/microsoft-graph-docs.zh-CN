---
title: ratingAustraliaMoviesType 枚举类型
description: 澳大利亚的电影评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df09ba09db619d22de4e59a5976173df5a3daa79
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995782"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="6aa34-103">ratingAustraliaMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6aa34-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="6aa34-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6aa34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aa34-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6aa34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aa34-106">澳大利亚的电影评级标签</span><span class="sxs-lookup"><span data-stu-id="6aa34-106">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="6aa34-107">成员</span><span class="sxs-lookup"><span data-stu-id="6aa34-107">Members</span></span>
|<span data-ttu-id="6aa34-108">成员</span><span class="sxs-lookup"><span data-stu-id="6aa34-108">Member</span></span>|<span data-ttu-id="6aa34-109">值</span><span class="sxs-lookup"><span data-stu-id="6aa34-109">Value</span></span>|<span data-ttu-id="6aa34-110">说明</span><span class="sxs-lookup"><span data-stu-id="6aa34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aa34-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="6aa34-111">allAllowed</span></span>|<span data-ttu-id="6aa34-112">0</span><span class="sxs-lookup"><span data-stu-id="6aa34-112">0</span></span>|<span data-ttu-id="6aa34-113">默认值, 允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="6aa34-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="6aa34-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="6aa34-114">allBlocked</span></span>|<span data-ttu-id="6aa34-115">1</span><span class="sxs-lookup"><span data-stu-id="6aa34-115">1</span></span>|<span data-ttu-id="6aa34-116">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="6aa34-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="6aa34-117">概要</span><span class="sxs-lookup"><span data-stu-id="6aa34-117">general</span></span>|<span data-ttu-id="6aa34-118">双面</span><span class="sxs-lookup"><span data-stu-id="6aa34-118">2</span></span>|<span data-ttu-id="6aa34-119">G 分类适用于所有人</span><span class="sxs-lookup"><span data-stu-id="6aa34-119">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="6aa34-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="6aa34-120">parentalGuidance</span></span>|<span data-ttu-id="6aa34-121">第三章</span><span class="sxs-lookup"><span data-stu-id="6aa34-121">3</span></span>|<span data-ttu-id="6aa34-122">PG 推荐查看者为15的人, 并提供来自家长或监护人的指导</span><span class="sxs-lookup"><span data-stu-id="6aa34-122">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="6aa34-123">成熟</span><span class="sxs-lookup"><span data-stu-id="6aa34-123">mature</span></span>|<span data-ttu-id="6aa34-124">4</span><span class="sxs-lookup"><span data-stu-id="6aa34-124">4</span></span>|<span data-ttu-id="6aa34-125">不建议在15下对查看器使用 M 分类</span><span class="sxs-lookup"><span data-stu-id="6aa34-125">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="6aa34-126">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="6aa34-126">agesAbove15</span></span>|<span data-ttu-id="6aa34-127">5</span><span class="sxs-lookup"><span data-stu-id="6aa34-127">5</span></span>|<span data-ttu-id="6aa34-128">MA15 + 分类不适用于15岁以上的查看器</span><span class="sxs-lookup"><span data-stu-id="6aa34-128">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="6aa34-129">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="6aa34-129">agesAbove18</span></span>|<span data-ttu-id="6aa34-130">型</span><span class="sxs-lookup"><span data-stu-id="6aa34-130">6</span></span>|<span data-ttu-id="6aa34-131">R18 + 分类不适用于18岁以上的观众</span><span class="sxs-lookup"><span data-stu-id="6aa34-131">The R18+ classification is not suitable for viewers under 18</span></span>|





