---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶级失败类别。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 623030bccfac9e023a0d1df2dff7ea317b503485
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258329"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="85a14-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="85a14-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="85a14-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85a14-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85a14-105">注册的顶级失败类别。</span><span class="sxs-lookup"><span data-stu-id="85a14-105">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="85a14-106">成员</span><span class="sxs-lookup"><span data-stu-id="85a14-106">Members</span></span>
|<span data-ttu-id="85a14-107">成员</span><span class="sxs-lookup"><span data-stu-id="85a14-107">Member</span></span>|<span data-ttu-id="85a14-108">值</span><span class="sxs-lookup"><span data-stu-id="85a14-108">Value</span></span>|<span data-ttu-id="85a14-109">说明</span><span class="sxs-lookup"><span data-stu-id="85a14-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85a14-110">unknown</span><span class="sxs-lookup"><span data-stu-id="85a14-110">unknown</span></span>|<span data-ttu-id="85a14-111">0</span><span class="sxs-lookup"><span data-stu-id="85a14-111">0</span></span>|<span data-ttu-id="85a14-112">默认值, 失败原因未知。</span><span class="sxs-lookup"><span data-stu-id="85a14-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="85a14-113">身份验证</span><span class="sxs-lookup"><span data-stu-id="85a14-113">authentication</span></span>|<span data-ttu-id="85a14-114">1</span><span class="sxs-lookup"><span data-stu-id="85a14-114">1</span></span>|<span data-ttu-id="85a14-115">身份验证失败</span><span class="sxs-lookup"><span data-stu-id="85a14-115">Authentication failed</span></span>|
|<span data-ttu-id="85a14-116">授权</span><span class="sxs-lookup"><span data-stu-id="85a14-116">authorization</span></span>|<span data-ttu-id="85a14-117">双面</span><span class="sxs-lookup"><span data-stu-id="85a14-117">2</span></span>|<span data-ttu-id="85a14-118">呼叫已通过身份验证, 但未获授权进行注册。</span><span class="sxs-lookup"><span data-stu-id="85a14-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="85a14-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="85a14-119">accountValidation</span></span>|<span data-ttu-id="85a14-120">第三章</span><span class="sxs-lookup"><span data-stu-id="85a14-120">3</span></span>|<span data-ttu-id="85a14-121">无法验证注册帐户。</span><span class="sxs-lookup"><span data-stu-id="85a14-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="85a14-122">(帐户被阻止, 未启用注册)</span><span class="sxs-lookup"><span data-stu-id="85a14-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="85a14-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="85a14-123">userValidation</span></span>|<span data-ttu-id="85a14-124">4</span><span class="sxs-lookup"><span data-stu-id="85a14-124">4</span></span>|<span data-ttu-id="85a14-125">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="85a14-125">User could not be validated.</span></span> <span data-ttu-id="85a14-126">(用户不存在, 缺少许可证)</span><span class="sxs-lookup"><span data-stu-id="85a14-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="85a14-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="85a14-127">deviceNotSupported</span></span>|<span data-ttu-id="85a14-128">5</span><span class="sxs-lookup"><span data-stu-id="85a14-128">5</span></span>|<span data-ttu-id="85a14-129">移动设备管理不支持设备。</span><span class="sxs-lookup"><span data-stu-id="85a14-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="85a14-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="85a14-130">inMaintenance</span></span>|<span data-ttu-id="85a14-131">型</span><span class="sxs-lookup"><span data-stu-id="85a14-131">6</span></span>|<span data-ttu-id="85a14-132">帐户处于维护中。</span><span class="sxs-lookup"><span data-stu-id="85a14-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="85a14-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="85a14-133">badRequest</span></span>|<span data-ttu-id="85a14-134">步</span><span class="sxs-lookup"><span data-stu-id="85a14-134">7</span></span>|<span data-ttu-id="85a14-135">客户端发送了服务无法理解/支持的请求。</span><span class="sxs-lookup"><span data-stu-id="85a14-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="85a14-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="85a14-136">featureNotSupported</span></span>|<span data-ttu-id="85a14-137">utf-8</span><span class="sxs-lookup"><span data-stu-id="85a14-137">8</span></span>|<span data-ttu-id="85a14-138">此帐户不支持此注册使用的功能。</span><span class="sxs-lookup"><span data-stu-id="85a14-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="85a14-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="85a14-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="85a14-140">第</span><span class="sxs-lookup"><span data-stu-id="85a14-140">9</span></span>|<span data-ttu-id="85a14-141">由管理员配置的注册限制阻止了此注册。</span><span class="sxs-lookup"><span data-stu-id="85a14-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="85a14-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="85a14-142">clientDisconnected</span></span>|<span data-ttu-id="85a14-143">10</span><span class="sxs-lookup"><span data-stu-id="85a14-143">10</span></span>|<span data-ttu-id="85a14-144">客户端超时或注册被 enduser 中止。</span><span class="sxs-lookup"><span data-stu-id="85a14-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="85a14-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="85a14-145">userAbandonment</span></span>|<span data-ttu-id="85a14-146">11x17</span><span class="sxs-lookup"><span data-stu-id="85a14-146">11</span></span>|<span data-ttu-id="85a14-147">注册已被 enduser 放弃。</span><span class="sxs-lookup"><span data-stu-id="85a14-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="85a14-148">(Enduser 已开始加入, 但无法及时完成它)</span><span class="sxs-lookup"><span data-stu-id="85a14-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

