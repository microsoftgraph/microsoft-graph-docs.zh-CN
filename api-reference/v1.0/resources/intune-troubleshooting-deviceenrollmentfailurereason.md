---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶部级别故障类别。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd7ba949c95d507d956dd7f315b3c19e0759c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885524"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="a3409-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a3409-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="a3409-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a3409-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3409-105">注册的顶部级别故障类别。</span><span class="sxs-lookup"><span data-stu-id="a3409-105">Top level failure categories for enrollment.</span></span>
## <a name="members"></a><span data-ttu-id="a3409-106">成员</span><span class="sxs-lookup"><span data-stu-id="a3409-106">Members</span></span>
|<span data-ttu-id="a3409-107">成员</span><span class="sxs-lookup"><span data-stu-id="a3409-107">Member</span></span>|<span data-ttu-id="a3409-108">值</span><span class="sxs-lookup"><span data-stu-id="a3409-108">Value</span></span>|<span data-ttu-id="a3409-109">Description</span><span class="sxs-lookup"><span data-stu-id="a3409-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3409-110">unknown</span><span class="sxs-lookup"><span data-stu-id="a3409-110">unknown</span></span>|<span data-ttu-id="a3409-111">0</span><span class="sxs-lookup"><span data-stu-id="a3409-111">0</span></span>|<span data-ttu-id="a3409-112">默认值是未知失败原因。</span><span class="sxs-lookup"><span data-stu-id="a3409-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="a3409-113">身份验证</span><span class="sxs-lookup"><span data-stu-id="a3409-113">authentication</span></span>|<span data-ttu-id="a3409-114">1</span><span class="sxs-lookup"><span data-stu-id="a3409-114">1</span></span>|<span data-ttu-id="a3409-115">失败的身份验证</span><span class="sxs-lookup"><span data-stu-id="a3409-115">Authentication failed</span></span>|
|<span data-ttu-id="a3409-116">授权</span><span class="sxs-lookup"><span data-stu-id="a3409-116">authorization</span></span>|<span data-ttu-id="a3409-117">2</span><span class="sxs-lookup"><span data-stu-id="a3409-117">2</span></span>|<span data-ttu-id="a3409-118">呼叫已通过身份验证，但未被授权注册。</span><span class="sxs-lookup"><span data-stu-id="a3409-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="a3409-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="a3409-119">accountValidation</span></span>|<span data-ttu-id="a3409-120">3</span><span class="sxs-lookup"><span data-stu-id="a3409-120">3</span></span>|<span data-ttu-id="a3409-121">无法验证注册的帐户。</span><span class="sxs-lookup"><span data-stu-id="a3409-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="a3409-122">（帐户已被阻止，注册未启用）</span><span class="sxs-lookup"><span data-stu-id="a3409-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="a3409-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="a3409-123">userValidation</span></span>|<span data-ttu-id="a3409-124">4</span><span class="sxs-lookup"><span data-stu-id="a3409-124">4</span></span>|<span data-ttu-id="a3409-125">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="a3409-125">User could not be validated.</span></span> <span data-ttu-id="a3409-126">(不存在用户，缺少许可证)</span><span class="sxs-lookup"><span data-stu-id="a3409-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="a3409-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="a3409-127">deviceNotSupported</span></span>|<span data-ttu-id="a3409-128">5</span><span class="sxs-lookup"><span data-stu-id="a3409-128">5</span></span>|<span data-ttu-id="a3409-129">不支持移动设备管理设备。</span><span class="sxs-lookup"><span data-stu-id="a3409-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="a3409-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="a3409-130">inMaintenance</span></span>|<span data-ttu-id="a3409-131">6</span><span class="sxs-lookup"><span data-stu-id="a3409-131">6</span></span>|<span data-ttu-id="a3409-132">帐户是在维护。</span><span class="sxs-lookup"><span data-stu-id="a3409-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="a3409-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="a3409-133">badRequest</span></span>|<span data-ttu-id="a3409-134">7</span><span class="sxs-lookup"><span data-stu-id="a3409-134">7</span></span>|<span data-ttu-id="a3409-135">客户端发送请求不是服务理解/支持。</span><span class="sxs-lookup"><span data-stu-id="a3409-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="a3409-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="a3409-136">featureNotSupported</span></span>|<span data-ttu-id="a3409-137">8</span><span class="sxs-lookup"><span data-stu-id="a3409-137">8</span></span>|<span data-ttu-id="a3409-138">此帐户不支持使用此注册的功能。</span><span class="sxs-lookup"><span data-stu-id="a3409-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="a3409-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="a3409-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="a3409-140">9</span><span class="sxs-lookup"><span data-stu-id="a3409-140">9</span></span>|<span data-ttu-id="a3409-141">注册限制配置被管理员阻止此注册。</span><span class="sxs-lookup"><span data-stu-id="a3409-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="a3409-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="a3409-142">clientDisconnected</span></span>|<span data-ttu-id="a3409-143">10</span><span class="sxs-lookup"><span data-stu-id="a3409-143">10</span></span>|<span data-ttu-id="a3409-144">客户端超时或注册已中止由最终用户。</span><span class="sxs-lookup"><span data-stu-id="a3409-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="a3409-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="a3409-145">userAbandonment</span></span>|<span data-ttu-id="a3409-146">11</span><span class="sxs-lookup"><span data-stu-id="a3409-146">11</span></span>|<span data-ttu-id="a3409-147">注册已放弃的最终用户。</span><span class="sxs-lookup"><span data-stu-id="a3409-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="a3409-148">（最终用户启动入职培训，但无法完成及时）</span><span class="sxs-lookup"><span data-stu-id="a3409-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
