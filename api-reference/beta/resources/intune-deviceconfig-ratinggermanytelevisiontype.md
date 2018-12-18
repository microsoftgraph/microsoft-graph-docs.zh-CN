---
title: ratingGermanyTelevisionType 枚举类型
description: 在德国 TV 内容评级标签
author: tfitzmac
ms.openlocfilehash: 4e619682d37dce6612624213de232893aa986694
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345358"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="f29b7-103">ratingGermanyTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f29b7-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="f29b7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f29b7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f29b7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f29b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f29b7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f29b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f29b7-107">在德国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="f29b7-107">TV content rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="f29b7-108">成员</span><span class="sxs-lookup"><span data-stu-id="f29b7-108">Members</span></span>
|<span data-ttu-id="f29b7-109">成员</span><span class="sxs-lookup"><span data-stu-id="f29b7-109">Member</span></span>|<span data-ttu-id="f29b7-110">值</span><span class="sxs-lookup"><span data-stu-id="f29b7-110">Value</span></span>|<span data-ttu-id="f29b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="f29b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f29b7-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f29b7-112">allAllowed</span></span>|<span data-ttu-id="f29b7-113">0</span><span class="sxs-lookup"><span data-stu-id="f29b7-113">0</span></span>|<span data-ttu-id="f29b7-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="f29b7-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="f29b7-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f29b7-115">allBlocked</span></span>|<span data-ttu-id="f29b7-116">1</span><span class="sxs-lookup"><span data-stu-id="f29b7-116">1</span></span>|<span data-ttu-id="f29b7-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="f29b7-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="f29b7-118">常规</span><span class="sxs-lookup"><span data-stu-id="f29b7-118">general</span></span>|<span data-ttu-id="f29b7-119">2</span><span class="sxs-lookup"><span data-stu-id="f29b7-119">2</span></span>|<span data-ttu-id="f29b7-120">Ab 0 Jahren，没有期限限制</span><span class="sxs-lookup"><span data-stu-id="f29b7-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="f29b7-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="f29b7-121">agesAbove6</span></span>|<span data-ttu-id="f29b7-122">3</span><span class="sxs-lookup"><span data-stu-id="f29b7-122">3</span></span>|<span data-ttu-id="f29b7-123">Ab 6 Jahren 老化 6 及较早</span><span class="sxs-lookup"><span data-stu-id="f29b7-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="f29b7-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="f29b7-124">agesAbove12</span></span>|<span data-ttu-id="f29b7-125">4</span><span class="sxs-lookup"><span data-stu-id="f29b7-125">4</span></span>|<span data-ttu-id="f29b7-126">Ab 12 Jahren 老化 12 及较早</span><span class="sxs-lookup"><span data-stu-id="f29b7-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="f29b7-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="f29b7-127">agesAbove16</span></span>|<span data-ttu-id="f29b7-128">5</span><span class="sxs-lookup"><span data-stu-id="f29b7-128">5</span></span>|<span data-ttu-id="f29b7-129">Ab 16 Jahren 老化 16 及较早</span><span class="sxs-lookup"><span data-stu-id="f29b7-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="f29b7-130">成人</span><span class="sxs-lookup"><span data-stu-id="f29b7-130">adults</span></span>|<span data-ttu-id="f29b7-131">6</span><span class="sxs-lookup"><span data-stu-id="f29b7-131">6</span></span>|<span data-ttu-id="f29b7-132">Ab 18 Jahren，仅成人</span><span class="sxs-lookup"><span data-stu-id="f29b7-132">Ab 18 Jahren, adults only</span></span>|





