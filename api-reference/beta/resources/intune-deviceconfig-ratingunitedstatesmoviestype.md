---
title: ratingUnitedStatesMoviesType 枚举类型
description: 美国的电影评分标签
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aae50d5061e2b3836801c06337678d4d5082c000
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000632"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="9f33a-103">ratingUnitedStatesMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9f33a-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="9f33a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f33a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f33a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f33a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f33a-106">美国的电影评分标签</span><span class="sxs-lookup"><span data-stu-id="9f33a-106">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="9f33a-107">成员</span><span class="sxs-lookup"><span data-stu-id="9f33a-107">Members</span></span>
|<span data-ttu-id="9f33a-108">成员</span><span class="sxs-lookup"><span data-stu-id="9f33a-108">Member</span></span>|<span data-ttu-id="9f33a-109">值</span><span class="sxs-lookup"><span data-stu-id="9f33a-109">Value</span></span>|<span data-ttu-id="9f33a-110">说明</span><span class="sxs-lookup"><span data-stu-id="9f33a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f33a-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="9f33a-111">allAllowed</span></span>|<span data-ttu-id="9f33a-112">0</span><span class="sxs-lookup"><span data-stu-id="9f33a-112">0</span></span>|<span data-ttu-id="9f33a-113">默认值, 允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="9f33a-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="9f33a-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="9f33a-114">allBlocked</span></span>|<span data-ttu-id="9f33a-115">1</span><span class="sxs-lookup"><span data-stu-id="9f33a-115">1</span></span>|<span data-ttu-id="9f33a-116">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="9f33a-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="9f33a-117">概要</span><span class="sxs-lookup"><span data-stu-id="9f33a-117">general</span></span>|<span data-ttu-id="9f33a-118">双面</span><span class="sxs-lookup"><span data-stu-id="9f33a-118">2</span></span>|<span data-ttu-id="9f33a-119">G, 许可的所有年龄段</span><span class="sxs-lookup"><span data-stu-id="9f33a-119">G, all ages admitted</span></span>|
|<span data-ttu-id="9f33a-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="9f33a-120">parentalGuidance</span></span>|<span data-ttu-id="9f33a-121">第三章</span><span class="sxs-lookup"><span data-stu-id="9f33a-121">3</span></span>|<span data-ttu-id="9f33a-122">PG, 某些材料可能不适用于儿童</span><span class="sxs-lookup"><span data-stu-id="9f33a-122">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="9f33a-123">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="9f33a-123">parentalGuidance13</span></span>|<span data-ttu-id="9f33a-124">4</span><span class="sxs-lookup"><span data-stu-id="9f33a-124">4</span></span>|<span data-ttu-id="9f33a-125">PG13, 某些材料可能不适用于13岁以下的儿童</span><span class="sxs-lookup"><span data-stu-id="9f33a-125">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="9f33a-126">受限</span><span class="sxs-lookup"><span data-stu-id="9f33a-126">restricted</span></span>|<span data-ttu-id="9f33a-127">5</span><span class="sxs-lookup"><span data-stu-id="9f33a-127">5</span></span>|<span data-ttu-id="9f33a-128">R, 17 下的查看者需要伴随父或成人监护人</span><span class="sxs-lookup"><span data-stu-id="9f33a-128">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="9f33a-129">成人</span><span class="sxs-lookup"><span data-stu-id="9f33a-129">adults</span></span>|<span data-ttu-id="9f33a-130">型</span><span class="sxs-lookup"><span data-stu-id="9f33a-130">6</span></span>|<span data-ttu-id="9f33a-131">NC17, 仅成人</span><span class="sxs-lookup"><span data-stu-id="9f33a-131">NC17, adults only</span></span>|





