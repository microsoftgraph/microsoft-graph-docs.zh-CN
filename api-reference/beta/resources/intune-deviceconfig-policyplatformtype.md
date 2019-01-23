---
title: policyPlatformType 枚举类型
description: 策略升高平台类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5e075c0974a315cfabd3238379278266a2f7fb8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399729"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="df299-103">policyPlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="df299-103">policyPlatformType enum type</span></span>

> <span data-ttu-id="df299-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="df299-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df299-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df299-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df299-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df299-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df299-107">策略升高平台类型。</span><span class="sxs-lookup"><span data-stu-id="df299-107">Suppoorted platform types for policies.</span></span>

## <a name="members"></a><span data-ttu-id="df299-108">成员</span><span class="sxs-lookup"><span data-stu-id="df299-108">Members</span></span>
|<span data-ttu-id="df299-109">成员</span><span class="sxs-lookup"><span data-stu-id="df299-109">Member</span></span>|<span data-ttu-id="df299-110">值</span><span class="sxs-lookup"><span data-stu-id="df299-110">Value</span></span>|<span data-ttu-id="df299-111">说明</span><span class="sxs-lookup"><span data-stu-id="df299-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df299-112">android</span><span class="sxs-lookup"><span data-stu-id="df299-112">android</span></span>|<span data-ttu-id="df299-113">0</span><span class="sxs-lookup"><span data-stu-id="df299-113">0</span></span>|<span data-ttu-id="df299-114">Android。</span><span class="sxs-lookup"><span data-stu-id="df299-114">Android.</span></span>|
|<span data-ttu-id="df299-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="df299-115">androidForWork</span></span>|<span data-ttu-id="df299-116">1</span><span class="sxs-lookup"><span data-stu-id="df299-116">1</span></span>|<span data-ttu-id="df299-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="df299-117">AndroidForWork.</span></span>|
|<span data-ttu-id="df299-118">iOS</span><span class="sxs-lookup"><span data-stu-id="df299-118">iOS</span></span>|<span data-ttu-id="df299-119">2</span><span class="sxs-lookup"><span data-stu-id="df299-119">2</span></span>|<span data-ttu-id="df299-120">iOS。</span><span class="sxs-lookup"><span data-stu-id="df299-120">iOS.</span></span>|
|<span data-ttu-id="df299-121">macOS</span><span class="sxs-lookup"><span data-stu-id="df299-121">macOS</span></span>|<span data-ttu-id="df299-122">3</span><span class="sxs-lookup"><span data-stu-id="df299-122">3</span></span>|<span data-ttu-id="df299-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="df299-123">MacOS.</span></span>|
|<span data-ttu-id="df299-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="df299-124">windowsPhone81</span></span>|<span data-ttu-id="df299-125">4</span><span class="sxs-lookup"><span data-stu-id="df299-125">4</span></span>|<span data-ttu-id="df299-126">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="df299-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="df299-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="df299-127">windows81AndLater</span></span>|<span data-ttu-id="df299-128">5</span><span class="sxs-lookup"><span data-stu-id="df299-128">5</span></span>|<span data-ttu-id="df299-129">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="df299-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="df299-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="df299-130">windows10AndLater</span></span>|<span data-ttu-id="df299-131">6</span><span class="sxs-lookup"><span data-stu-id="df299-131">6</span></span>|<span data-ttu-id="df299-132">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="df299-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="df299-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="df299-133">androidWorkProfile</span></span>|<span data-ttu-id="df299-134">7</span><span class="sxs-lookup"><span data-stu-id="df299-134">7</span></span>|<span data-ttu-id="df299-135">AndroidWorkProfile。</span><span class="sxs-lookup"><span data-stu-id="df299-135">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="df299-136">all</span><span class="sxs-lookup"><span data-stu-id="df299-136">all</span></span>|<span data-ttu-id="df299-137">100</span><span class="sxs-lookup"><span data-stu-id="df299-137">100</span></span>|<span data-ttu-id="df299-138">所有平台。</span><span class="sxs-lookup"><span data-stu-id="df299-138">All platforms.</span></span>|




