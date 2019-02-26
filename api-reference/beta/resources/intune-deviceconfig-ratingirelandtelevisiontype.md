---
title: ratingIrelandTelevisionType 枚举类型
description: 爱尔兰的电视内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d186659ff2e67217c8d4c6f3b449925907822a11
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172462"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="f19c0-103">ratingIrelandTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f19c0-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="f19c0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f19c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f19c0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f19c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f19c0-106">爱尔兰的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="f19c0-106">TV content rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="f19c0-107">成员</span><span class="sxs-lookup"><span data-stu-id="f19c0-107">Members</span></span>
|<span data-ttu-id="f19c0-108">成员</span><span class="sxs-lookup"><span data-stu-id="f19c0-108">Member</span></span>|<span data-ttu-id="f19c0-109">值</span><span class="sxs-lookup"><span data-stu-id="f19c0-109">Value</span></span>|<span data-ttu-id="f19c0-110">说明</span><span class="sxs-lookup"><span data-stu-id="f19c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f19c0-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f19c0-111">allAllowed</span></span>|<span data-ttu-id="f19c0-112">0</span><span class="sxs-lookup"><span data-stu-id="f19c0-112">0</span></span>|<span data-ttu-id="f19c0-113">默认值, 允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="f19c0-113">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="f19c0-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f19c0-114">allBlocked</span></span>|<span data-ttu-id="f19c0-115">1</span><span class="sxs-lookup"><span data-stu-id="f19c0-115">1</span></span>|<span data-ttu-id="f19c0-116">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="f19c0-116">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="f19c0-117">概要</span><span class="sxs-lookup"><span data-stu-id="f19c0-117">general</span></span>|<span data-ttu-id="f19c0-118">双面</span><span class="sxs-lookup"><span data-stu-id="f19c0-118">2</span></span>|<span data-ttu-id="f19c0-119">GA 分类适用于所有受众</span><span class="sxs-lookup"><span data-stu-id="f19c0-119">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="f19c0-120">children</span><span class="sxs-lookup"><span data-stu-id="f19c0-120">children</span></span>|<span data-ttu-id="f19c0-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f19c0-121">3</span></span>|<span data-ttu-id="f19c0-122">CH 分类适用于儿童</span><span class="sxs-lookup"><span data-stu-id="f19c0-122">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="f19c0-123">youngAdults</span><span class="sxs-lookup"><span data-stu-id="f19c0-123">youngAdults</span></span>|<span data-ttu-id="f19c0-124">4</span><span class="sxs-lookup"><span data-stu-id="f19c0-124">4</span></span>|<span data-ttu-id="f19c0-125">YA 分类适用于 teenage 访问群体</span><span class="sxs-lookup"><span data-stu-id="f19c0-125">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="f19c0-126">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="f19c0-126">parentalSupervision</span></span>|<span data-ttu-id="f19c0-127">5</span><span class="sxs-lookup"><span data-stu-id="f19c0-127">5</span></span>|<span data-ttu-id="f19c0-128">PS 分类邀请家长和监护人来考虑限制儿童的访问权限</span><span class="sxs-lookup"><span data-stu-id="f19c0-128">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="f19c0-129">成熟</span><span class="sxs-lookup"><span data-stu-id="f19c0-129">mature</span></span>|<span data-ttu-id="f19c0-130">型</span><span class="sxs-lookup"><span data-stu-id="f19c0-130">6</span></span>|<span data-ttu-id="f19c0-131">MA 分类适用于成年人</span><span class="sxs-lookup"><span data-stu-id="f19c0-131">The MA classification is suitable for adults</span></span>|




