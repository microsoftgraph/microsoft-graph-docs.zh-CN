---
title: ratingGermanyTelevisionType 枚举类型
description: 德国的电视内容评级标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b7785d5ce06ccac610bfa5ae7c59cb5ebeb1b7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525927"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="71beb-103">ratingGermanyTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="71beb-103">ratingGermanyTelevisionType enum type</span></span>

<span data-ttu-id="71beb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="71beb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71beb-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71beb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71beb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71beb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71beb-107">德国的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="71beb-107">TV content rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="71beb-108">成员</span><span class="sxs-lookup"><span data-stu-id="71beb-108">Members</span></span>
|<span data-ttu-id="71beb-109">成员</span><span class="sxs-lookup"><span data-stu-id="71beb-109">Member</span></span>|<span data-ttu-id="71beb-110">值</span><span class="sxs-lookup"><span data-stu-id="71beb-110">Value</span></span>|<span data-ttu-id="71beb-111">说明</span><span class="sxs-lookup"><span data-stu-id="71beb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71beb-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="71beb-112">allAllowed</span></span>|<span data-ttu-id="71beb-113">0</span><span class="sxs-lookup"><span data-stu-id="71beb-113">0</span></span>|<span data-ttu-id="71beb-114">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="71beb-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="71beb-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="71beb-115">allBlocked</span></span>|<span data-ttu-id="71beb-116">1 </span><span class="sxs-lookup"><span data-stu-id="71beb-116">1</span></span>|<span data-ttu-id="71beb-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="71beb-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="71beb-118">概要</span><span class="sxs-lookup"><span data-stu-id="71beb-118">general</span></span>|<span data-ttu-id="71beb-119">2 </span><span class="sxs-lookup"><span data-stu-id="71beb-119">2</span></span>|<span data-ttu-id="71beb-120">Ab 0 Jahren，无期限限制</span><span class="sxs-lookup"><span data-stu-id="71beb-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="71beb-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="71beb-121">agesAbove6</span></span>|<span data-ttu-id="71beb-122">3 </span><span class="sxs-lookup"><span data-stu-id="71beb-122">3</span></span>|<span data-ttu-id="71beb-123">Ab 6 Jahren，年龄6及更早</span><span class="sxs-lookup"><span data-stu-id="71beb-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="71beb-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="71beb-124">agesAbove12</span></span>|<span data-ttu-id="71beb-125">4 </span><span class="sxs-lookup"><span data-stu-id="71beb-125">4</span></span>|<span data-ttu-id="71beb-126">Ab 12 Jahren，12岁及更早</span><span class="sxs-lookup"><span data-stu-id="71beb-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="71beb-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="71beb-127">agesAbove16</span></span>|<span data-ttu-id="71beb-128">5 </span><span class="sxs-lookup"><span data-stu-id="71beb-128">5</span></span>|<span data-ttu-id="71beb-129">Ab 16 Jahren，超过16岁及以上</span><span class="sxs-lookup"><span data-stu-id="71beb-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="71beb-130">成人</span><span class="sxs-lookup"><span data-stu-id="71beb-130">adults</span></span>|<span data-ttu-id="71beb-131">6 </span><span class="sxs-lookup"><span data-stu-id="71beb-131">6</span></span>|<span data-ttu-id="71beb-132">Ab 18 Jahren，仅成人</span><span class="sxs-lookup"><span data-stu-id="71beb-132">Ab 18 Jahren, adults only</span></span>|



