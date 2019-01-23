---
title: ratingGermanyMoviesType 枚举类型
description: 电影分级德国的标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dfa8211b562fac95e5c325c9afe682c38e5272db
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395872"
---
# <a name="ratinggermanymoviestype-enum-type"></a><span data-ttu-id="a8133-103">ratingGermanyMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a8133-103">ratingGermanyMoviesType enum type</span></span>

> <span data-ttu-id="a8133-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a8133-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8133-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8133-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8133-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8133-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8133-107">电影分级德国的标签</span><span class="sxs-lookup"><span data-stu-id="a8133-107">Movies rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="a8133-108">成员</span><span class="sxs-lookup"><span data-stu-id="a8133-108">Members</span></span>
|<span data-ttu-id="a8133-109">成员</span><span class="sxs-lookup"><span data-stu-id="a8133-109">Member</span></span>|<span data-ttu-id="a8133-110">值</span><span class="sxs-lookup"><span data-stu-id="a8133-110">Value</span></span>|<span data-ttu-id="a8133-111">说明</span><span class="sxs-lookup"><span data-stu-id="a8133-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8133-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="a8133-112">allAllowed</span></span>|<span data-ttu-id="a8133-113">0</span><span class="sxs-lookup"><span data-stu-id="a8133-113">0</span></span>|<span data-ttu-id="a8133-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="a8133-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="a8133-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="a8133-115">allBlocked</span></span>|<span data-ttu-id="a8133-116">1</span><span class="sxs-lookup"><span data-stu-id="a8133-116">1</span></span>|<span data-ttu-id="a8133-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="a8133-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="a8133-118">常规</span><span class="sxs-lookup"><span data-stu-id="a8133-118">general</span></span>|<span data-ttu-id="a8133-119">2</span><span class="sxs-lookup"><span data-stu-id="a8133-119">2</span></span>|<span data-ttu-id="a8133-120">Ab 0 Jahren，没有期限限制</span><span class="sxs-lookup"><span data-stu-id="a8133-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="a8133-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="a8133-121">agesAbove6</span></span>|<span data-ttu-id="a8133-122">3</span><span class="sxs-lookup"><span data-stu-id="a8133-122">3</span></span>|<span data-ttu-id="a8133-123">Ab 6 Jahren 老化 6 及较早</span><span class="sxs-lookup"><span data-stu-id="a8133-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="a8133-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="a8133-124">agesAbove12</span></span>|<span data-ttu-id="a8133-125">4</span><span class="sxs-lookup"><span data-stu-id="a8133-125">4</span></span>|<span data-ttu-id="a8133-126">Ab 12 Jahren 老化 12 及较早</span><span class="sxs-lookup"><span data-stu-id="a8133-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="a8133-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="a8133-127">agesAbove16</span></span>|<span data-ttu-id="a8133-128">5</span><span class="sxs-lookup"><span data-stu-id="a8133-128">5</span></span>|<span data-ttu-id="a8133-129">Ab 16 Jahren 老化 16 及较早</span><span class="sxs-lookup"><span data-stu-id="a8133-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="a8133-130">成人</span><span class="sxs-lookup"><span data-stu-id="a8133-130">adults</span></span>|<span data-ttu-id="a8133-131">6</span><span class="sxs-lookup"><span data-stu-id="a8133-131">6</span></span>|<span data-ttu-id="a8133-132">Ab 18 Jahren，仅成人</span><span class="sxs-lookup"><span data-stu-id="a8133-132">Ab 18 Jahren, adults only</span></span>|




