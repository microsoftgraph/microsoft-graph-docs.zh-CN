---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶级失败类别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4d975f554c426bf8050b5603b0b4fb1d2297f8b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255376"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="e246f-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e246f-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="e246f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e246f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e246f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e246f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e246f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e246f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e246f-107">注册的顶级失败类别。</span><span class="sxs-lookup"><span data-stu-id="e246f-107">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="e246f-108">成员</span><span class="sxs-lookup"><span data-stu-id="e246f-108">Members</span></span>
|<span data-ttu-id="e246f-109">成员</span><span class="sxs-lookup"><span data-stu-id="e246f-109">Member</span></span>|<span data-ttu-id="e246f-110">值</span><span class="sxs-lookup"><span data-stu-id="e246f-110">Value</span></span>|<span data-ttu-id="e246f-111">说明</span><span class="sxs-lookup"><span data-stu-id="e246f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e246f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e246f-112">unknown</span></span>|<span data-ttu-id="e246f-113">0</span><span class="sxs-lookup"><span data-stu-id="e246f-113">0</span></span>|<span data-ttu-id="e246f-114">默认值，失败原因未知。</span><span class="sxs-lookup"><span data-stu-id="e246f-114">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="e246f-115">authentication</span><span class="sxs-lookup"><span data-stu-id="e246f-115">authentication</span></span>|<span data-ttu-id="e246f-116">1</span><span class="sxs-lookup"><span data-stu-id="e246f-116">1</span></span>|<span data-ttu-id="e246f-117">身份验证失败</span><span class="sxs-lookup"><span data-stu-id="e246f-117">Authentication failed</span></span>|
|<span data-ttu-id="e246f-118">批准</span><span class="sxs-lookup"><span data-stu-id="e246f-118">authorization</span></span>|<span data-ttu-id="e246f-119">双面</span><span class="sxs-lookup"><span data-stu-id="e246f-119">2</span></span>|<span data-ttu-id="e246f-120">呼叫已通过身份验证，但未获授权进行注册。</span><span class="sxs-lookup"><span data-stu-id="e246f-120">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="e246f-121">accountValidation</span><span class="sxs-lookup"><span data-stu-id="e246f-121">accountValidation</span></span>|<span data-ttu-id="e246f-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e246f-122">3</span></span>|<span data-ttu-id="e246f-123">无法验证注册帐户。</span><span class="sxs-lookup"><span data-stu-id="e246f-123">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="e246f-124"> (帐户已被阻止，未启用注册) </span><span class="sxs-lookup"><span data-stu-id="e246f-124">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="e246f-125">userValidation</span><span class="sxs-lookup"><span data-stu-id="e246f-125">userValidation</span></span>|<span data-ttu-id="e246f-126">4 </span><span class="sxs-lookup"><span data-stu-id="e246f-126">4</span></span>|<span data-ttu-id="e246f-127">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="e246f-127">User could not be validated.</span></span> <span data-ttu-id="e246f-128"> (用户不存在，缺少许可证) </span><span class="sxs-lookup"><span data-stu-id="e246f-128">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="e246f-129">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="e246f-129">deviceNotSupported</span></span>|<span data-ttu-id="e246f-130">5 </span><span class="sxs-lookup"><span data-stu-id="e246f-130">5</span></span>|<span data-ttu-id="e246f-131">移动设备管理不支持设备。</span><span class="sxs-lookup"><span data-stu-id="e246f-131">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="e246f-132">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="e246f-132">inMaintenance</span></span>|<span data-ttu-id="e246f-133">6 </span><span class="sxs-lookup"><span data-stu-id="e246f-133">6</span></span>|<span data-ttu-id="e246f-134">帐户处于维护中。</span><span class="sxs-lookup"><span data-stu-id="e246f-134">Account is in maintenance.</span></span>|
|<span data-ttu-id="e246f-135">badRequest</span><span class="sxs-lookup"><span data-stu-id="e246f-135">badRequest</span></span>|<span data-ttu-id="e246f-136">7 </span><span class="sxs-lookup"><span data-stu-id="e246f-136">7</span></span>|<span data-ttu-id="e246f-137">客户端发送了服务无法理解/支持的请求。</span><span class="sxs-lookup"><span data-stu-id="e246f-137">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="e246f-138">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="e246f-138">featureNotSupported</span></span>|<span data-ttu-id="e246f-139">8 </span><span class="sxs-lookup"><span data-stu-id="e246f-139">8</span></span>|<span data-ttu-id="e246f-140">此帐户不支持此注册使用的功能 (s) 。</span><span class="sxs-lookup"><span data-stu-id="e246f-140">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="e246f-141">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="e246f-141">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="e246f-142">9 </span><span class="sxs-lookup"><span data-stu-id="e246f-142">9</span></span>|<span data-ttu-id="e246f-143">由管理员配置的注册限制阻止了此注册。</span><span class="sxs-lookup"><span data-stu-id="e246f-143">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="e246f-144">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="e246f-144">clientDisconnected</span></span>|<span data-ttu-id="e246f-145">10  </span><span class="sxs-lookup"><span data-stu-id="e246f-145">10</span></span>|<span data-ttu-id="e246f-146">客户端超时或注册被 enduser 中止。</span><span class="sxs-lookup"><span data-stu-id="e246f-146">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="e246f-147">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="e246f-147">userAbandonment</span></span>|<span data-ttu-id="e246f-148">11 </span><span class="sxs-lookup"><span data-stu-id="e246f-148">11</span></span>|<span data-ttu-id="e246f-149">注册已被 enduser 放弃。</span><span class="sxs-lookup"><span data-stu-id="e246f-149">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="e246f-150"> (Enduser 已开始加入，但无法及时完成它) </span><span class="sxs-lookup"><span data-stu-id="e246f-150">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|




