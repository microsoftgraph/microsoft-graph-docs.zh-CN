---
title: ratingUnitedStatesMoviesType 枚举类型
description: 电影分级美国的标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c14fcc87c949e3f16403ca4654ec987423f8b647
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412224"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="72c04-103">ratingUnitedStatesMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="72c04-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="72c04-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="72c04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72c04-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="72c04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72c04-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72c04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72c04-107">电影分级美国的标签</span><span class="sxs-lookup"><span data-stu-id="72c04-107">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="72c04-108">成员</span><span class="sxs-lookup"><span data-stu-id="72c04-108">Members</span></span>
|<span data-ttu-id="72c04-109">成员</span><span class="sxs-lookup"><span data-stu-id="72c04-109">Member</span></span>|<span data-ttu-id="72c04-110">值</span><span class="sxs-lookup"><span data-stu-id="72c04-110">Value</span></span>|<span data-ttu-id="72c04-111">说明</span><span class="sxs-lookup"><span data-stu-id="72c04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72c04-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="72c04-112">allAllowed</span></span>|<span data-ttu-id="72c04-113">0</span><span class="sxs-lookup"><span data-stu-id="72c04-113">0</span></span>|<span data-ttu-id="72c04-114">默认值，允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="72c04-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="72c04-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="72c04-115">allBlocked</span></span>|<span data-ttu-id="72c04-116">1</span><span class="sxs-lookup"><span data-stu-id="72c04-116">1</span></span>|<span data-ttu-id="72c04-117">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="72c04-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="72c04-118">常规</span><span class="sxs-lookup"><span data-stu-id="72c04-118">general</span></span>|<span data-ttu-id="72c04-119">2</span><span class="sxs-lookup"><span data-stu-id="72c04-119">2</span></span>|<span data-ttu-id="72c04-120">G、 获准加入会议的所有岁</span><span class="sxs-lookup"><span data-stu-id="72c04-120">G, all ages admitted</span></span>|
|<span data-ttu-id="72c04-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="72c04-121">parentalGuidance</span></span>|<span data-ttu-id="72c04-122">3</span><span class="sxs-lookup"><span data-stu-id="72c04-122">3</span></span>|<span data-ttu-id="72c04-123">PG，一些材料可能不适合子级</span><span class="sxs-lookup"><span data-stu-id="72c04-123">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="72c04-124">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="72c04-124">parentalGuidance13</span></span>|<span data-ttu-id="72c04-125">4</span><span class="sxs-lookup"><span data-stu-id="72c04-125">4</span></span>|<span data-ttu-id="72c04-126">PG13，一些材料可能不适合子级下 13</span><span class="sxs-lookup"><span data-stu-id="72c04-126">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="72c04-127">受限制</span><span class="sxs-lookup"><span data-stu-id="72c04-127">restricted</span></span>|<span data-ttu-id="72c04-128">5</span><span class="sxs-lookup"><span data-stu-id="72c04-128">5</span></span>|<span data-ttu-id="72c04-129">R，查看下 17 需要随附父或成人指导</span><span class="sxs-lookup"><span data-stu-id="72c04-129">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="72c04-130">成人</span><span class="sxs-lookup"><span data-stu-id="72c04-130">adults</span></span>|<span data-ttu-id="72c04-131">6</span><span class="sxs-lookup"><span data-stu-id="72c04-131">6</span></span>|<span data-ttu-id="72c04-132">NC17，仅成人</span><span class="sxs-lookup"><span data-stu-id="72c04-132">NC17, adults only</span></span>|




