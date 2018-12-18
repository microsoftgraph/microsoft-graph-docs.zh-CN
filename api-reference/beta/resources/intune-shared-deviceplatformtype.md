---
title: devicePlatformType 枚举类型
description: 支持的平台类型。
author: tfitzmac
ms.openlocfilehash: 6609ea65eb7469155f4e1bf3f8d6e5ccc424d338
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316217"
---
# <a name="deviceplatformtype-enum-type"></a><span data-ttu-id="cc8e5-103">devicePlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cc8e5-103">devicePlatformType enum type</span></span>

> <span data-ttu-id="cc8e5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc8e5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc8e5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc8e5-107">支持的平台类型。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-107">Supported platform types.</span></span>
## <a name="members"></a><span data-ttu-id="cc8e5-108">成员</span><span class="sxs-lookup"><span data-stu-id="cc8e5-108">Members</span></span>
|<span data-ttu-id="cc8e5-109">成员</span><span class="sxs-lookup"><span data-stu-id="cc8e5-109">Member</span></span>|<span data-ttu-id="cc8e5-110">值</span><span class="sxs-lookup"><span data-stu-id="cc8e5-110">Value</span></span>|<span data-ttu-id="cc8e5-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc8e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc8e5-112">android</span><span class="sxs-lookup"><span data-stu-id="cc8e5-112">android</span></span>|<span data-ttu-id="cc8e5-113">0</span><span class="sxs-lookup"><span data-stu-id="cc8e5-113">0</span></span>|<span data-ttu-id="cc8e5-114">Android。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-114">Android.</span></span>|
|<span data-ttu-id="cc8e5-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="cc8e5-115">androidForWork</span></span>|<span data-ttu-id="cc8e5-116">1</span><span class="sxs-lookup"><span data-stu-id="cc8e5-116">1</span></span>|<span data-ttu-id="cc8e5-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-117">AndroidForWork.</span></span>|
|<span data-ttu-id="cc8e5-118">iOS</span><span class="sxs-lookup"><span data-stu-id="cc8e5-118">iOS</span></span>|<span data-ttu-id="cc8e5-119">2</span><span class="sxs-lookup"><span data-stu-id="cc8e5-119">2</span></span>|<span data-ttu-id="cc8e5-120">iOS。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-120">iOS.</span></span>|
|<span data-ttu-id="cc8e5-121">macOS</span><span class="sxs-lookup"><span data-stu-id="cc8e5-121">macOS</span></span>|<span data-ttu-id="cc8e5-122">3</span><span class="sxs-lookup"><span data-stu-id="cc8e5-122">3</span></span>|<span data-ttu-id="cc8e5-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-123">MacOS.</span></span>|
|<span data-ttu-id="cc8e5-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="cc8e5-124">windowsPhone81</span></span>|<span data-ttu-id="cc8e5-125">4</span><span class="sxs-lookup"><span data-stu-id="cc8e5-125">4</span></span>|<span data-ttu-id="cc8e5-126">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="cc8e5-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="cc8e5-127">windows81AndLater</span></span>|<span data-ttu-id="cc8e5-128">5</span><span class="sxs-lookup"><span data-stu-id="cc8e5-128">5</span></span>|<span data-ttu-id="cc8e5-129">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="cc8e5-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="cc8e5-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="cc8e5-130">windows10AndLater</span></span>|<span data-ttu-id="cc8e5-131">6</span><span class="sxs-lookup"><span data-stu-id="cc8e5-131">6</span></span>|<span data-ttu-id="cc8e5-132">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="cc8e5-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="cc8e5-133">androidWorkProfile</span></span>|<span data-ttu-id="cc8e5-134">7</span><span class="sxs-lookup"><span data-stu-id="cc8e5-134">7</span></span>|<span data-ttu-id="cc8e5-135">Android 工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="cc8e5-135">Android Work Profile.</span></span>|





