---
title: androidKeyguardFeature 枚举类型
description: Android keyguard 功能。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c3dac1536f13fc068eb9bac0d2c922e0ce51fa08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011734"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="bac57-103">androidKeyguardFeature 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bac57-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="bac57-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bac57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bac57-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bac57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bac57-106">Android keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="bac57-106">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="bac57-107">成员</span><span class="sxs-lookup"><span data-stu-id="bac57-107">Members</span></span>
|<span data-ttu-id="bac57-108">成员</span><span class="sxs-lookup"><span data-stu-id="bac57-108">Member</span></span>|<span data-ttu-id="bac57-109">值</span><span class="sxs-lookup"><span data-stu-id="bac57-109">Value</span></span>|<span data-ttu-id="bac57-110">说明</span><span class="sxs-lookup"><span data-stu-id="bac57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac57-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bac57-111">notConfigured</span></span>|<span data-ttu-id="bac57-112">0</span><span class="sxs-lookup"><span data-stu-id="bac57-112">0</span></span>|<span data-ttu-id="bac57-113">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="bac57-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="bac57-114">拍照</span><span class="sxs-lookup"><span data-stu-id="bac57-114">camera</span></span>|<span data-ttu-id="bac57-115">1</span><span class="sxs-lookup"><span data-stu-id="bac57-115">1</span></span>|<span data-ttu-id="bac57-116">在安全 keyguard 屏幕上使用摄像头。</span><span class="sxs-lookup"><span data-stu-id="bac57-116">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="bac57-117">通知</span><span class="sxs-lookup"><span data-stu-id="bac57-117">notifications</span></span>|<span data-ttu-id="bac57-118">双面</span><span class="sxs-lookup"><span data-stu-id="bac57-118">2</span></span>|<span data-ttu-id="bac57-119">在安全 keyguard 屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="bac57-119">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="bac57-120">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="bac57-120">unredactedNotifications</span></span>|<span data-ttu-id="bac57-121">第三章</span><span class="sxs-lookup"><span data-stu-id="bac57-121">3</span></span>|<span data-ttu-id="bac57-122">在安全 keyguard 屏幕上显示 unredacted 通知。</span><span class="sxs-lookup"><span data-stu-id="bac57-122">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="bac57-123">trustAgents</span><span class="sxs-lookup"><span data-stu-id="bac57-123">trustAgents</span></span>|<span data-ttu-id="bac57-124">4</span><span class="sxs-lookup"><span data-stu-id="bac57-124">4</span></span>|<span data-ttu-id="bac57-125">在安全 keyguard 屏幕上信任代理状态。</span><span class="sxs-lookup"><span data-stu-id="bac57-125">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="bac57-126">其次</span><span class="sxs-lookup"><span data-stu-id="bac57-126">fingerprint</span></span>|<span data-ttu-id="bac57-127">5</span><span class="sxs-lookup"><span data-stu-id="bac57-127">5</span></span>|<span data-ttu-id="bac57-128">在安全 keyguard 屏幕上使用指纹传感器。</span><span class="sxs-lookup"><span data-stu-id="bac57-128">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="bac57-129">remoteInput</span><span class="sxs-lookup"><span data-stu-id="bac57-129">remoteInput</span></span>|<span data-ttu-id="bac57-130">型</span><span class="sxs-lookup"><span data-stu-id="bac57-130">6</span></span>|<span data-ttu-id="bac57-131">在安全 keyguard 屏幕上时发出通知文本条目。</span><span class="sxs-lookup"><span data-stu-id="bac57-131">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="bac57-132">allFeatures</span><span class="sxs-lookup"><span data-stu-id="bac57-132">allFeatures</span></span>|<span data-ttu-id="bac57-133">步</span><span class="sxs-lookup"><span data-stu-id="bac57-133">7</span></span>|<span data-ttu-id="bac57-134">在安全 keyguard 屏幕上时的所有 keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="bac57-134">All keyguard features when on secure keyguard screens.</span></span>|





