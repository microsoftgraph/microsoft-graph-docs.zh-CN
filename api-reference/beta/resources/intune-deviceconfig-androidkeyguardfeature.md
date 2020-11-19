---
title: androidKeyguardFeature 枚举类型
description: Android keyguard 功能。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d22db1f0960aac0f3cf94d81fcfdd08bb4c45642
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269523"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="c53c3-103">androidKeyguardFeature 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c53c3-103">androidKeyguardFeature enum type</span></span>

<span data-ttu-id="c53c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c53c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c53c3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c53c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c53c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c53c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c53c3-107">Android keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="c53c3-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="c53c3-108">成员</span><span class="sxs-lookup"><span data-stu-id="c53c3-108">Members</span></span>
|<span data-ttu-id="c53c3-109">成员</span><span class="sxs-lookup"><span data-stu-id="c53c3-109">Member</span></span>|<span data-ttu-id="c53c3-110">值</span><span class="sxs-lookup"><span data-stu-id="c53c3-110">Value</span></span>|<span data-ttu-id="c53c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="c53c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c53c3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c53c3-112">notConfigured</span></span>|<span data-ttu-id="c53c3-113">0</span><span class="sxs-lookup"><span data-stu-id="c53c3-113">0</span></span>|<span data-ttu-id="c53c3-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="c53c3-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="c53c3-115">拍照</span><span class="sxs-lookup"><span data-stu-id="c53c3-115">camera</span></span>|<span data-ttu-id="c53c3-116">1</span><span class="sxs-lookup"><span data-stu-id="c53c3-116">1</span></span>|<span data-ttu-id="c53c3-117">在安全 keyguard 屏幕上使用摄像头。</span><span class="sxs-lookup"><span data-stu-id="c53c3-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="c53c3-118">通知</span><span class="sxs-lookup"><span data-stu-id="c53c3-118">notifications</span></span>|<span data-ttu-id="c53c3-119">双面</span><span class="sxs-lookup"><span data-stu-id="c53c3-119">2</span></span>|<span data-ttu-id="c53c3-120">在安全 keyguard 屏幕上显示通知。</span><span class="sxs-lookup"><span data-stu-id="c53c3-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="c53c3-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="c53c3-121">unredactedNotifications</span></span>|<span data-ttu-id="c53c3-122">第三章</span><span class="sxs-lookup"><span data-stu-id="c53c3-122">3</span></span>|<span data-ttu-id="c53c3-123">在安全 keyguard 屏幕上显示 unredacted 通知。</span><span class="sxs-lookup"><span data-stu-id="c53c3-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="c53c3-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="c53c3-124">trustAgents</span></span>|<span data-ttu-id="c53c3-125">4 </span><span class="sxs-lookup"><span data-stu-id="c53c3-125">4</span></span>|<span data-ttu-id="c53c3-126">在安全 keyguard 屏幕上信任代理状态。</span><span class="sxs-lookup"><span data-stu-id="c53c3-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="c53c3-127">其次</span><span class="sxs-lookup"><span data-stu-id="c53c3-127">fingerprint</span></span>|<span data-ttu-id="c53c3-128">5 </span><span class="sxs-lookup"><span data-stu-id="c53c3-128">5</span></span>|<span data-ttu-id="c53c3-129">在安全 keyguard 屏幕上使用指纹传感器。</span><span class="sxs-lookup"><span data-stu-id="c53c3-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="c53c3-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="c53c3-130">remoteInput</span></span>|<span data-ttu-id="c53c3-131">6 </span><span class="sxs-lookup"><span data-stu-id="c53c3-131">6</span></span>|<span data-ttu-id="c53c3-132">在安全 keyguard 屏幕上时发出通知文本条目。</span><span class="sxs-lookup"><span data-stu-id="c53c3-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="c53c3-133">allFeatures</span><span class="sxs-lookup"><span data-stu-id="c53c3-133">allFeatures</span></span>|<span data-ttu-id="c53c3-134">7 </span><span class="sxs-lookup"><span data-stu-id="c53c3-134">7</span></span>|<span data-ttu-id="c53c3-135">在安全 keyguard 屏幕上时的所有 keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="c53c3-135">All keyguard features when on secure keyguard screens.</span></span>|




