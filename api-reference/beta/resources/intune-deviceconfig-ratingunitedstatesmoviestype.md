---
title: ratingUnitedStatesMoviesType 枚举类型
description: 电影分级美国的标签
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 22861c0b05fc6a3dacbf520d03ee04b516dad3e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887841"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="3c213-103">ratingUnitedStatesMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3c213-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="3c213-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3c213-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c213-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3c213-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c213-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3c213-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c213-107">电影分级美国的标签</span><span class="sxs-lookup"><span data-stu-id="3c213-107">Movies rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="3c213-108">成员</span><span class="sxs-lookup"><span data-stu-id="3c213-108">Members</span></span>
|<span data-ttu-id="3c213-109">成员</span><span class="sxs-lookup"><span data-stu-id="3c213-109">Member</span></span>|<span data-ttu-id="3c213-110">值</span><span class="sxs-lookup"><span data-stu-id="3c213-110">Value</span></span>|<span data-ttu-id="3c213-111">Description</span><span class="sxs-lookup"><span data-stu-id="3c213-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c213-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="3c213-112">allAllowed</span></span>|<span data-ttu-id="3c213-113">0</span><span class="sxs-lookup"><span data-stu-id="3c213-113">0</span></span>|<span data-ttu-id="3c213-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="3c213-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="3c213-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="3c213-115">allBlocked</span></span>|<span data-ttu-id="3c213-116">1</span><span class="sxs-lookup"><span data-stu-id="3c213-116">1</span></span>|<span data-ttu-id="3c213-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="3c213-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="3c213-118">常规</span><span class="sxs-lookup"><span data-stu-id="3c213-118">general</span></span>|<span data-ttu-id="3c213-119">2</span><span class="sxs-lookup"><span data-stu-id="3c213-119">2</span></span>|<span data-ttu-id="3c213-120">G、 获准加入会议的所有岁</span><span class="sxs-lookup"><span data-stu-id="3c213-120">G, all ages admitted</span></span>|
|<span data-ttu-id="3c213-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="3c213-121">parentalGuidance</span></span>|<span data-ttu-id="3c213-122">3</span><span class="sxs-lookup"><span data-stu-id="3c213-122">3</span></span>|<span data-ttu-id="3c213-123">PG，一些材料可能不适合子级</span><span class="sxs-lookup"><span data-stu-id="3c213-123">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="3c213-124">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="3c213-124">parentalGuidance13</span></span>|<span data-ttu-id="3c213-125">4</span><span class="sxs-lookup"><span data-stu-id="3c213-125">4</span></span>|<span data-ttu-id="3c213-126">PG13，一些材料可能不适合子级下 13</span><span class="sxs-lookup"><span data-stu-id="3c213-126">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="3c213-127">受限制</span><span class="sxs-lookup"><span data-stu-id="3c213-127">restricted</span></span>|<span data-ttu-id="3c213-128">5</span><span class="sxs-lookup"><span data-stu-id="3c213-128">5</span></span>|<span data-ttu-id="3c213-129">R，查看下 17 需要随附父或成人指导</span><span class="sxs-lookup"><span data-stu-id="3c213-129">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="3c213-130">成人</span><span class="sxs-lookup"><span data-stu-id="3c213-130">adults</span></span>|<span data-ttu-id="3c213-131">6</span><span class="sxs-lookup"><span data-stu-id="3c213-131">6</span></span>|<span data-ttu-id="3c213-132">NC17，仅成人</span><span class="sxs-lookup"><span data-stu-id="3c213-132">NC17, adults only</span></span>|





