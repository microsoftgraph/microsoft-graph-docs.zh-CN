---
title: ratingGermanyTelevisionType 枚举类型
description: 在德国 TV 内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1f5f2a27a86151244dd7b2db3d160e8e570a61f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947664"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="12ef3-103">ratingGermanyTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="12ef3-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="12ef3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12ef3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12ef3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12ef3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12ef3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12ef3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12ef3-107">在德国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="12ef3-107">TV content rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="12ef3-108">成员</span><span class="sxs-lookup"><span data-stu-id="12ef3-108">Members</span></span>
|<span data-ttu-id="12ef3-109">成员</span><span class="sxs-lookup"><span data-stu-id="12ef3-109">Member</span></span>|<span data-ttu-id="12ef3-110">值</span><span class="sxs-lookup"><span data-stu-id="12ef3-110">Value</span></span>|<span data-ttu-id="12ef3-111">Description</span><span class="sxs-lookup"><span data-stu-id="12ef3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12ef3-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="12ef3-112">allAllowed</span></span>|<span data-ttu-id="12ef3-113">0</span><span class="sxs-lookup"><span data-stu-id="12ef3-113">0</span></span>|<span data-ttu-id="12ef3-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="12ef3-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="12ef3-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="12ef3-115">allBlocked</span></span>|<span data-ttu-id="12ef3-116">1</span><span class="sxs-lookup"><span data-stu-id="12ef3-116">1</span></span>|<span data-ttu-id="12ef3-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="12ef3-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="12ef3-118">常规</span><span class="sxs-lookup"><span data-stu-id="12ef3-118">general</span></span>|<span data-ttu-id="12ef3-119">2</span><span class="sxs-lookup"><span data-stu-id="12ef3-119">2</span></span>|<span data-ttu-id="12ef3-120">Ab 0 Jahren，没有期限限制</span><span class="sxs-lookup"><span data-stu-id="12ef3-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="12ef3-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="12ef3-121">agesAbove6</span></span>|<span data-ttu-id="12ef3-122">3</span><span class="sxs-lookup"><span data-stu-id="12ef3-122">3</span></span>|<span data-ttu-id="12ef3-123">Ab 6 Jahren 老化 6 及较早</span><span class="sxs-lookup"><span data-stu-id="12ef3-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="12ef3-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="12ef3-124">agesAbove12</span></span>|<span data-ttu-id="12ef3-125">4</span><span class="sxs-lookup"><span data-stu-id="12ef3-125">4</span></span>|<span data-ttu-id="12ef3-126">Ab 12 Jahren 老化 12 及较早</span><span class="sxs-lookup"><span data-stu-id="12ef3-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="12ef3-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="12ef3-127">agesAbove16</span></span>|<span data-ttu-id="12ef3-128">5</span><span class="sxs-lookup"><span data-stu-id="12ef3-128">5</span></span>|<span data-ttu-id="12ef3-129">Ab 16 Jahren 老化 16 及较早</span><span class="sxs-lookup"><span data-stu-id="12ef3-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="12ef3-130">成人</span><span class="sxs-lookup"><span data-stu-id="12ef3-130">adults</span></span>|<span data-ttu-id="12ef3-131">6</span><span class="sxs-lookup"><span data-stu-id="12ef3-131">6</span></span>|<span data-ttu-id="12ef3-132">Ab 18 Jahren，仅成人</span><span class="sxs-lookup"><span data-stu-id="12ef3-132">Ab 18 Jahren, adults only</span></span>|





