---
title: androidKeyguardFeature 枚举类型
description: Android keyguard 功能。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0ff958273d8b39293709b14a960d8bd6b3ea940
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556233"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="2df6f-103">androidKeyguardFeature 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2df6f-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="2df6f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2df6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2df6f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2df6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2df6f-106">Android keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="2df6f-106">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="2df6f-107">成员</span><span class="sxs-lookup"><span data-stu-id="2df6f-107">Members</span></span>
|<span data-ttu-id="2df6f-108">成员</span><span class="sxs-lookup"><span data-stu-id="2df6f-108">Member</span></span>|<span data-ttu-id="2df6f-109">值</span><span class="sxs-lookup"><span data-stu-id="2df6f-109">Value</span></span>|<span data-ttu-id="2df6f-110">说明</span><span class="sxs-lookup"><span data-stu-id="2df6f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df6f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2df6f-111">notConfigured</span></span>|<span data-ttu-id="2df6f-112">0</span><span class="sxs-lookup"><span data-stu-id="2df6f-112">0</span></span>|<span data-ttu-id="2df6f-113">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="2df6f-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="2df6f-114">拍照</span><span class="sxs-lookup"><span data-stu-id="2df6f-114">camera</span></span>|<span data-ttu-id="2df6f-115">1</span><span class="sxs-lookup"><span data-stu-id="2df6f-115">1</span></span>|<span data-ttu-id="2df6f-116">在安全 keyguard 屏幕上使用摄像头。</span><span class="sxs-lookup"><span data-stu-id="2df6f-116">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2df6f-117">通知</span><span class="sxs-lookup"><span data-stu-id="2df6f-117">notifications</span></span>|<span data-ttu-id="2df6f-118">2 </span><span class="sxs-lookup"><span data-stu-id="2df6f-118">2</span></span>|<span data-ttu-id="2df6f-119">在安全 keyguard 屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="2df6f-119">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2df6f-120">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="2df6f-120">unredactedNotifications</span></span>|<span data-ttu-id="2df6f-121">3 </span><span class="sxs-lookup"><span data-stu-id="2df6f-121">3</span></span>|<span data-ttu-id="2df6f-122">在安全 keyguard 屏幕上显示 unredacted 通知。</span><span class="sxs-lookup"><span data-stu-id="2df6f-122">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2df6f-123">trustAgents</span><span class="sxs-lookup"><span data-stu-id="2df6f-123">trustAgents</span></span>|<span data-ttu-id="2df6f-124">4 </span><span class="sxs-lookup"><span data-stu-id="2df6f-124">4</span></span>|<span data-ttu-id="2df6f-125">在安全 keyguard 屏幕上信任代理状态。</span><span class="sxs-lookup"><span data-stu-id="2df6f-125">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2df6f-126">其次</span><span class="sxs-lookup"><span data-stu-id="2df6f-126">fingerprint</span></span>|<span data-ttu-id="2df6f-127">5 </span><span class="sxs-lookup"><span data-stu-id="2df6f-127">5</span></span>|<span data-ttu-id="2df6f-128">在安全 keyguard 屏幕上使用指纹传感器。</span><span class="sxs-lookup"><span data-stu-id="2df6f-128">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2df6f-129">remoteInput</span><span class="sxs-lookup"><span data-stu-id="2df6f-129">remoteInput</span></span>|<span data-ttu-id="2df6f-130">6 </span><span class="sxs-lookup"><span data-stu-id="2df6f-130">6</span></span>|<span data-ttu-id="2df6f-131">在安全 keyguard 屏幕上时发出通知文本条目。</span><span class="sxs-lookup"><span data-stu-id="2df6f-131">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="2df6f-132">allFeatures</span><span class="sxs-lookup"><span data-stu-id="2df6f-132">allFeatures</span></span>|<span data-ttu-id="2df6f-133">7 </span><span class="sxs-lookup"><span data-stu-id="2df6f-133">7</span></span>|<span data-ttu-id="2df6f-134">在安全 keyguard 屏幕上时的所有 keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="2df6f-134">All keyguard features when on secure keyguard screens.</span></span>|





