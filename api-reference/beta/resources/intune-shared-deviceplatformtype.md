---
title: devicePlatformType 枚举类型
description: 支持的平台类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 17b3325ae93443af8660291170975eb3944add4d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523693"
---
# <a name="deviceplatformtype-enum-type"></a><span data-ttu-id="56896-103">devicePlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="56896-103">devicePlatformType enum type</span></span>

<span data-ttu-id="56896-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="56896-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56896-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56896-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56896-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56896-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56896-107">支持的平台类型。</span><span class="sxs-lookup"><span data-stu-id="56896-107">Supported platform types.</span></span>

## <a name="members"></a><span data-ttu-id="56896-108">成员</span><span class="sxs-lookup"><span data-stu-id="56896-108">Members</span></span>
|<span data-ttu-id="56896-109">成员</span><span class="sxs-lookup"><span data-stu-id="56896-109">Member</span></span>|<span data-ttu-id="56896-110">值</span><span class="sxs-lookup"><span data-stu-id="56896-110">Value</span></span>|<span data-ttu-id="56896-111">说明</span><span class="sxs-lookup"><span data-stu-id="56896-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56896-112">android</span><span class="sxs-lookup"><span data-stu-id="56896-112">android</span></span>|<span data-ttu-id="56896-113">0</span><span class="sxs-lookup"><span data-stu-id="56896-113">0</span></span>|<span data-ttu-id="56896-114">Android.</span><span class="sxs-lookup"><span data-stu-id="56896-114">Android.</span></span>|
|<span data-ttu-id="56896-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="56896-115">androidForWork</span></span>|<span data-ttu-id="56896-116">1 </span><span class="sxs-lookup"><span data-stu-id="56896-116">1</span></span>|<span data-ttu-id="56896-117">AndroidForWork.</span><span class="sxs-lookup"><span data-stu-id="56896-117">AndroidForWork.</span></span>|
|<span data-ttu-id="56896-118">iOS</span><span class="sxs-lookup"><span data-stu-id="56896-118">iOS</span></span>|<span data-ttu-id="56896-119">2 </span><span class="sxs-lookup"><span data-stu-id="56896-119">2</span></span>|<span data-ttu-id="56896-120">iOS.</span><span class="sxs-lookup"><span data-stu-id="56896-120">iOS.</span></span>|
|<span data-ttu-id="56896-121">macOS</span><span class="sxs-lookup"><span data-stu-id="56896-121">macOS</span></span>|<span data-ttu-id="56896-122">3 </span><span class="sxs-lookup"><span data-stu-id="56896-122">3</span></span>|<span data-ttu-id="56896-123">MacOS.</span><span class="sxs-lookup"><span data-stu-id="56896-123">MacOS.</span></span>|
|<span data-ttu-id="56896-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="56896-124">windowsPhone81</span></span>|<span data-ttu-id="56896-125">4 </span><span class="sxs-lookup"><span data-stu-id="56896-125">4</span></span>|<span data-ttu-id="56896-126">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="56896-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="56896-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="56896-127">windows81AndLater</span></span>|<span data-ttu-id="56896-128">5 </span><span class="sxs-lookup"><span data-stu-id="56896-128">5</span></span>|<span data-ttu-id="56896-129">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="56896-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="56896-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="56896-130">windows10AndLater</span></span>|<span data-ttu-id="56896-131">6 </span><span class="sxs-lookup"><span data-stu-id="56896-131">6</span></span>|<span data-ttu-id="56896-132">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="56896-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="56896-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="56896-133">androidWorkProfile</span></span>|<span data-ttu-id="56896-134">7 </span><span class="sxs-lookup"><span data-stu-id="56896-134">7</span></span>|<span data-ttu-id="56896-135">Android 工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="56896-135">Android Work Profile.</span></span>|
|<span data-ttu-id="56896-136">unknown</span><span class="sxs-lookup"><span data-stu-id="56896-136">unknown</span></span>|<span data-ttu-id="56896-137">8 </span><span class="sxs-lookup"><span data-stu-id="56896-137">8</span></span>|<span data-ttu-id="56896-138">陌生.</span><span class="sxs-lookup"><span data-stu-id="56896-138">Unknown.</span></span>|



