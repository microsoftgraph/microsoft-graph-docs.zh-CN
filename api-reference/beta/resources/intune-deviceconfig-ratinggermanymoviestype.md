---
title: ratingGermanyMoviesType 枚举类型
description: 电影分级德国的标签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8806461969b5bea7957d5be75722181654de9097
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922002"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="4189b-103">ratingGermanyMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4189b-103">ratingGermanyMoviesType enum type</span></span>

> <span data-ttu-id="4189b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4189b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4189b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4189b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4189b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4189b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4189b-107">电影分级德国的标签</span><span class="sxs-lookup"><span data-stu-id="4189b-107">Movies rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="4189b-108">成员</span><span class="sxs-lookup"><span data-stu-id="4189b-108">Members</span></span>
|<span data-ttu-id="4189b-109">成员</span><span class="sxs-lookup"><span data-stu-id="4189b-109">Member</span></span>|<span data-ttu-id="4189b-110">值</span><span class="sxs-lookup"><span data-stu-id="4189b-110">Value</span></span>|<span data-ttu-id="4189b-111">说明</span><span class="sxs-lookup"><span data-stu-id="4189b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4189b-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="4189b-112">allAllowed</span></span>|<span data-ttu-id="4189b-113">0</span><span class="sxs-lookup"><span data-stu-id="4189b-113">0</span></span>|<span data-ttu-id="4189b-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="4189b-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="4189b-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="4189b-115">allBlocked</span></span>|<span data-ttu-id="4189b-116">1</span><span class="sxs-lookup"><span data-stu-id="4189b-116">1</span></span>|<span data-ttu-id="4189b-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="4189b-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="4189b-118">常规</span><span class="sxs-lookup"><span data-stu-id="4189b-118">general</span></span>|<span data-ttu-id="4189b-119">2</span><span class="sxs-lookup"><span data-stu-id="4189b-119">2</span></span>|<span data-ttu-id="4189b-120">Ab 0 Jahren，没有期限限制</span><span class="sxs-lookup"><span data-stu-id="4189b-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="4189b-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="4189b-121">agesAbove6</span></span>|<span data-ttu-id="4189b-122">3</span><span class="sxs-lookup"><span data-stu-id="4189b-122">3</span></span>|<span data-ttu-id="4189b-123">Ab 6 Jahren 老化 6 及较早</span><span class="sxs-lookup"><span data-stu-id="4189b-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="4189b-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="4189b-124">agesAbove12</span></span>|<span data-ttu-id="4189b-125">4</span><span class="sxs-lookup"><span data-stu-id="4189b-125">4</span></span>|<span data-ttu-id="4189b-126">Ab 12 Jahren 老化 12 及较早</span><span class="sxs-lookup"><span data-stu-id="4189b-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="4189b-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="4189b-127">agesAbove16</span></span>|<span data-ttu-id="4189b-128">5</span><span class="sxs-lookup"><span data-stu-id="4189b-128">5</span></span>|<span data-ttu-id="4189b-129">Ab 16 Jahren 老化 16 及较早</span><span class="sxs-lookup"><span data-stu-id="4189b-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="4189b-130">成人</span><span class="sxs-lookup"><span data-stu-id="4189b-130">adults</span></span>|<span data-ttu-id="4189b-131">6</span><span class="sxs-lookup"><span data-stu-id="4189b-131">6</span></span>|<span data-ttu-id="4189b-132">Ab 18 Jahren，仅成人</span><span class="sxs-lookup"><span data-stu-id="4189b-132">Ab 18 Jahren, adults only</span></span>|





