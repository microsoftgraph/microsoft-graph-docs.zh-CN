---
title: policyPlatformType 枚举类型
description: 策略支持的平台类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d36251048fda3ffb1e47c8bcc676e5cb62ab67ef
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664893"
---
# <a name="policyplatformtype-enum-type"></a><span data-ttu-id="37e69-103">policyPlatformType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="37e69-103">policyPlatformType enum type</span></span>

<span data-ttu-id="37e69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37e69-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37e69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37e69-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37e69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37e69-107">策略支持的平台类型。</span><span class="sxs-lookup"><span data-stu-id="37e69-107">Supported platform types for policies.</span></span>

## <a name="members"></a><span data-ttu-id="37e69-108">成员</span><span class="sxs-lookup"><span data-stu-id="37e69-108">Members</span></span>
|<span data-ttu-id="37e69-109">成员</span><span class="sxs-lookup"><span data-stu-id="37e69-109">Member</span></span>|<span data-ttu-id="37e69-110">值</span><span class="sxs-lookup"><span data-stu-id="37e69-110">Value</span></span>|<span data-ttu-id="37e69-111">说明</span><span class="sxs-lookup"><span data-stu-id="37e69-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37e69-112">android</span><span class="sxs-lookup"><span data-stu-id="37e69-112">android</span></span>|<span data-ttu-id="37e69-113">0</span><span class="sxs-lookup"><span data-stu-id="37e69-113">0</span></span>|<span data-ttu-id="37e69-114">Android。</span><span class="sxs-lookup"><span data-stu-id="37e69-114">Android.</span></span>|
|<span data-ttu-id="37e69-115">androidForWork</span><span class="sxs-lookup"><span data-stu-id="37e69-115">androidForWork</span></span>|<span data-ttu-id="37e69-116">1</span><span class="sxs-lookup"><span data-stu-id="37e69-116">1</span></span>|<span data-ttu-id="37e69-117">AndroidForWork。</span><span class="sxs-lookup"><span data-stu-id="37e69-117">AndroidForWork.</span></span>|
|<span data-ttu-id="37e69-118">iOS</span><span class="sxs-lookup"><span data-stu-id="37e69-118">iOS</span></span>|<span data-ttu-id="37e69-119">2</span><span class="sxs-lookup"><span data-stu-id="37e69-119">2</span></span>|<span data-ttu-id="37e69-120">iOS。</span><span class="sxs-lookup"><span data-stu-id="37e69-120">iOS.</span></span>|
|<span data-ttu-id="37e69-121">macOS</span><span class="sxs-lookup"><span data-stu-id="37e69-121">macOS</span></span>|<span data-ttu-id="37e69-122">3</span><span class="sxs-lookup"><span data-stu-id="37e69-122">3</span></span>|<span data-ttu-id="37e69-123">MacOS。</span><span class="sxs-lookup"><span data-stu-id="37e69-123">MacOS.</span></span>|
|<span data-ttu-id="37e69-124">windowsPhone81</span><span class="sxs-lookup"><span data-stu-id="37e69-124">windowsPhone81</span></span>|<span data-ttu-id="37e69-125">4 </span><span class="sxs-lookup"><span data-stu-id="37e69-125">4</span></span>|<span data-ttu-id="37e69-126">WindowsPhone 8.1。</span><span class="sxs-lookup"><span data-stu-id="37e69-126">WindowsPhone 8.1.</span></span>|
|<span data-ttu-id="37e69-127">windows81AndLater</span><span class="sxs-lookup"><span data-stu-id="37e69-127">windows81AndLater</span></span>|<span data-ttu-id="37e69-128">5 </span><span class="sxs-lookup"><span data-stu-id="37e69-128">5</span></span>|<span data-ttu-id="37e69-129">Windows 8.1及更高版本</span><span class="sxs-lookup"><span data-stu-id="37e69-129">Windows 8.1 and later</span></span>|
|<span data-ttu-id="37e69-130">windows10AndLater</span><span class="sxs-lookup"><span data-stu-id="37e69-130">windows10AndLater</span></span>|<span data-ttu-id="37e69-131">6 </span><span class="sxs-lookup"><span data-stu-id="37e69-131">6</span></span>|<span data-ttu-id="37e69-132">Windows 10及更高版本。</span><span class="sxs-lookup"><span data-stu-id="37e69-132">Windows 10 and later.</span></span>|
|<span data-ttu-id="37e69-133">androidWorkProfile</span><span class="sxs-lookup"><span data-stu-id="37e69-133">androidWorkProfile</span></span>|<span data-ttu-id="37e69-134">7 </span><span class="sxs-lookup"><span data-stu-id="37e69-134">7</span></span>|<span data-ttu-id="37e69-135">AndroidWorkProfile。</span><span class="sxs-lookup"><span data-stu-id="37e69-135">AndroidWorkProfile.</span></span>|
|<span data-ttu-id="37e69-136">windows10XProfile</span><span class="sxs-lookup"><span data-stu-id="37e69-136">windows10XProfile</span></span>|<span data-ttu-id="37e69-137">8 </span><span class="sxs-lookup"><span data-stu-id="37e69-137">8</span></span>|<span data-ttu-id="37e69-138">Windows10XProfile。</span><span class="sxs-lookup"><span data-stu-id="37e69-138">Windows10XProfile.</span></span>|
|<span data-ttu-id="37e69-139">androidAOSP</span><span class="sxs-lookup"><span data-stu-id="37e69-139">androidAOSP</span></span>|<span data-ttu-id="37e69-140">9 </span><span class="sxs-lookup"><span data-stu-id="37e69-140">9</span></span>|<span data-ttu-id="37e69-141">AndroidAOSPProfile。</span><span class="sxs-lookup"><span data-stu-id="37e69-141">AndroidAOSPProfile.</span></span>|
|<span data-ttu-id="37e69-142">all</span><span class="sxs-lookup"><span data-stu-id="37e69-142">all</span></span>|<span data-ttu-id="37e69-143">100</span><span class="sxs-lookup"><span data-stu-id="37e69-143">100</span></span>|<span data-ttu-id="37e69-144">所有平台。</span><span class="sxs-lookup"><span data-stu-id="37e69-144">All platforms.</span></span>|



