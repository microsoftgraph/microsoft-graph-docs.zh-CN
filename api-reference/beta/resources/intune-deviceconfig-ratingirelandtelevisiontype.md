---
title: ratingIrelandTelevisionType 枚举类型
description: 爱尔兰的电视内容评级标签
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0a198c98fd82e5b4f388175b244ded0cb2c9dbd2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049707"
---
# <a name="ratingirelandtelevisiontype-enum-type"></a><span data-ttu-id="22d32-103">ratingIrelandTelevisionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="22d32-103">ratingIrelandTelevisionType enum type</span></span>

<span data-ttu-id="22d32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22d32-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22d32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22d32-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22d32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22d32-107">爱尔兰的电视内容评级标签</span><span class="sxs-lookup"><span data-stu-id="22d32-107">TV content rating labels in Ireland</span></span>

## <a name="members"></a><span data-ttu-id="22d32-108">成员</span><span class="sxs-lookup"><span data-stu-id="22d32-108">Members</span></span>
|<span data-ttu-id="22d32-109">成员</span><span class="sxs-lookup"><span data-stu-id="22d32-109">Member</span></span>|<span data-ttu-id="22d32-110">值</span><span class="sxs-lookup"><span data-stu-id="22d32-110">Value</span></span>|<span data-ttu-id="22d32-111">说明</span><span class="sxs-lookup"><span data-stu-id="22d32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d32-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="22d32-112">allAllowed</span></span>|<span data-ttu-id="22d32-113">0</span><span class="sxs-lookup"><span data-stu-id="22d32-113">0</span></span>|<span data-ttu-id="22d32-114">默认值，允许所有电视节目内容</span><span class="sxs-lookup"><span data-stu-id="22d32-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="22d32-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="22d32-115">allBlocked</span></span>|<span data-ttu-id="22d32-116">1 </span><span class="sxs-lookup"><span data-stu-id="22d32-116">1</span></span>|<span data-ttu-id="22d32-117">不允许任何电视显示内容</span><span class="sxs-lookup"><span data-stu-id="22d32-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="22d32-118">概要</span><span class="sxs-lookup"><span data-stu-id="22d32-118">general</span></span>|<span data-ttu-id="22d32-119">2 </span><span class="sxs-lookup"><span data-stu-id="22d32-119">2</span></span>|<span data-ttu-id="22d32-120">GA 分类适用于所有受众</span><span class="sxs-lookup"><span data-stu-id="22d32-120">The GA classification is suitable for all audiences</span></span>|
|<span data-ttu-id="22d32-121">children</span><span class="sxs-lookup"><span data-stu-id="22d32-121">children</span></span>|<span data-ttu-id="22d32-122">第三章</span><span class="sxs-lookup"><span data-stu-id="22d32-122">3</span></span>|<span data-ttu-id="22d32-123">CH 分类适用于儿童</span><span class="sxs-lookup"><span data-stu-id="22d32-123">The CH classification is suitable for children</span></span>|
|<span data-ttu-id="22d32-124">youngAdults</span><span class="sxs-lookup"><span data-stu-id="22d32-124">youngAdults</span></span>|<span data-ttu-id="22d32-125">4 </span><span class="sxs-lookup"><span data-stu-id="22d32-125">4</span></span>|<span data-ttu-id="22d32-126">YA 分类适用于 teenage 访问群体</span><span class="sxs-lookup"><span data-stu-id="22d32-126">The YA classification is suitable for teenage audience</span></span>|
|<span data-ttu-id="22d32-127">parentalSupervision</span><span class="sxs-lookup"><span data-stu-id="22d32-127">parentalSupervision</span></span>|<span data-ttu-id="22d32-128">5 </span><span class="sxs-lookup"><span data-stu-id="22d32-128">5</span></span>|<span data-ttu-id="22d32-129">PS 分类邀请家长和监护人来考虑限制儿童的访问权限</span><span class="sxs-lookup"><span data-stu-id="22d32-129">The PS classification invites parents and guardians to consider restriction children’s access</span></span>|
|<span data-ttu-id="22d32-130">成熟</span><span class="sxs-lookup"><span data-stu-id="22d32-130">mature</span></span>|<span data-ttu-id="22d32-131">6 </span><span class="sxs-lookup"><span data-stu-id="22d32-131">6</span></span>|<span data-ttu-id="22d32-132">MA 分类适用于成年人</span><span class="sxs-lookup"><span data-stu-id="22d32-132">The MA classification is suitable for adults</span></span>|






