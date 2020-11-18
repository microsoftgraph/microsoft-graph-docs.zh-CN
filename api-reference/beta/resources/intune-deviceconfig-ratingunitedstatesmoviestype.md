---
title: ratingUnitedStatesMoviesType 枚举类型
description: 美国的电影评分标签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e8d3fe75f394279acdbd74489ac39041c4a47254
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198358"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="648e7-103">ratingUnitedStatesMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="648e7-103">ratingUnitedStatesMoviesType enum type</span></span>

<span data-ttu-id="648e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="648e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="648e7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="648e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="648e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="648e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="648e7-107">美国的电影评分标签</span><span class="sxs-lookup"><span data-stu-id="648e7-107">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="648e7-108">成员</span><span class="sxs-lookup"><span data-stu-id="648e7-108">Members</span></span>
|<span data-ttu-id="648e7-109">成员</span><span class="sxs-lookup"><span data-stu-id="648e7-109">Member</span></span>|<span data-ttu-id="648e7-110">值</span><span class="sxs-lookup"><span data-stu-id="648e7-110">Value</span></span>|<span data-ttu-id="648e7-111">说明</span><span class="sxs-lookup"><span data-stu-id="648e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="648e7-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="648e7-112">allAllowed</span></span>|<span data-ttu-id="648e7-113">0</span><span class="sxs-lookup"><span data-stu-id="648e7-113">0</span></span>|<span data-ttu-id="648e7-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="648e7-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="648e7-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="648e7-115">allBlocked</span></span>|<span data-ttu-id="648e7-116">1</span><span class="sxs-lookup"><span data-stu-id="648e7-116">1</span></span>|<span data-ttu-id="648e7-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="648e7-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="648e7-118">概要</span><span class="sxs-lookup"><span data-stu-id="648e7-118">general</span></span>|<span data-ttu-id="648e7-119">双面</span><span class="sxs-lookup"><span data-stu-id="648e7-119">2</span></span>|<span data-ttu-id="648e7-120">G，许可的所有年龄段</span><span class="sxs-lookup"><span data-stu-id="648e7-120">G, all ages admitted</span></span>|
|<span data-ttu-id="648e7-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="648e7-121">parentalGuidance</span></span>|<span data-ttu-id="648e7-122">第三章</span><span class="sxs-lookup"><span data-stu-id="648e7-122">3</span></span>|<span data-ttu-id="648e7-123">PG，某些材料可能不适用于儿童</span><span class="sxs-lookup"><span data-stu-id="648e7-123">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="648e7-124">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="648e7-124">parentalGuidance13</span></span>|<span data-ttu-id="648e7-125">4 </span><span class="sxs-lookup"><span data-stu-id="648e7-125">4</span></span>|<span data-ttu-id="648e7-126">PG13，某些材料可能不适用于13岁以下的儿童</span><span class="sxs-lookup"><span data-stu-id="648e7-126">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="648e7-127">受限</span><span class="sxs-lookup"><span data-stu-id="648e7-127">restricted</span></span>|<span data-ttu-id="648e7-128">5 </span><span class="sxs-lookup"><span data-stu-id="648e7-128">5</span></span>|<span data-ttu-id="648e7-129">R，17下的查看者需要伴随父或成人监护人</span><span class="sxs-lookup"><span data-stu-id="648e7-129">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="648e7-130">成人</span><span class="sxs-lookup"><span data-stu-id="648e7-130">adults</span></span>|<span data-ttu-id="648e7-131">6 </span><span class="sxs-lookup"><span data-stu-id="648e7-131">6</span></span>|<span data-ttu-id="648e7-132">NC17，仅成人</span><span class="sxs-lookup"><span data-stu-id="648e7-132">NC17, adults only</span></span>|




