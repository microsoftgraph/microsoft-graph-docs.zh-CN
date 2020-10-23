---
title: androidKeyguardFeature 枚举类型
description: Android keyguard 功能。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 15e0c8f1dc14dae41b917e85867020fb4d57571f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690712"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="7e2f2-103">androidKeyguardFeature 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7e2f2-103">androidKeyguardFeature enum type</span></span>

<span data-ttu-id="7e2f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e2f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e2f2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e2f2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e2f2-107">Android keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="7e2f2-108">成员</span><span class="sxs-lookup"><span data-stu-id="7e2f2-108">Members</span></span>
|<span data-ttu-id="7e2f2-109">成员</span><span class="sxs-lookup"><span data-stu-id="7e2f2-109">Member</span></span>|<span data-ttu-id="7e2f2-110">值</span><span class="sxs-lookup"><span data-stu-id="7e2f2-110">Value</span></span>|<span data-ttu-id="7e2f2-111">说明</span><span class="sxs-lookup"><span data-stu-id="7e2f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e2f2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7e2f2-112">notConfigured</span></span>|<span data-ttu-id="7e2f2-113">0</span><span class="sxs-lookup"><span data-stu-id="7e2f2-113">0</span></span>|<span data-ttu-id="7e2f2-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="7e2f2-115">拍照</span><span class="sxs-lookup"><span data-stu-id="7e2f2-115">camera</span></span>|<span data-ttu-id="7e2f2-116">1</span><span class="sxs-lookup"><span data-stu-id="7e2f2-116">1</span></span>|<span data-ttu-id="7e2f2-117">在安全 keyguard 屏幕上使用摄像头。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7e2f2-118">通知</span><span class="sxs-lookup"><span data-stu-id="7e2f2-118">notifications</span></span>|<span data-ttu-id="7e2f2-119">双面</span><span class="sxs-lookup"><span data-stu-id="7e2f2-119">2</span></span>|<span data-ttu-id="7e2f2-120">在安全 keyguard 屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7e2f2-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="7e2f2-121">unredactedNotifications</span></span>|<span data-ttu-id="7e2f2-122">第三章</span><span class="sxs-lookup"><span data-stu-id="7e2f2-122">3</span></span>|<span data-ttu-id="7e2f2-123">在安全 keyguard 屏幕上显示 unredacted 通知。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7e2f2-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="7e2f2-124">trustAgents</span></span>|<span data-ttu-id="7e2f2-125">4 </span><span class="sxs-lookup"><span data-stu-id="7e2f2-125">4</span></span>|<span data-ttu-id="7e2f2-126">在安全 keyguard 屏幕上信任代理状态。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7e2f2-127">其次</span><span class="sxs-lookup"><span data-stu-id="7e2f2-127">fingerprint</span></span>|<span data-ttu-id="7e2f2-128">5 </span><span class="sxs-lookup"><span data-stu-id="7e2f2-128">5</span></span>|<span data-ttu-id="7e2f2-129">在安全 keyguard 屏幕上使用指纹传感器。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7e2f2-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="7e2f2-130">remoteInput</span></span>|<span data-ttu-id="7e2f2-131">6 </span><span class="sxs-lookup"><span data-stu-id="7e2f2-131">6</span></span>|<span data-ttu-id="7e2f2-132">在安全 keyguard 屏幕上时发出通知文本条目。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7e2f2-133">allFeatures</span><span class="sxs-lookup"><span data-stu-id="7e2f2-133">allFeatures</span></span>|<span data-ttu-id="7e2f2-134">7 </span><span class="sxs-lookup"><span data-stu-id="7e2f2-134">7</span></span>|<span data-ttu-id="7e2f2-135">在安全 keyguard 屏幕上时的所有 keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="7e2f2-135">All keyguard features when on secure keyguard screens.</span></span>|





