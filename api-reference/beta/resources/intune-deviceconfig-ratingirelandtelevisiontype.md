---
title: ratingIrelandTelevisionType 枚举类型
description: 在爱尔兰 TV 内容评级标签
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8177ea18d5a8f840daf8f13c0493288fad342285
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394633"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="80f6f-103">ratingIrelandTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="80f6f-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="80f6f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="80f6f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80f6f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80f6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80f6f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80f6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80f6f-107">在爱尔兰 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="80f6f-107">TV content rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="80f6f-108">成员</span><span class="sxs-lookup"><span data-stu-id="80f6f-108">Members</span></span>
|<span data-ttu-id="80f6f-109">成员</span><span class="sxs-lookup"><span data-stu-id="80f6f-109">Member</span></span>|<span data-ttu-id="80f6f-110">值</span><span class="sxs-lookup"><span data-stu-id="80f6f-110">Value</span></span>|<span data-ttu-id="80f6f-111">说明</span><span class="sxs-lookup"><span data-stu-id="80f6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80f6f-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="80f6f-112">allAllowed</span></span>|<span data-ttu-id="80f6f-113">0</span><span class="sxs-lookup"><span data-stu-id="80f6f-113">0</span></span>|<span data-ttu-id="80f6f-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="80f6f-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="80f6f-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="80f6f-115">allBlocked</span></span>|<span data-ttu-id="80f6f-116">1</span><span class="sxs-lookup"><span data-stu-id="80f6f-116">1</span></span>|<span data-ttu-id="80f6f-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="80f6f-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="80f6f-118">常规</span><span class="sxs-lookup"><span data-stu-id="80f6f-118">general</span></span>|<span data-ttu-id="80f6f-119">2</span><span class="sxs-lookup"><span data-stu-id="80f6f-119">2</span></span>|<span data-ttu-id="80f6f-120">GA 分类是适用于所有访问群体</span><span class="sxs-lookup"><span data-stu-id="80f6f-120">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="80f6f-121">children</span><span class="sxs-lookup"><span data-stu-id="80f6f-121">children</span></span>|<span data-ttu-id="80f6f-122">3</span><span class="sxs-lookup"><span data-stu-id="80f6f-122">3</span></span>|<span data-ttu-id="80f6f-123">频道分类适合子级</span><span class="sxs-lookup"><span data-stu-id="80f6f-123">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="80f6f-124">youngAdults</span><span class="sxs-lookup"><span data-stu-id="80f6f-124">youngAdults</span></span>|<span data-ttu-id="80f6f-125">4</span><span class="sxs-lookup"><span data-stu-id="80f6f-125">4</span></span>|<span data-ttu-id="80f6f-126">YA 分类适合青春期访问群体</span><span class="sxs-lookup"><span data-stu-id="80f6f-126">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="80f6f-127">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="80f6f-127">parentalSupervision</span></span>|<span data-ttu-id="80f6f-128">5</span><span class="sxs-lookup"><span data-stu-id="80f6f-128">5</span></span>|<span data-ttu-id="80f6f-129">PS 分类邀请父母和监护人考虑限制子级的访问</span><span class="sxs-lookup"><span data-stu-id="80f6f-129">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="80f6f-130">成熟的</span><span class="sxs-lookup"><span data-stu-id="80f6f-130">mature</span></span>|<span data-ttu-id="80f6f-131">6</span><span class="sxs-lookup"><span data-stu-id="80f6f-131">6</span></span>|<span data-ttu-id="80f6f-132">MA 分类适合成人</span><span class="sxs-lookup"><span data-stu-id="80f6f-132">The MA classification is suitable for adults</span></span>|




