---
title: ratingIrelandTelevisionType 枚举类型
description: 在爱尔兰 TV 内容评级标签
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b357a2604479789cc85c17b0867cb56fa8cc2b3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991830"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="2eae4-103">ratingIrelandTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2eae4-103">ratingIrelandTelevisionType enum type</span></span>

> <span data-ttu-id="2eae4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2eae4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2eae4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2eae4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2eae4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2eae4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2eae4-107">在爱尔兰 TV 内容评级标签</span><span class="sxs-lookup"><span data-stu-id="2eae4-107">TV content rating labels in Ireland</span></span>
## <a name="members"></a><span data-ttu-id="2eae4-108">成员</span><span class="sxs-lookup"><span data-stu-id="2eae4-108">Members</span></span>
|<span data-ttu-id="2eae4-109">成员</span><span class="sxs-lookup"><span data-stu-id="2eae4-109">Member</span></span>|<span data-ttu-id="2eae4-110">值</span><span class="sxs-lookup"><span data-stu-id="2eae4-110">Value</span></span>|<span data-ttu-id="2eae4-111">说明</span><span class="sxs-lookup"><span data-stu-id="2eae4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eae4-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="2eae4-112">allAllowed</span></span>|<span data-ttu-id="2eae4-113">0</span><span class="sxs-lookup"><span data-stu-id="2eae4-113">0</span></span>|<span data-ttu-id="2eae4-114">默认值，允许所有 TV 都显示内容</span><span class="sxs-lookup"><span data-stu-id="2eae4-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="2eae4-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="2eae4-115">allBlocked</span></span>|<span data-ttu-id="2eae4-116">1</span><span class="sxs-lookup"><span data-stu-id="2eae4-116">1</span></span>|<span data-ttu-id="2eae4-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="2eae4-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="2eae4-118">常规</span><span class="sxs-lookup"><span data-stu-id="2eae4-118">general</span></span>|<span data-ttu-id="2eae4-119">2</span><span class="sxs-lookup"><span data-stu-id="2eae4-119">2</span></span>|<span data-ttu-id="2eae4-120">GA 分类是适用于所有访问群体</span><span class="sxs-lookup"><span data-stu-id="2eae4-120">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="2eae4-121">children</span><span class="sxs-lookup"><span data-stu-id="2eae4-121">children</span></span>|<span data-ttu-id="2eae4-122">3</span><span class="sxs-lookup"><span data-stu-id="2eae4-122">3</span></span>|<span data-ttu-id="2eae4-123">频道分类适合子级</span><span class="sxs-lookup"><span data-stu-id="2eae4-123">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="2eae4-124">youngAdults</span><span class="sxs-lookup"><span data-stu-id="2eae4-124">youngAdults</span></span>|<span data-ttu-id="2eae4-125">4</span><span class="sxs-lookup"><span data-stu-id="2eae4-125">4</span></span>|<span data-ttu-id="2eae4-126">YA 分类适合青春期访问群体</span><span class="sxs-lookup"><span data-stu-id="2eae4-126">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="2eae4-127">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="2eae4-127">parentalSupervision</span></span>|<span data-ttu-id="2eae4-128">5</span><span class="sxs-lookup"><span data-stu-id="2eae4-128">5</span></span>|<span data-ttu-id="2eae4-129">PS 分类邀请父母和监护人考虑限制子级的访问</span><span class="sxs-lookup"><span data-stu-id="2eae4-129">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="2eae4-130">成熟的</span><span class="sxs-lookup"><span data-stu-id="2eae4-130">mature</span></span>|<span data-ttu-id="2eae4-131">6</span><span class="sxs-lookup"><span data-stu-id="2eae4-131">6</span></span>|<span data-ttu-id="2eae4-132">MA 分类适合成人</span><span class="sxs-lookup"><span data-stu-id="2eae4-132">The MA classification is suitable for adults</span></span>|





