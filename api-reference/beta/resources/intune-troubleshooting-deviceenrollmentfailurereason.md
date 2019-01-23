---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶部级别故障类别。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fbfe7193c72f1ff1a03a7e7bb4da57d0a032e530
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396208"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="c37f5-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c37f5-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="c37f5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c37f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c37f5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c37f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c37f5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c37f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c37f5-107">注册的顶部级别故障类别。</span><span class="sxs-lookup"><span data-stu-id="c37f5-107">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="c37f5-108">成员</span><span class="sxs-lookup"><span data-stu-id="c37f5-108">Members</span></span>
|<span data-ttu-id="c37f5-109">成员</span><span class="sxs-lookup"><span data-stu-id="c37f5-109">Member</span></span>|<span data-ttu-id="c37f5-110">值</span><span class="sxs-lookup"><span data-stu-id="c37f5-110">Value</span></span>|<span data-ttu-id="c37f5-111">说明</span><span class="sxs-lookup"><span data-stu-id="c37f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c37f5-112">unknown</span><span class="sxs-lookup"><span data-stu-id="c37f5-112">unknown</span></span>|<span data-ttu-id="c37f5-113">0</span><span class="sxs-lookup"><span data-stu-id="c37f5-113">0</span></span>|<span data-ttu-id="c37f5-114">默认值是未知失败原因。</span><span class="sxs-lookup"><span data-stu-id="c37f5-114">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="c37f5-115">身份验证</span><span class="sxs-lookup"><span data-stu-id="c37f5-115">authentication</span></span>|<span data-ttu-id="c37f5-116">1</span><span class="sxs-lookup"><span data-stu-id="c37f5-116">1</span></span>|<span data-ttu-id="c37f5-117">失败的身份验证</span><span class="sxs-lookup"><span data-stu-id="c37f5-117">Authentication failed</span></span>|
|<span data-ttu-id="c37f5-118">授权</span><span class="sxs-lookup"><span data-stu-id="c37f5-118">authorization</span></span>|<span data-ttu-id="c37f5-119">2</span><span class="sxs-lookup"><span data-stu-id="c37f5-119">2</span></span>|<span data-ttu-id="c37f5-120">呼叫已通过身份验证，但未被授权注册。</span><span class="sxs-lookup"><span data-stu-id="c37f5-120">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="c37f5-121">accountValidation</span><span class="sxs-lookup"><span data-stu-id="c37f5-121">accountValidation</span></span>|<span data-ttu-id="c37f5-122">3</span><span class="sxs-lookup"><span data-stu-id="c37f5-122">3</span></span>|<span data-ttu-id="c37f5-123">无法验证注册的帐户。</span><span class="sxs-lookup"><span data-stu-id="c37f5-123">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="c37f5-124">（帐户已被阻止，注册未启用）</span><span class="sxs-lookup"><span data-stu-id="c37f5-124">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="c37f5-125">userValidation</span><span class="sxs-lookup"><span data-stu-id="c37f5-125">userValidation</span></span>|<span data-ttu-id="c37f5-126">4</span><span class="sxs-lookup"><span data-stu-id="c37f5-126">4</span></span>|<span data-ttu-id="c37f5-127">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="c37f5-127">User could not be validated.</span></span> <span data-ttu-id="c37f5-128">(不存在用户，缺少许可证)</span><span class="sxs-lookup"><span data-stu-id="c37f5-128">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="c37f5-129">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="c37f5-129">deviceNotSupported</span></span>|<span data-ttu-id="c37f5-130">5</span><span class="sxs-lookup"><span data-stu-id="c37f5-130">5</span></span>|<span data-ttu-id="c37f5-131">不支持移动设备管理设备。</span><span class="sxs-lookup"><span data-stu-id="c37f5-131">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="c37f5-132">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="c37f5-132">inMaintenance</span></span>|<span data-ttu-id="c37f5-133">6</span><span class="sxs-lookup"><span data-stu-id="c37f5-133">6</span></span>|<span data-ttu-id="c37f5-134">帐户是在维护。</span><span class="sxs-lookup"><span data-stu-id="c37f5-134">Account is in maintenance.</span></span>|
|<span data-ttu-id="c37f5-135">badRequest</span><span class="sxs-lookup"><span data-stu-id="c37f5-135">badRequest</span></span>|<span data-ttu-id="c37f5-136">7</span><span class="sxs-lookup"><span data-stu-id="c37f5-136">7</span></span>|<span data-ttu-id="c37f5-137">客户端发送请求不是服务理解/支持。</span><span class="sxs-lookup"><span data-stu-id="c37f5-137">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="c37f5-138">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="c37f5-138">featureNotSupported</span></span>|<span data-ttu-id="c37f5-139">8</span><span class="sxs-lookup"><span data-stu-id="c37f5-139">8</span></span>|<span data-ttu-id="c37f5-140">此帐户不支持使用此注册的功能。</span><span class="sxs-lookup"><span data-stu-id="c37f5-140">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="c37f5-141">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="c37f5-141">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="c37f5-142">9</span><span class="sxs-lookup"><span data-stu-id="c37f5-142">9</span></span>|<span data-ttu-id="c37f5-143">注册限制配置被管理员阻止此注册。</span><span class="sxs-lookup"><span data-stu-id="c37f5-143">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="c37f5-144">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="c37f5-144">clientDisconnected</span></span>|<span data-ttu-id="c37f5-145">10</span><span class="sxs-lookup"><span data-stu-id="c37f5-145">10</span></span>|<span data-ttu-id="c37f5-146">客户端超时或注册已中止由最终用户。</span><span class="sxs-lookup"><span data-stu-id="c37f5-146">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="c37f5-147">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="c37f5-147">userAbandonment</span></span>|<span data-ttu-id="c37f5-148">11</span><span class="sxs-lookup"><span data-stu-id="c37f5-148">11</span></span>|<span data-ttu-id="c37f5-149">注册已放弃的最终用户。</span><span class="sxs-lookup"><span data-stu-id="c37f5-149">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="c37f5-150">（最终用户启动入职培训，但无法完成及时）</span><span class="sxs-lookup"><span data-stu-id="c37f5-150">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|




