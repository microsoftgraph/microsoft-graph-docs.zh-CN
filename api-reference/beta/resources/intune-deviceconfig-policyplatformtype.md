---
title: policyPlatformType 枚举类型
description: 策略升高平台类型。
author: tfitzmac
ms.openlocfilehash: c36551393be37f2087c64d03a323ff82a5e6e037
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323945"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="d453d-103">policyPlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d453d-103">policyPlatformType enum type</span></span>

> <span data-ttu-id="d453d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d453d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d453d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d453d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d453d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d453d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d453d-107">策略升高平台类型。</span><span class="sxs-lookup"><span data-stu-id="d453d-107">Suppoorted platform types for policies.</span></span>
## <a name="members"></a><span data-ttu-id="d453d-108">成员</span><span class="sxs-lookup"><span data-stu-id="d453d-108">Members</span></span>
|<span data-ttu-id="d453d-109">成员</span><span class="sxs-lookup"><span data-stu-id="d453d-109">Member</span></span>|<span data-ttu-id="d453d-110">值</span><span class="sxs-lookup"><span data-stu-id="d453d-110">Value</span></span>|<span data-ttu-id="d453d-111">说明</span><span class="sxs-lookup"><span data-stu-id="d453d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d453d-112">android</span><span class="sxs-lookup"><span data-stu-id="d453d-112">android</span></span>|<span data-ttu-id="d453d-113">0</span><span class="sxs-lookup"><span data-stu-id="d453d-113">0</span></span>|<span data-ttu-id="d453d-114">Android。</span><span class="sxs-lookup"><span data-stu-id="d453d-114">Android.</span></span>|
|<span data-ttu-id="d453d-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="d453d-115">androidForWork</span></span>|<span data-ttu-id="d453d-116">1</span><span class="sxs-lookup"><span data-stu-id="d453d-116">1</span></span>|<span data-ttu-id="d453d-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="d453d-117">AndroidForWork.</span></span>|
|<span data-ttu-id="d453d-118">iOS</span><span class="sxs-lookup"><span data-stu-id="d453d-118">iOS</span></span>|<span data-ttu-id="d453d-119">2</span><span class="sxs-lookup"><span data-stu-id="d453d-119">2</span></span>|<span data-ttu-id="d453d-120">iOS。</span><span class="sxs-lookup"><span data-stu-id="d453d-120">iOS.</span></span>|
|<span data-ttu-id="d453d-121">macOS</span><span class="sxs-lookup"><span data-stu-id="d453d-121">macOS</span></span>|<span data-ttu-id="d453d-122">3</span><span class="sxs-lookup"><span data-stu-id="d453d-122">3</span></span>|<span data-ttu-id="d453d-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="d453d-123">MacOS.</span></span>|
|<span data-ttu-id="d453d-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="d453d-124">windowsPhone81</span></span>|<span data-ttu-id="d453d-125">4</span><span class="sxs-lookup"><span data-stu-id="d453d-125">4</span></span>|<span data-ttu-id="d453d-126">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="d453d-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="d453d-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="d453d-127">windows81AndLater</span></span>|<span data-ttu-id="d453d-128">5</span><span class="sxs-lookup"><span data-stu-id="d453d-128">5</span></span>|<span data-ttu-id="d453d-129">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="d453d-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="d453d-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="d453d-130">windows10AndLater</span></span>|<span data-ttu-id="d453d-131">6</span><span class="sxs-lookup"><span data-stu-id="d453d-131">6</span></span>|<span data-ttu-id="d453d-132">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="d453d-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="d453d-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="d453d-133">androidWorkProfile</span></span>|<span data-ttu-id="d453d-134">7</span><span class="sxs-lookup"><span data-stu-id="d453d-134">7</span></span>|<span data-ttu-id="d453d-135">AndroidWorkProfile。</span><span class="sxs-lookup"><span data-stu-id="d453d-135">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="d453d-136">all</span><span class="sxs-lookup"><span data-stu-id="d453d-136">all</span></span>|<span data-ttu-id="d453d-137">100</span><span class="sxs-lookup"><span data-stu-id="d453d-137">100</span></span>|<span data-ttu-id="d453d-138">所有平台。</span><span class="sxs-lookup"><span data-stu-id="d453d-138">All platforms.</span></span>|





