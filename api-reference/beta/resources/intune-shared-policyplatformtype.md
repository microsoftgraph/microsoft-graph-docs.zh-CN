---
title: policyPlatformType 枚举类型
description: 策略支持的平台类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ad3e4a578db77fa9b2880cd7ff861cb15c6f1d9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159289"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="5cc48-103">policyPlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5cc48-103">policyPlatformType enum type</span></span>

<span data-ttu-id="5cc48-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cc48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cc48-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5cc48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cc48-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5cc48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cc48-107">策略支持的平台类型。</span><span class="sxs-lookup"><span data-stu-id="5cc48-107">Supported platform types for policies.</span></span>

## <a name="members"></a><span data-ttu-id="5cc48-108">成员</span><span class="sxs-lookup"><span data-stu-id="5cc48-108">Members</span></span>
|<span data-ttu-id="5cc48-109">成员</span><span class="sxs-lookup"><span data-stu-id="5cc48-109">Member</span></span>|<span data-ttu-id="5cc48-110">值</span><span class="sxs-lookup"><span data-stu-id="5cc48-110">Value</span></span>|<span data-ttu-id="5cc48-111">说明</span><span class="sxs-lookup"><span data-stu-id="5cc48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cc48-112">android</span><span class="sxs-lookup"><span data-stu-id="5cc48-112">android</span></span>|<span data-ttu-id="5cc48-113">0</span><span class="sxs-lookup"><span data-stu-id="5cc48-113">0</span></span>|<span data-ttu-id="5cc48-114">Android。</span><span class="sxs-lookup"><span data-stu-id="5cc48-114">Android.</span></span>|
|<span data-ttu-id="5cc48-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="5cc48-115">androidForWork</span></span>|<span data-ttu-id="5cc48-116">1</span><span class="sxs-lookup"><span data-stu-id="5cc48-116">1</span></span>|<span data-ttu-id="5cc48-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="5cc48-117">AndroidForWork.</span></span>|
|<span data-ttu-id="5cc48-118">iOS</span><span class="sxs-lookup"><span data-stu-id="5cc48-118">iOS</span></span>|<span data-ttu-id="5cc48-119">2</span><span class="sxs-lookup"><span data-stu-id="5cc48-119">2</span></span>|<span data-ttu-id="5cc48-120">iOS。</span><span class="sxs-lookup"><span data-stu-id="5cc48-120">iOS.</span></span>|
|<span data-ttu-id="5cc48-121">macOS</span><span class="sxs-lookup"><span data-stu-id="5cc48-121">macOS</span></span>|<span data-ttu-id="5cc48-122">3</span><span class="sxs-lookup"><span data-stu-id="5cc48-122">3</span></span>|<span data-ttu-id="5cc48-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="5cc48-123">MacOS.</span></span>|
|<span data-ttu-id="5cc48-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="5cc48-124">windowsPhone81</span></span>|<span data-ttu-id="5cc48-125">4 </span><span class="sxs-lookup"><span data-stu-id="5cc48-125">4</span></span>|<span data-ttu-id="5cc48-126">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="5cc48-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="5cc48-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="5cc48-127">windows81AndLater</span></span>|<span data-ttu-id="5cc48-128">5 </span><span class="sxs-lookup"><span data-stu-id="5cc48-128">5</span></span>|<span data-ttu-id="5cc48-129">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="5cc48-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="5cc48-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="5cc48-130">windows10AndLater</span></span>|<span data-ttu-id="5cc48-131">6 </span><span class="sxs-lookup"><span data-stu-id="5cc48-131">6</span></span>|<span data-ttu-id="5cc48-132">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="5cc48-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="5cc48-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="5cc48-133">androidWorkProfile</span></span>|<span data-ttu-id="5cc48-134">7 </span><span class="sxs-lookup"><span data-stu-id="5cc48-134">7</span></span>|<span data-ttu-id="5cc48-135">AndroidWorkProfile。</span><span class="sxs-lookup"><span data-stu-id="5cc48-135">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="5cc48-136">windows10XProfile</span><span class="sxs-lookup"><span data-stu-id="5cc48-136">windows10XProfile</span></span>|<span data-ttu-id="5cc48-137">8 </span><span class="sxs-lookup"><span data-stu-id="5cc48-137">8</span></span>|<span data-ttu-id="5cc48-138">Windows10XProfile。</span><span class="sxs-lookup"><span data-stu-id="5cc48-138">Windows10XProfile.</span></span>|
|<span data-ttu-id="5cc48-139">all</span><span class="sxs-lookup"><span data-stu-id="5cc48-139">all</span></span>|<span data-ttu-id="5cc48-140">100</span><span class="sxs-lookup"><span data-stu-id="5cc48-140">100</span></span>|<span data-ttu-id="5cc48-141">所有平台。</span><span class="sxs-lookup"><span data-stu-id="5cc48-141">All platforms.</span></span>|





