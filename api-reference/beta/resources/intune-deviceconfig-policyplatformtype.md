---
title: policyPlatformType 枚举类型
description: Suppoorted 策略的平台类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae846552b736fccd34415459a08567eb82a0d347
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566729"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="a5103-103">policyPlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a5103-103">policyPlatformType enum type</span></span>

> <span data-ttu-id="a5103-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a5103-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5103-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5103-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5103-106">Suppoorted 策略的平台类型。</span><span class="sxs-lookup"><span data-stu-id="a5103-106">Suppoorted platform types for policies.</span></span>

## <a name="members"></a><span data-ttu-id="a5103-107">成员</span><span class="sxs-lookup"><span data-stu-id="a5103-107">Members</span></span>
|<span data-ttu-id="a5103-108">成员</span><span class="sxs-lookup"><span data-stu-id="a5103-108">Member</span></span>|<span data-ttu-id="a5103-109">值</span><span class="sxs-lookup"><span data-stu-id="a5103-109">Value</span></span>|<span data-ttu-id="a5103-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5103-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5103-111">android</span><span class="sxs-lookup"><span data-stu-id="a5103-111">android</span></span>|<span data-ttu-id="a5103-112">0</span><span class="sxs-lookup"><span data-stu-id="a5103-112">0</span></span>|<span data-ttu-id="a5103-113">Android.</span><span class="sxs-lookup"><span data-stu-id="a5103-113">Android.</span></span>|
|<span data-ttu-id="a5103-114">androidForWork</span><span class="sxs-lookup"><span data-stu-id="a5103-114">androidForWork</span></span>|<span data-ttu-id="a5103-115">1</span><span class="sxs-lookup"><span data-stu-id="a5103-115">1</span></span>|<span data-ttu-id="a5103-116">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="a5103-116">AndroidForWork.</span></span>|
|<span data-ttu-id="a5103-117">iOS</span><span class="sxs-lookup"><span data-stu-id="a5103-117">iOS</span></span>|<span data-ttu-id="a5103-118">2 </span><span class="sxs-lookup"><span data-stu-id="a5103-118">2</span></span>|<span data-ttu-id="a5103-119">iOS.</span><span class="sxs-lookup"><span data-stu-id="a5103-119">iOS.</span></span>|
|<span data-ttu-id="a5103-120">macOS</span><span class="sxs-lookup"><span data-stu-id="a5103-120">macOS</span></span>|<span data-ttu-id="a5103-121">3 </span><span class="sxs-lookup"><span data-stu-id="a5103-121">3</span></span>|<span data-ttu-id="a5103-122">MacOS.</span><span class="sxs-lookup"><span data-stu-id="a5103-122">MacOS.</span></span>|
|<span data-ttu-id="a5103-123">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="a5103-123">windowsPhone81</span></span>|<span data-ttu-id="a5103-124">4 </span><span class="sxs-lookup"><span data-stu-id="a5103-124">4</span></span>|<span data-ttu-id="a5103-125">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="a5103-125">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="a5103-126">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="a5103-126">windows81AndLater</span></span>|<span data-ttu-id="a5103-127">5 </span><span class="sxs-lookup"><span data-stu-id="a5103-127">5</span></span>|<span data-ttu-id="a5103-128">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="a5103-128">Windows 8.1 and later</span></span>|
|<span data-ttu-id="a5103-129">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="a5103-129">windows10AndLater</span></span>|<span data-ttu-id="a5103-130">6 </span><span class="sxs-lookup"><span data-stu-id="a5103-130">6</span></span>|<span data-ttu-id="a5103-131">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="a5103-131">Windows 10 and later.</span></span>|
|<span data-ttu-id="a5103-132">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="a5103-132">androidWorkProfile</span></span>|<span data-ttu-id="a5103-133">7 </span><span class="sxs-lookup"><span data-stu-id="a5103-133">7</span></span>|<span data-ttu-id="a5103-134">AndroidWorkProfile.</span><span class="sxs-lookup"><span data-stu-id="a5103-134">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="a5103-135">各种</span><span class="sxs-lookup"><span data-stu-id="a5103-135">all</span></span>|<span data-ttu-id="a5103-136">100</span><span class="sxs-lookup"><span data-stu-id="a5103-136">100</span></span>|<span data-ttu-id="a5103-137">所有平台。</span><span class="sxs-lookup"><span data-stu-id="a5103-137">All platforms.</span></span>|





