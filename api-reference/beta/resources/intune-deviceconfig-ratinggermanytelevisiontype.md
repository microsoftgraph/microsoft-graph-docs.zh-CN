---
title: ratingGermanyTelevisionType 枚举类型
description: 在德国 TV 内容评级标签
ms.openlocfilehash: 615ccc0fbd0d155a4db9c1dc25e6478d916448a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041947"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="84d7c-103">ratingGermanyTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="84d7c-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="84d7c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="84d7c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84d7c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="84d7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84d7c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="84d7c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84d7c-107">在德国 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="84d7c-107">TV content rating labels in Germany</span></span>
## <a name="members"></a><span data-ttu-id="84d7c-108">成员</span><span class="sxs-lookup"><span data-stu-id="84d7c-108">Members</span></span>
|<span data-ttu-id="84d7c-109">成员</span><span class="sxs-lookup"><span data-stu-id="84d7c-109">Member</span></span>|<span data-ttu-id="84d7c-110">值</span><span class="sxs-lookup"><span data-stu-id="84d7c-110">Value</span></span>|<span data-ttu-id="84d7c-111">说明</span><span class="sxs-lookup"><span data-stu-id="84d7c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84d7c-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="84d7c-112">allAllowed</span></span>|<span data-ttu-id="84d7c-113">0</span><span class="sxs-lookup"><span data-stu-id="84d7c-113">0</span></span>|<span data-ttu-id="84d7c-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="84d7c-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="84d7c-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="84d7c-115">allBlocked</span></span>|<span data-ttu-id="84d7c-116">1</span><span class="sxs-lookup"><span data-stu-id="84d7c-116">1</span></span>|<span data-ttu-id="84d7c-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="84d7c-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="84d7c-118">常规</span><span class="sxs-lookup"><span data-stu-id="84d7c-118">general</span></span>|<span data-ttu-id="84d7c-119">2</span><span class="sxs-lookup"><span data-stu-id="84d7c-119">2</span></span>|<span data-ttu-id="84d7c-120">Ab 0 Jahren，没有期限限制</span><span class="sxs-lookup"><span data-stu-id="84d7c-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="84d7c-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="84d7c-121">agesAbove6</span></span>|<span data-ttu-id="84d7c-122">3</span><span class="sxs-lookup"><span data-stu-id="84d7c-122">3</span></span>|<span data-ttu-id="84d7c-123">Ab 6 Jahren 老化 6 及较早</span><span class="sxs-lookup"><span data-stu-id="84d7c-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="84d7c-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="84d7c-124">agesAbove12</span></span>|<span data-ttu-id="84d7c-125">4</span><span class="sxs-lookup"><span data-stu-id="84d7c-125">4</span></span>|<span data-ttu-id="84d7c-126">Ab 12 Jahren 老化 12 及较早</span><span class="sxs-lookup"><span data-stu-id="84d7c-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="84d7c-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="84d7c-127">agesAbove16</span></span>|<span data-ttu-id="84d7c-128">5</span><span class="sxs-lookup"><span data-stu-id="84d7c-128">5</span></span>|<span data-ttu-id="84d7c-129">Ab 16 Jahren 老化 16 及较早</span><span class="sxs-lookup"><span data-stu-id="84d7c-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="84d7c-130">成人</span><span class="sxs-lookup"><span data-stu-id="84d7c-130">adults</span></span>|<span data-ttu-id="84d7c-131">6</span><span class="sxs-lookup"><span data-stu-id="84d7c-131">6</span></span>|<span data-ttu-id="84d7c-132">Ab 18 Jahren，仅成人</span><span class="sxs-lookup"><span data-stu-id="84d7c-132">Ab 18 Jahren, adults only</span></span>|





