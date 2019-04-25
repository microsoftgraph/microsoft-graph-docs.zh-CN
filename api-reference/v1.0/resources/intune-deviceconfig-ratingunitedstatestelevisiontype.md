---
title: ratingUnitedStatesTelevisionType 枚举类型
description: 美国的电视内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86ee28f600ae9f1e55f09d3d7db794fd55c79281
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534750"
---
# <a name="ratingunitedstatestelevisiontype-enum-type"></a><span data-ttu-id="0fc22-103">ratingUnitedStatesTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0fc22-103">ratingUnitedStatesTelevisionType enum type</span></span>

> <span data-ttu-id="0fc22-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fc22-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fc22-105">美国的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="0fc22-105">TV content rating labels in United States</span></span>

## <a name="members"></a><span data-ttu-id="0fc22-106">成员</span><span class="sxs-lookup"><span data-stu-id="0fc22-106">Members</span></span>
|<span data-ttu-id="0fc22-107">成员</span><span class="sxs-lookup"><span data-stu-id="0fc22-107">Member</span></span>|<span data-ttu-id="0fc22-108">值</span><span class="sxs-lookup"><span data-stu-id="0fc22-108">Value</span></span>|<span data-ttu-id="0fc22-109">说明</span><span class="sxs-lookup"><span data-stu-id="0fc22-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc22-110">allAllowed</span><span class="sxs-lookup"><span data-stu-id="0fc22-110">allAllowed</span></span>|<span data-ttu-id="0fc22-111">0</span><span class="sxs-lookup"><span data-stu-id="0fc22-111">0</span></span>|<span data-ttu-id="0fc22-112">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="0fc22-112">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="0fc22-113">allBlocked</span><span class="sxs-lookup"><span data-stu-id="0fc22-113">allBlocked</span></span>|<span data-ttu-id="0fc22-114">1</span><span class="sxs-lookup"><span data-stu-id="0fc22-114">1</span></span>|<span data-ttu-id="0fc22-115">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="0fc22-115">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="0fc22-116">childrenAll</span><span class="sxs-lookup"><span data-stu-id="0fc22-116">childrenAll</span></span>|<span data-ttu-id="0fc22-117">2 </span><span class="sxs-lookup"><span data-stu-id="0fc22-117">2</span></span>|<span data-ttu-id="0fc22-118">TV-Y, 所有子项</span><span class="sxs-lookup"><span data-stu-id="0fc22-118">TV-Y, all children</span></span>|
|<span data-ttu-id="0fc22-119">childrenAbove7</span><span class="sxs-lookup"><span data-stu-id="0fc22-119">childrenAbove7</span></span>|<span data-ttu-id="0fc22-120">3 </span><span class="sxs-lookup"><span data-stu-id="0fc22-120">3</span></span>|<span data-ttu-id="0fc22-121">电视-Y7, 儿童年龄7及更高版本</span><span class="sxs-lookup"><span data-stu-id="0fc22-121">TV-Y7, children age 7 and above</span></span>|
|<span data-ttu-id="0fc22-122">概要</span><span class="sxs-lookup"><span data-stu-id="0fc22-122">general</span></span>|<span data-ttu-id="0fc22-123">4 </span><span class="sxs-lookup"><span data-stu-id="0fc22-123">4</span></span>|<span data-ttu-id="0fc22-124">TV-G, 适用于所有年龄</span><span class="sxs-lookup"><span data-stu-id="0fc22-124">TV-G, suitable for all ages</span></span>|
|<span data-ttu-id="0fc22-125">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="0fc22-125">parentalGuidance</span></span>|<span data-ttu-id="0fc22-126">5 </span><span class="sxs-lookup"><span data-stu-id="0fc22-126">5</span></span>|<span data-ttu-id="0fc22-127">TV PG、家长指导</span><span class="sxs-lookup"><span data-stu-id="0fc22-127">TV-PG, parental guidance</span></span>|
|<span data-ttu-id="0fc22-128">childrenAbove14</span><span class="sxs-lookup"><span data-stu-id="0fc22-128">childrenAbove14</span></span>|<span data-ttu-id="0fc22-129">6 </span><span class="sxs-lookup"><span data-stu-id="0fc22-129">6</span></span>|<span data-ttu-id="0fc22-130">电视-14, 儿童年龄14及更高版本</span><span class="sxs-lookup"><span data-stu-id="0fc22-130">TV-14, children age 14 and above</span></span>|
|<span data-ttu-id="0fc22-131">成人</span><span class="sxs-lookup"><span data-stu-id="0fc22-131">adults</span></span>|<span data-ttu-id="0fc22-132">7 </span><span class="sxs-lookup"><span data-stu-id="0fc22-132">7</span></span>|<span data-ttu-id="0fc22-133">仅限成人的电视-MA</span><span class="sxs-lookup"><span data-stu-id="0fc22-133">TV-MA, adults only</span></span>|



