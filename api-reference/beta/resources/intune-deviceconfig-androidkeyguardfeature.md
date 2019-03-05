---
title: androidKeyguardFeature 枚举类型
description: Android keyguard 功能。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2987a8220bbbcfc99238587a989b890aff958e47
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161948"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="7d69e-103">androidKeyguardFeature 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7d69e-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="7d69e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7d69e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d69e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7d69e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d69e-106">Android keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="7d69e-106">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="7d69e-107">成员</span><span class="sxs-lookup"><span data-stu-id="7d69e-107">Members</span></span>
|<span data-ttu-id="7d69e-108">成员</span><span class="sxs-lookup"><span data-stu-id="7d69e-108">Member</span></span>|<span data-ttu-id="7d69e-109">值</span><span class="sxs-lookup"><span data-stu-id="7d69e-109">Value</span></span>|<span data-ttu-id="7d69e-110">说明</span><span class="sxs-lookup"><span data-stu-id="7d69e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d69e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7d69e-111">notConfigured</span></span>|<span data-ttu-id="7d69e-112">0</span><span class="sxs-lookup"><span data-stu-id="7d69e-112">0</span></span>|<span data-ttu-id="7d69e-113">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="7d69e-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="7d69e-114">拍照</span><span class="sxs-lookup"><span data-stu-id="7d69e-114">camera</span></span>|<span data-ttu-id="7d69e-115">1</span><span class="sxs-lookup"><span data-stu-id="7d69e-115">1</span></span>|<span data-ttu-id="7d69e-116">在安全 keyguard 屏幕上使用摄像头。</span><span class="sxs-lookup"><span data-stu-id="7d69e-116">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7d69e-117">通知</span><span class="sxs-lookup"><span data-stu-id="7d69e-117">notifications</span></span>|<span data-ttu-id="7d69e-118">双面</span><span class="sxs-lookup"><span data-stu-id="7d69e-118">2</span></span>|<span data-ttu-id="7d69e-119">在安全 keyguard 屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="7d69e-119">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7d69e-120">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="7d69e-120">unredactedNotifications</span></span>|<span data-ttu-id="7d69e-121">第三章</span><span class="sxs-lookup"><span data-stu-id="7d69e-121">3</span></span>|<span data-ttu-id="7d69e-122">在安全 keyguard 屏幕上显示 unredacted 通知。</span><span class="sxs-lookup"><span data-stu-id="7d69e-122">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7d69e-123">trustAgents</span><span class="sxs-lookup"><span data-stu-id="7d69e-123">trustAgents</span></span>|<span data-ttu-id="7d69e-124">4</span><span class="sxs-lookup"><span data-stu-id="7d69e-124">4</span></span>|<span data-ttu-id="7d69e-125">在安全 keyguard 屏幕上信任代理状态。</span><span class="sxs-lookup"><span data-stu-id="7d69e-125">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7d69e-126">其次</span><span class="sxs-lookup"><span data-stu-id="7d69e-126">fingerprint</span></span>|<span data-ttu-id="7d69e-127">5</span><span class="sxs-lookup"><span data-stu-id="7d69e-127">5</span></span>|<span data-ttu-id="7d69e-128">在安全 keyguard 屏幕上使用指纹传感器。</span><span class="sxs-lookup"><span data-stu-id="7d69e-128">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7d69e-129">remoteInput</span><span class="sxs-lookup"><span data-stu-id="7d69e-129">remoteInput</span></span>|<span data-ttu-id="7d69e-130">型</span><span class="sxs-lookup"><span data-stu-id="7d69e-130">6</span></span>|<span data-ttu-id="7d69e-131">在安全 keyguard 屏幕上时发出通知文本条目。</span><span class="sxs-lookup"><span data-stu-id="7d69e-131">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="7d69e-132">allFeatures</span><span class="sxs-lookup"><span data-stu-id="7d69e-132">allFeatures</span></span>|<span data-ttu-id="7d69e-133">步</span><span class="sxs-lookup"><span data-stu-id="7d69e-133">7</span></span>|<span data-ttu-id="7d69e-134">在安全 keyguard 屏幕上时的所有 keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="7d69e-134">All keyguard features when on secure keyguard screens.</span></span>|




