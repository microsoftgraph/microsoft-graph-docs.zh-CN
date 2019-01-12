---
title: policyPlatformType 枚举类型
description: 策略升高平台类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0eef91313b308824b4e2395efb8e7aa95cf0c1ac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919305"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="c701a-103">policyPlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c701a-103">policyPlatformType enum type</span></span>

> <span data-ttu-id="c701a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c701a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c701a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c701a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c701a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c701a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c701a-107">策略升高平台类型。</span><span class="sxs-lookup"><span data-stu-id="c701a-107">Suppoorted platform types for policies.</span></span>
## <a name="members"></a><span data-ttu-id="c701a-108">成员</span><span class="sxs-lookup"><span data-stu-id="c701a-108">Members</span></span>
|<span data-ttu-id="c701a-109">成员</span><span class="sxs-lookup"><span data-stu-id="c701a-109">Member</span></span>|<span data-ttu-id="c701a-110">值</span><span class="sxs-lookup"><span data-stu-id="c701a-110">Value</span></span>|<span data-ttu-id="c701a-111">说明</span><span class="sxs-lookup"><span data-stu-id="c701a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c701a-112">android</span><span class="sxs-lookup"><span data-stu-id="c701a-112">android</span></span>|<span data-ttu-id="c701a-113">0</span><span class="sxs-lookup"><span data-stu-id="c701a-113">0</span></span>|<span data-ttu-id="c701a-114">Android。</span><span class="sxs-lookup"><span data-stu-id="c701a-114">Android.</span></span>|
|<span data-ttu-id="c701a-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="c701a-115">androidForWork</span></span>|<span data-ttu-id="c701a-116">1</span><span class="sxs-lookup"><span data-stu-id="c701a-116">1</span></span>|<span data-ttu-id="c701a-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="c701a-117">AndroidForWork.</span></span>|
|<span data-ttu-id="c701a-118">iOS</span><span class="sxs-lookup"><span data-stu-id="c701a-118">iOS</span></span>|<span data-ttu-id="c701a-119">2</span><span class="sxs-lookup"><span data-stu-id="c701a-119">2</span></span>|<span data-ttu-id="c701a-120">iOS。</span><span class="sxs-lookup"><span data-stu-id="c701a-120">iOS.</span></span>|
|<span data-ttu-id="c701a-121">macOS</span><span class="sxs-lookup"><span data-stu-id="c701a-121">macOS</span></span>|<span data-ttu-id="c701a-122">3</span><span class="sxs-lookup"><span data-stu-id="c701a-122">3</span></span>|<span data-ttu-id="c701a-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="c701a-123">MacOS.</span></span>|
|<span data-ttu-id="c701a-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="c701a-124">windowsPhone81</span></span>|<span data-ttu-id="c701a-125">4</span><span class="sxs-lookup"><span data-stu-id="c701a-125">4</span></span>|<span data-ttu-id="c701a-126">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="c701a-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="c701a-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="c701a-127">windows81AndLater</span></span>|<span data-ttu-id="c701a-128">5</span><span class="sxs-lookup"><span data-stu-id="c701a-128">5</span></span>|<span data-ttu-id="c701a-129">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="c701a-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="c701a-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="c701a-130">windows10AndLater</span></span>|<span data-ttu-id="c701a-131">6</span><span class="sxs-lookup"><span data-stu-id="c701a-131">6</span></span>|<span data-ttu-id="c701a-132">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="c701a-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="c701a-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="c701a-133">androidWorkProfile</span></span>|<span data-ttu-id="c701a-134">7</span><span class="sxs-lookup"><span data-stu-id="c701a-134">7</span></span>|<span data-ttu-id="c701a-135">AndroidWorkProfile。</span><span class="sxs-lookup"><span data-stu-id="c701a-135">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="c701a-136">all</span><span class="sxs-lookup"><span data-stu-id="c701a-136">all</span></span>|<span data-ttu-id="c701a-137">100</span><span class="sxs-lookup"><span data-stu-id="c701a-137">100</span></span>|<span data-ttu-id="c701a-138">所有平台。</span><span class="sxs-lookup"><span data-stu-id="c701a-138">All platforms.</span></span>|





