---
title: devicePlatformType 枚举类型
description: 支持的平台类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 51f74a9820b808bcc5685494665c67679d2191a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562207"
---
# <a name="deviceplatformtype-enum-type"></a><span data-ttu-id="3e1d7-103">devicePlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3e1d7-103">devicePlatformType enum type</span></span>

> <span data-ttu-id="3e1d7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e1d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e1d7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e1d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e1d7-106">支持的平台类型。</span><span class="sxs-lookup"><span data-stu-id="3e1d7-106">Supported platform types.</span></span>

## <a name="members"></a><span data-ttu-id="3e1d7-107">成员</span><span class="sxs-lookup"><span data-stu-id="3e1d7-107">Members</span></span>
|<span data-ttu-id="3e1d7-108">成员</span><span class="sxs-lookup"><span data-stu-id="3e1d7-108">Member</span></span>|<span data-ttu-id="3e1d7-109">值</span><span class="sxs-lookup"><span data-stu-id="3e1d7-109">Value</span></span>|<span data-ttu-id="3e1d7-110">说明</span><span class="sxs-lookup"><span data-stu-id="3e1d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e1d7-111">android</span><span class="sxs-lookup"><span data-stu-id="3e1d7-111">android</span></span>|<span data-ttu-id="3e1d7-112">0</span><span class="sxs-lookup"><span data-stu-id="3e1d7-112">0</span></span>|<span data-ttu-id="3e1d7-113">Android.</span><span class="sxs-lookup"><span data-stu-id="3e1d7-113">Android.</span></span>|
|<span data-ttu-id="3e1d7-114">androidForWork</span><span class="sxs-lookup"><span data-stu-id="3e1d7-114">androidForWork</span></span>|<span data-ttu-id="3e1d7-115">1</span><span class="sxs-lookup"><span data-stu-id="3e1d7-115">1</span></span>|<span data-ttu-id="3e1d7-116">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="3e1d7-116">AndroidForWork.</span></span>|
|<span data-ttu-id="3e1d7-117">iOS</span><span class="sxs-lookup"><span data-stu-id="3e1d7-117">iOS</span></span>|<span data-ttu-id="3e1d7-118">2 </span><span class="sxs-lookup"><span data-stu-id="3e1d7-118">2</span></span>|<span data-ttu-id="3e1d7-119">iOS.</span><span class="sxs-lookup"><span data-stu-id="3e1d7-119">iOS.</span></span>|
|<span data-ttu-id="3e1d7-120">macOS</span><span class="sxs-lookup"><span data-stu-id="3e1d7-120">macOS</span></span>|<span data-ttu-id="3e1d7-121">3 </span><span class="sxs-lookup"><span data-stu-id="3e1d7-121">3</span></span>|<span data-ttu-id="3e1d7-122">MacOS.</span><span class="sxs-lookup"><span data-stu-id="3e1d7-122">MacOS.</span></span>|
|<span data-ttu-id="3e1d7-123">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="3e1d7-123">windowsPhone81</span></span>|<span data-ttu-id="3e1d7-124">4 </span><span class="sxs-lookup"><span data-stu-id="3e1d7-124">4</span></span>|<span data-ttu-id="3e1d7-125">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="3e1d7-125">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="3e1d7-126">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="3e1d7-126">windows81AndLater</span></span>|<span data-ttu-id="3e1d7-127">5 </span><span class="sxs-lookup"><span data-stu-id="3e1d7-127">5</span></span>|<span data-ttu-id="3e1d7-128">Windows 8.1 及更高版本</span><span class="sxs-lookup"><span data-stu-id="3e1d7-128">Windows 8.1 and later</span></span>|
|<span data-ttu-id="3e1d7-129">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="3e1d7-129">windows10AndLater</span></span>|<span data-ttu-id="3e1d7-130">6 </span><span class="sxs-lookup"><span data-stu-id="3e1d7-130">6</span></span>|<span data-ttu-id="3e1d7-131">Windows 10 及更高版本。</span><span class="sxs-lookup"><span data-stu-id="3e1d7-131">Windows 10 and later.</span></span>|
|<span data-ttu-id="3e1d7-132">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="3e1d7-132">androidWorkProfile</span></span>|<span data-ttu-id="3e1d7-133">7 </span><span class="sxs-lookup"><span data-stu-id="3e1d7-133">7</span></span>|<span data-ttu-id="3e1d7-134">Android 工作配置文件。</span><span class="sxs-lookup"><span data-stu-id="3e1d7-134">Android Work Profile.</span></span>|





