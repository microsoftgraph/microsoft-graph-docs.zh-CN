---
title: androidKeyguardFeature 枚举类型
description: Android keyguard 功能。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df89e1e9170bf2e3691116e27125514c7e0a6de9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429370"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="ec831-103">androidKeyguardFeature 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ec831-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="ec831-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ec831-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ec831-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ec831-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec831-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec831-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec831-107">Android keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="ec831-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="ec831-108">成员</span><span class="sxs-lookup"><span data-stu-id="ec831-108">Members</span></span>
|<span data-ttu-id="ec831-109">成员</span><span class="sxs-lookup"><span data-stu-id="ec831-109">Member</span></span>|<span data-ttu-id="ec831-110">值</span><span class="sxs-lookup"><span data-stu-id="ec831-110">Value</span></span>|<span data-ttu-id="ec831-111">说明</span><span class="sxs-lookup"><span data-stu-id="ec831-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec831-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ec831-112">notConfigured</span></span>|<span data-ttu-id="ec831-113">0</span><span class="sxs-lookup"><span data-stu-id="ec831-113">0</span></span>|<span data-ttu-id="ec831-114">未配置;此值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="ec831-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="ec831-115">摄像机</span><span class="sxs-lookup"><span data-stu-id="ec831-115">camera</span></span>|<span data-ttu-id="ec831-116">1</span><span class="sxs-lookup"><span data-stu-id="ec831-116">1</span></span>|<span data-ttu-id="ec831-117">在安全 keyguard 屏幕上时的照相机用法。</span><span class="sxs-lookup"><span data-stu-id="ec831-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="ec831-118">通知</span><span class="sxs-lookup"><span data-stu-id="ec831-118">notifications</span></span>|<span data-ttu-id="ec831-119">2</span><span class="sxs-lookup"><span data-stu-id="ec831-119">2</span></span>|<span data-ttu-id="ec831-120">显示在安全 keyguard 屏幕上时的通知。</span><span class="sxs-lookup"><span data-stu-id="ec831-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="ec831-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="ec831-121">unredactedNotifications</span></span>|<span data-ttu-id="ec831-122">3</span><span class="sxs-lookup"><span data-stu-id="ec831-122">3</span></span>|<span data-ttu-id="ec831-123">在安全 keyguard 屏幕上时显示 unredacted 通知。</span><span class="sxs-lookup"><span data-stu-id="ec831-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="ec831-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="ec831-124">trustAgents</span></span>|<span data-ttu-id="ec831-125">4</span><span class="sxs-lookup"><span data-stu-id="ec831-125">4</span></span>|<span data-ttu-id="ec831-126">信任代理时安全 keyguard 屏幕上的状态。</span><span class="sxs-lookup"><span data-stu-id="ec831-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="ec831-127">指纹</span><span class="sxs-lookup"><span data-stu-id="ec831-127">fingerprint</span></span>|<span data-ttu-id="ec831-128">5</span><span class="sxs-lookup"><span data-stu-id="ec831-128">5</span></span>|<span data-ttu-id="ec831-129">指纹传感器使用率在安全 keyguard 屏幕上时。</span><span class="sxs-lookup"><span data-stu-id="ec831-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="ec831-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="ec831-130">remoteInput</span></span>|<span data-ttu-id="ec831-131">6</span><span class="sxs-lookup"><span data-stu-id="ec831-131">6</span></span>|<span data-ttu-id="ec831-132">在安全 keyguard 屏幕上时通知文本项。</span><span class="sxs-lookup"><span data-stu-id="ec831-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="ec831-133">allFeatures</span><span class="sxs-lookup"><span data-stu-id="ec831-133">allFeatures</span></span>|<span data-ttu-id="ec831-134">7</span><span class="sxs-lookup"><span data-stu-id="ec831-134">7</span></span>|<span data-ttu-id="ec831-135">在安全 keyguard 屏幕上时的所有 keyguard 功能。</span><span class="sxs-lookup"><span data-stu-id="ec831-135">All keyguard features when on secure keyguard screens.</span></span>|




