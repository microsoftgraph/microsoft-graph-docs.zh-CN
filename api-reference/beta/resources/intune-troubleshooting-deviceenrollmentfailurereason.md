---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶级失败类别。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a0721495a8eb217007c0ee1f18942009614696d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010313"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="7410e-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7410e-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="7410e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7410e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7410e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7410e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7410e-106">注册的顶级失败类别。</span><span class="sxs-lookup"><span data-stu-id="7410e-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="7410e-107">成员</span><span class="sxs-lookup"><span data-stu-id="7410e-107">Members</span></span>
|<span data-ttu-id="7410e-108">成员</span><span class="sxs-lookup"><span data-stu-id="7410e-108">Member</span></span>|<span data-ttu-id="7410e-109">值</span><span class="sxs-lookup"><span data-stu-id="7410e-109">Value</span></span>|<span data-ttu-id="7410e-110">说明</span><span class="sxs-lookup"><span data-stu-id="7410e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7410e-111">unknown</span><span class="sxs-lookup"><span data-stu-id="7410e-111">unknown</span></span>|<span data-ttu-id="7410e-112">0</span><span class="sxs-lookup"><span data-stu-id="7410e-112">0</span></span>|<span data-ttu-id="7410e-113">默认值, 失败原因未知。</span><span class="sxs-lookup"><span data-stu-id="7410e-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="7410e-114">authentication</span><span class="sxs-lookup"><span data-stu-id="7410e-114">authentication</span></span>|<span data-ttu-id="7410e-115">1</span><span class="sxs-lookup"><span data-stu-id="7410e-115">1</span></span>|<span data-ttu-id="7410e-116">身份验证失败</span><span class="sxs-lookup"><span data-stu-id="7410e-116">Authentication failed</span></span>|
|<span data-ttu-id="7410e-117">批准</span><span class="sxs-lookup"><span data-stu-id="7410e-117">authorization</span></span>|<span data-ttu-id="7410e-118">双面</span><span class="sxs-lookup"><span data-stu-id="7410e-118">2</span></span>|<span data-ttu-id="7410e-119">呼叫已通过身份验证, 但未获授权进行注册。</span><span class="sxs-lookup"><span data-stu-id="7410e-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="7410e-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="7410e-120">accountValidation</span></span>|<span data-ttu-id="7410e-121">第三章</span><span class="sxs-lookup"><span data-stu-id="7410e-121">3</span></span>|<span data-ttu-id="7410e-122">无法验证注册帐户。</span><span class="sxs-lookup"><span data-stu-id="7410e-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="7410e-123">(帐户被阻止, 未启用注册)</span><span class="sxs-lookup"><span data-stu-id="7410e-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="7410e-124">userValidation</span><span class="sxs-lookup"><span data-stu-id="7410e-124">userValidation</span></span>|<span data-ttu-id="7410e-125">4</span><span class="sxs-lookup"><span data-stu-id="7410e-125">4</span></span>|<span data-ttu-id="7410e-126">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="7410e-126">User could not be validated.</span></span> <span data-ttu-id="7410e-127">(用户不存在, 缺少许可证)</span><span class="sxs-lookup"><span data-stu-id="7410e-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="7410e-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="7410e-128">deviceNotSupported</span></span>|<span data-ttu-id="7410e-129">5</span><span class="sxs-lookup"><span data-stu-id="7410e-129">5</span></span>|<span data-ttu-id="7410e-130">移动设备管理不支持设备。</span><span class="sxs-lookup"><span data-stu-id="7410e-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="7410e-131">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="7410e-131">inMaintenance</span></span>|<span data-ttu-id="7410e-132">型</span><span class="sxs-lookup"><span data-stu-id="7410e-132">6</span></span>|<span data-ttu-id="7410e-133">帐户处于维护中。</span><span class="sxs-lookup"><span data-stu-id="7410e-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="7410e-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="7410e-134">badRequest</span></span>|<span data-ttu-id="7410e-135">步</span><span class="sxs-lookup"><span data-stu-id="7410e-135">7</span></span>|<span data-ttu-id="7410e-136">客户端发送了服务无法理解/支持的请求。</span><span class="sxs-lookup"><span data-stu-id="7410e-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="7410e-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="7410e-137">featureNotSupported</span></span>|<span data-ttu-id="7410e-138">utf-8</span><span class="sxs-lookup"><span data-stu-id="7410e-138">8</span></span>|<span data-ttu-id="7410e-139">此帐户不支持此注册使用的功能。</span><span class="sxs-lookup"><span data-stu-id="7410e-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="7410e-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="7410e-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="7410e-141">第</span><span class="sxs-lookup"><span data-stu-id="7410e-141">9</span></span>|<span data-ttu-id="7410e-142">由管理员配置的注册限制阻止了此注册。</span><span class="sxs-lookup"><span data-stu-id="7410e-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="7410e-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="7410e-143">clientDisconnected</span></span>|<span data-ttu-id="7410e-144">10 </span><span class="sxs-lookup"><span data-stu-id="7410e-144">10</span></span>|<span data-ttu-id="7410e-145">客户端超时或注册被 enduser 中止。</span><span class="sxs-lookup"><span data-stu-id="7410e-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="7410e-146">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="7410e-146">userAbandonment</span></span>|<span data-ttu-id="7410e-147">11x17</span><span class="sxs-lookup"><span data-stu-id="7410e-147">11</span></span>|<span data-ttu-id="7410e-148">注册已被 enduser 放弃。</span><span class="sxs-lookup"><span data-stu-id="7410e-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="7410e-149">(Enduser 已开始加入, 但无法及时完成它)</span><span class="sxs-lookup"><span data-stu-id="7410e-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|





