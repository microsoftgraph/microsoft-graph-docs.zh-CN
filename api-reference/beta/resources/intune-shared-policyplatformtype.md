---
title: policyPlatformType 枚举类型
description: Suppoorted 策略的平台类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 16f928beefb54daa632c578d042be73c023b364c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271728"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="b4862-103">policyPlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b4862-103">policyPlatformType enum type</span></span>

<span data-ttu-id="b4862-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4862-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4862-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4862-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4862-107">Suppoorted 策略的平台类型。</span><span class="sxs-lookup"><span data-stu-id="b4862-107">Suppoorted platform types for policies.</span></span>

## <a name="members"></a><span data-ttu-id="b4862-108">成员</span><span class="sxs-lookup"><span data-stu-id="b4862-108">Members</span></span>
|<span data-ttu-id="b4862-109">成员</span><span class="sxs-lookup"><span data-stu-id="b4862-109">Member</span></span>|<span data-ttu-id="b4862-110">值</span><span class="sxs-lookup"><span data-stu-id="b4862-110">Value</span></span>|<span data-ttu-id="b4862-111">说明</span><span class="sxs-lookup"><span data-stu-id="b4862-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4862-112">android</span><span class="sxs-lookup"><span data-stu-id="b4862-112">android</span></span>|<span data-ttu-id="b4862-113">0</span><span class="sxs-lookup"><span data-stu-id="b4862-113">0</span></span>|<span data-ttu-id="b4862-114">Android.</span><span class="sxs-lookup"><span data-stu-id="b4862-114">Android.</span></span>|
|<span data-ttu-id="b4862-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="b4862-115">androidForWork</span></span>|<span data-ttu-id="b4862-116">1</span><span class="sxs-lookup"><span data-stu-id="b4862-116">1</span></span>|<span data-ttu-id="b4862-117">AndroidForWork.</span><span class="sxs-lookup"><span data-stu-id="b4862-117">AndroidForWork.</span></span>|
|<span data-ttu-id="b4862-118">iOS</span><span class="sxs-lookup"><span data-stu-id="b4862-118">iOS</span></span>|<span data-ttu-id="b4862-119">双面</span><span class="sxs-lookup"><span data-stu-id="b4862-119">2</span></span>|<span data-ttu-id="b4862-120">iOS.</span><span class="sxs-lookup"><span data-stu-id="b4862-120">iOS.</span></span>|
|<span data-ttu-id="b4862-121">macOS</span><span class="sxs-lookup"><span data-stu-id="b4862-121">macOS</span></span>|<span data-ttu-id="b4862-122">第三章</span><span class="sxs-lookup"><span data-stu-id="b4862-122">3</span></span>|<span data-ttu-id="b4862-123">MacOS.</span><span class="sxs-lookup"><span data-stu-id="b4862-123">MacOS.</span></span>|
|<span data-ttu-id="b4862-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="b4862-124">windowsPhone81</span></span>|<span data-ttu-id="b4862-125">4 </span><span class="sxs-lookup"><span data-stu-id="b4862-125">4</span></span>|<span data-ttu-id="b4862-126">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="b4862-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="b4862-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="b4862-127">windows81AndLater</span></span>|<span data-ttu-id="b4862-128">5 </span><span class="sxs-lookup"><span data-stu-id="b4862-128">5</span></span>|<span data-ttu-id="b4862-129">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="b4862-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="b4862-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="b4862-130">windows10AndLater</span></span>|<span data-ttu-id="b4862-131">6 </span><span class="sxs-lookup"><span data-stu-id="b4862-131">6</span></span>|<span data-ttu-id="b4862-132">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="b4862-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="b4862-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="b4862-133">androidWorkProfile</span></span>|<span data-ttu-id="b4862-134">7 </span><span class="sxs-lookup"><span data-stu-id="b4862-134">7</span></span>|<span data-ttu-id="b4862-135">AndroidWorkProfile.</span><span class="sxs-lookup"><span data-stu-id="b4862-135">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="b4862-136">windows10XProfile</span><span class="sxs-lookup"><span data-stu-id="b4862-136">windows10XProfile</span></span>|<span data-ttu-id="b4862-137">8 </span><span class="sxs-lookup"><span data-stu-id="b4862-137">8</span></span>|<span data-ttu-id="b4862-138">Windows10XProfile.</span><span class="sxs-lookup"><span data-stu-id="b4862-138">Windows10XProfile.</span></span>|
|<span data-ttu-id="b4862-139">各种</span><span class="sxs-lookup"><span data-stu-id="b4862-139">all</span></span>|<span data-ttu-id="b4862-140">100</span><span class="sxs-lookup"><span data-stu-id="b4862-140">100</span></span>|<span data-ttu-id="b4862-141">所有平台。</span><span class="sxs-lookup"><span data-stu-id="b4862-141">All platforms.</span></span>|




