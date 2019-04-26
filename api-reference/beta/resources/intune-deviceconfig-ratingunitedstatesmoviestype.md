---
title: ratingUnitedStatesMoviesType 枚举类型
description: 美国的电影评分标签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 804110ee07c85a1ca68f259e8b4ae9a206f5f29b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555225"
---
# <a name="ratingunitedstatesmoviestype-enum-type"></a><span data-ttu-id="fea8c-103">ratingUnitedStatesMoviesType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fea8c-103">ratingUnitedStatesMoviesType enum type</span></span>

> <span data-ttu-id="fea8c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fea8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fea8c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fea8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fea8c-106">美国的电影评分标签</span><span class="sxs-lookup"><span data-stu-id="fea8c-106">Movies rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="fea8c-107">成员</span><span class="sxs-lookup"><span data-stu-id="fea8c-107">Members</span></span>
|<span data-ttu-id="fea8c-108">成员</span><span class="sxs-lookup"><span data-stu-id="fea8c-108">Member</span></span>|<span data-ttu-id="fea8c-109">值</span><span class="sxs-lookup"><span data-stu-id="fea8c-109">Value</span></span>|<span data-ttu-id="fea8c-110">说明</span><span class="sxs-lookup"><span data-stu-id="fea8c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fea8c-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="fea8c-111">allAllowed</span></span>|<span data-ttu-id="fea8c-112">0</span><span class="sxs-lookup"><span data-stu-id="fea8c-112">0</span></span>|<span data-ttu-id="fea8c-113">默认值, 允许所有电影内容</span><span class="sxs-lookup"><span data-stu-id="fea8c-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="fea8c-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="fea8c-114">allBlocked</span></span>|<span data-ttu-id="fea8c-115">1</span><span class="sxs-lookup"><span data-stu-id="fea8c-115">1</span></span>|<span data-ttu-id="fea8c-116">不允许任何电影内容</span><span class="sxs-lookup"><span data-stu-id="fea8c-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="fea8c-117">概要</span><span class="sxs-lookup"><span data-stu-id="fea8c-117">general</span></span>|<span data-ttu-id="fea8c-118">2 </span><span class="sxs-lookup"><span data-stu-id="fea8c-118">2</span></span>|<span data-ttu-id="fea8c-119">G, 许可的所有年龄段</span><span class="sxs-lookup"><span data-stu-id="fea8c-119">G, all ages admitted</span></span>|
|<span data-ttu-id="fea8c-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="fea8c-120">parentalGuidance</span></span>|<span data-ttu-id="fea8c-121">3 </span><span class="sxs-lookup"><span data-stu-id="fea8c-121">3</span></span>|<span data-ttu-id="fea8c-122">PG, 某些材料可能不适用于儿童</span><span class="sxs-lookup"><span data-stu-id="fea8c-122">PG, some material may not be suitable for children</span></span>|
|<span data-ttu-id="fea8c-123">parentalGuidance13</span><span class="sxs-lookup"><span data-stu-id="fea8c-123">parentalGuidance13</span></span>|<span data-ttu-id="fea8c-124">4 </span><span class="sxs-lookup"><span data-stu-id="fea8c-124">4</span></span>|<span data-ttu-id="fea8c-125">PG13, 某些材料可能不适用于13岁以下的儿童</span><span class="sxs-lookup"><span data-stu-id="fea8c-125">PG13, some material may be inappropriate for children under 13</span></span>|
|<span data-ttu-id="fea8c-126">受限</span><span class="sxs-lookup"><span data-stu-id="fea8c-126">restricted</span></span>|<span data-ttu-id="fea8c-127">5 </span><span class="sxs-lookup"><span data-stu-id="fea8c-127">5</span></span>|<span data-ttu-id="fea8c-128">R, 17 下的查看者需要伴随父或成人监护人</span><span class="sxs-lookup"><span data-stu-id="fea8c-128">R, viewers under 17 require accompanying parent or adult guardian</span></span>|
|<span data-ttu-id="fea8c-129">成人</span><span class="sxs-lookup"><span data-stu-id="fea8c-129">adults</span></span>|<span data-ttu-id="fea8c-130">6 </span><span class="sxs-lookup"><span data-stu-id="fea8c-130">6</span></span>|<span data-ttu-id="fea8c-131">NC17, 仅成人</span><span class="sxs-lookup"><span data-stu-id="fea8c-131">NC17, adults only</span></span>|





