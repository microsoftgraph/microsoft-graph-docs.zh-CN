---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶级失败类别。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efe1a63a86a01001168d2d631280e8a190125987
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368048"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="6fa7a-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6fa7a-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="6fa7a-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fa7a-105">注册的顶级失败类别。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-105">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="6fa7a-106">成员</span><span class="sxs-lookup"><span data-stu-id="6fa7a-106">Members</span></span>
|<span data-ttu-id="6fa7a-107">成员</span><span class="sxs-lookup"><span data-stu-id="6fa7a-107">Member</span></span>|<span data-ttu-id="6fa7a-108">值</span><span class="sxs-lookup"><span data-stu-id="6fa7a-108">Value</span></span>|<span data-ttu-id="6fa7a-109">说明</span><span class="sxs-lookup"><span data-stu-id="6fa7a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa7a-110">unknown</span><span class="sxs-lookup"><span data-stu-id="6fa7a-110">unknown</span></span>|<span data-ttu-id="6fa7a-111">0</span><span class="sxs-lookup"><span data-stu-id="6fa7a-111">0</span></span>|<span data-ttu-id="6fa7a-112">默认值，失败原因未知。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="6fa7a-113">authentication</span><span class="sxs-lookup"><span data-stu-id="6fa7a-113">authentication</span></span>|<span data-ttu-id="6fa7a-114">1</span><span class="sxs-lookup"><span data-stu-id="6fa7a-114">1</span></span>|<span data-ttu-id="6fa7a-115">身份验证失败</span><span class="sxs-lookup"><span data-stu-id="6fa7a-115">Authentication failed</span></span>|
|<span data-ttu-id="6fa7a-116">批准</span><span class="sxs-lookup"><span data-stu-id="6fa7a-116">authorization</span></span>|<span data-ttu-id="6fa7a-117">双面</span><span class="sxs-lookup"><span data-stu-id="6fa7a-117">2</span></span>|<span data-ttu-id="6fa7a-118">呼叫已通过身份验证，但未获授权进行注册。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="6fa7a-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="6fa7a-119">accountValidation</span></span>|<span data-ttu-id="6fa7a-120">第三章</span><span class="sxs-lookup"><span data-stu-id="6fa7a-120">3</span></span>|<span data-ttu-id="6fa7a-121">无法验证注册帐户。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="6fa7a-122">（帐户被阻止，未启用注册）</span><span class="sxs-lookup"><span data-stu-id="6fa7a-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="6fa7a-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="6fa7a-123">userValidation</span></span>|<span data-ttu-id="6fa7a-124">4</span><span class="sxs-lookup"><span data-stu-id="6fa7a-124">4</span></span>|<span data-ttu-id="6fa7a-125">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-125">User could not be validated.</span></span> <span data-ttu-id="6fa7a-126">（用户不存在，缺少许可证）</span><span class="sxs-lookup"><span data-stu-id="6fa7a-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="6fa7a-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="6fa7a-127">deviceNotSupported</span></span>|<span data-ttu-id="6fa7a-128">5</span><span class="sxs-lookup"><span data-stu-id="6fa7a-128">5</span></span>|<span data-ttu-id="6fa7a-129">移动设备管理不支持设备。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="6fa7a-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="6fa7a-130">inMaintenance</span></span>|<span data-ttu-id="6fa7a-131">型</span><span class="sxs-lookup"><span data-stu-id="6fa7a-131">6</span></span>|<span data-ttu-id="6fa7a-132">帐户处于维护中。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="6fa7a-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="6fa7a-133">badRequest</span></span>|<span data-ttu-id="6fa7a-134">步</span><span class="sxs-lookup"><span data-stu-id="6fa7a-134">7</span></span>|<span data-ttu-id="6fa7a-135">客户端发送了服务无法理解/支持的请求。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="6fa7a-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="6fa7a-136">featureNotSupported</span></span>|<span data-ttu-id="6fa7a-137">utf-8</span><span class="sxs-lookup"><span data-stu-id="6fa7a-137">8</span></span>|<span data-ttu-id="6fa7a-138">此帐户不支持此注册使用的功能。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="6fa7a-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="6fa7a-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="6fa7a-140">第</span><span class="sxs-lookup"><span data-stu-id="6fa7a-140">9</span></span>|<span data-ttu-id="6fa7a-141">由管理员配置的注册限制阻止了此注册。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="6fa7a-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="6fa7a-142">clientDisconnected</span></span>|<span data-ttu-id="6fa7a-143">10 </span><span class="sxs-lookup"><span data-stu-id="6fa7a-143">10</span></span>|<span data-ttu-id="6fa7a-144">客户端超时或注册被 enduser 中止。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="6fa7a-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="6fa7a-145">userAbandonment</span></span>|<span data-ttu-id="6fa7a-146">11x17</span><span class="sxs-lookup"><span data-stu-id="6fa7a-146">11</span></span>|<span data-ttu-id="6fa7a-147">注册已被 enduser 放弃。</span><span class="sxs-lookup"><span data-stu-id="6fa7a-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="6fa7a-148">（Enduser 已开始加入，但无法及时完成它）</span><span class="sxs-lookup"><span data-stu-id="6fa7a-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->


