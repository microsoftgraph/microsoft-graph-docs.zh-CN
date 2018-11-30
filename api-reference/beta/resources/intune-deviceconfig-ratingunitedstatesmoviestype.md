---
title: ratingUnitedStatesMoviesType 枚举类型
description: 电影分级美国的标签
ms.openlocfilehash: a281f9c2d50a4f2b960e98422501e73c256fc6ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042842"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="6c8f9-103">ratingUnitedStatesMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6c8f9-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="6c8f9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6c8f9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c8f9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c8f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c8f9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6c8f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c8f9-107">电影分级美国的标签</span><span class="sxs-lookup"><span data-stu-id="6c8f9-107">Movies rating labels in United States</span></span>
## <a name="members"></a><span data-ttu-id="6c8f9-108">成员</span><span class="sxs-lookup"><span data-stu-id="6c8f9-108">Members</span></span>
|<span data-ttu-id="6c8f9-109">成员</span><span class="sxs-lookup"><span data-stu-id="6c8f9-109">Member</span></span>|<span data-ttu-id="6c8f9-110">值</span><span class="sxs-lookup"><span data-stu-id="6c8f9-110">Value</span></span>|<span data-ttu-id="6c8f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="6c8f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c8f9-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="6c8f9-112">allAllowed</span></span>|<span data-ttu-id="6c8f9-113">0</span><span class="sxs-lookup"><span data-stu-id="6c8f9-113">0</span></span>|<span data-ttu-id="6c8f9-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="6c8f9-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="6c8f9-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="6c8f9-115">allBlocked</span></span>|<span data-ttu-id="6c8f9-116">1</span><span class="sxs-lookup"><span data-stu-id="6c8f9-116">1</span></span>|<span data-ttu-id="6c8f9-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="6c8f9-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="6c8f9-118">常规</span><span class="sxs-lookup"><span data-stu-id="6c8f9-118">general</span></span>|<span data-ttu-id="6c8f9-119">2</span><span class="sxs-lookup"><span data-stu-id="6c8f9-119">2</span></span>|<span data-ttu-id="6c8f9-120">G、 获准加入会议的所有岁</span><span class="sxs-lookup"><span data-stu-id="6c8f9-120">G, all ages admitted</span></span>|
|<span data-ttu-id="6c8f9-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="6c8f9-121">parentalGuidance</span></span>|<span data-ttu-id="6c8f9-122">3</span><span class="sxs-lookup"><span data-stu-id="6c8f9-122">3</span></span>|<span data-ttu-id="6c8f9-123">PG，一些材料可能不适合子级</span><span class="sxs-lookup"><span data-stu-id="6c8f9-123">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="6c8f9-124">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="6c8f9-124">parentalGuidance13</span></span>|<span data-ttu-id="6c8f9-125">4</span><span class="sxs-lookup"><span data-stu-id="6c8f9-125">4</span></span>|<span data-ttu-id="6c8f9-126">PG13，一些材料可能不适合子级下 13</span><span class="sxs-lookup"><span data-stu-id="6c8f9-126">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="6c8f9-127">受限制</span><span class="sxs-lookup"><span data-stu-id="6c8f9-127">restricted</span></span>|<span data-ttu-id="6c8f9-128">5</span><span class="sxs-lookup"><span data-stu-id="6c8f9-128">5</span></span>|<span data-ttu-id="6c8f9-129">R，查看下 17 需要随附父或成人指导</span><span class="sxs-lookup"><span data-stu-id="6c8f9-129">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="6c8f9-130">成人</span><span class="sxs-lookup"><span data-stu-id="6c8f9-130">adults</span></span>|<span data-ttu-id="6c8f9-131">6</span><span class="sxs-lookup"><span data-stu-id="6c8f9-131">6</span></span>|<span data-ttu-id="6c8f9-132">NC17，仅成人</span><span class="sxs-lookup"><span data-stu-id="6c8f9-132">NC17, adults only</span></span>|





