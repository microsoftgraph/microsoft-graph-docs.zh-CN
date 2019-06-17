---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶级失败类别。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e932a86cef5c15d3a6d41cc424b1acfdf4c95a7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991014"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="90492-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="90492-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="90492-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90492-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90492-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90492-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90492-106">注册的顶级失败类别。</span><span class="sxs-lookup"><span data-stu-id="90492-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="90492-107">成员</span><span class="sxs-lookup"><span data-stu-id="90492-107">Members</span></span>
|<span data-ttu-id="90492-108">成员</span><span class="sxs-lookup"><span data-stu-id="90492-108">Member</span></span>|<span data-ttu-id="90492-109">值</span><span class="sxs-lookup"><span data-stu-id="90492-109">Value</span></span>|<span data-ttu-id="90492-110">说明</span><span class="sxs-lookup"><span data-stu-id="90492-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90492-111">unknown</span><span class="sxs-lookup"><span data-stu-id="90492-111">unknown</span></span>|<span data-ttu-id="90492-112">0</span><span class="sxs-lookup"><span data-stu-id="90492-112">0</span></span>|<span data-ttu-id="90492-113">默认值, 失败原因未知。</span><span class="sxs-lookup"><span data-stu-id="90492-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="90492-114">authentication</span><span class="sxs-lookup"><span data-stu-id="90492-114">authentication</span></span>|<span data-ttu-id="90492-115">1</span><span class="sxs-lookup"><span data-stu-id="90492-115">1</span></span>|<span data-ttu-id="90492-116">身份验证失败</span><span class="sxs-lookup"><span data-stu-id="90492-116">Authentication failed</span></span>|
|<span data-ttu-id="90492-117">批准</span><span class="sxs-lookup"><span data-stu-id="90492-117">authorization</span></span>|<span data-ttu-id="90492-118">双面</span><span class="sxs-lookup"><span data-stu-id="90492-118">2</span></span>|<span data-ttu-id="90492-119">呼叫已通过身份验证, 但未获授权进行注册。</span><span class="sxs-lookup"><span data-stu-id="90492-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="90492-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="90492-120">accountValidation</span></span>|<span data-ttu-id="90492-121">第三章</span><span class="sxs-lookup"><span data-stu-id="90492-121">3</span></span>|<span data-ttu-id="90492-122">无法验证注册帐户。</span><span class="sxs-lookup"><span data-stu-id="90492-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="90492-123">(帐户被阻止, 未启用注册)</span><span class="sxs-lookup"><span data-stu-id="90492-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="90492-124">userValidation</span><span class="sxs-lookup"><span data-stu-id="90492-124">userValidation</span></span>|<span data-ttu-id="90492-125">4</span><span class="sxs-lookup"><span data-stu-id="90492-125">4</span></span>|<span data-ttu-id="90492-126">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="90492-126">User could not be validated.</span></span> <span data-ttu-id="90492-127">(用户不存在, 缺少许可证)</span><span class="sxs-lookup"><span data-stu-id="90492-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="90492-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="90492-128">deviceNotSupported</span></span>|<span data-ttu-id="90492-129">5</span><span class="sxs-lookup"><span data-stu-id="90492-129">5</span></span>|<span data-ttu-id="90492-130">移动设备管理不支持设备。</span><span class="sxs-lookup"><span data-stu-id="90492-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="90492-131">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="90492-131">inMaintenance</span></span>|<span data-ttu-id="90492-132">型</span><span class="sxs-lookup"><span data-stu-id="90492-132">6</span></span>|<span data-ttu-id="90492-133">帐户处于维护中。</span><span class="sxs-lookup"><span data-stu-id="90492-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="90492-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="90492-134">badRequest</span></span>|<span data-ttu-id="90492-135">步</span><span class="sxs-lookup"><span data-stu-id="90492-135">7</span></span>|<span data-ttu-id="90492-136">客户端发送了服务无法理解/支持的请求。</span><span class="sxs-lookup"><span data-stu-id="90492-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="90492-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="90492-137">featureNotSupported</span></span>|<span data-ttu-id="90492-138">utf-8</span><span class="sxs-lookup"><span data-stu-id="90492-138">8</span></span>|<span data-ttu-id="90492-139">此帐户不支持此注册使用的功能。</span><span class="sxs-lookup"><span data-stu-id="90492-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="90492-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="90492-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="90492-141">第</span><span class="sxs-lookup"><span data-stu-id="90492-141">9</span></span>|<span data-ttu-id="90492-142">由管理员配置的注册限制阻止了此注册。</span><span class="sxs-lookup"><span data-stu-id="90492-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="90492-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="90492-143">clientDisconnected</span></span>|<span data-ttu-id="90492-144">10 </span><span class="sxs-lookup"><span data-stu-id="90492-144">10</span></span>|<span data-ttu-id="90492-145">客户端超时或注册被 enduser 中止。</span><span class="sxs-lookup"><span data-stu-id="90492-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="90492-146">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="90492-146">userAbandonment</span></span>|<span data-ttu-id="90492-147">11x17</span><span class="sxs-lookup"><span data-stu-id="90492-147">11</span></span>|<span data-ttu-id="90492-148">注册已被 enduser 放弃。</span><span class="sxs-lookup"><span data-stu-id="90492-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="90492-149">(Enduser 已开始加入, 但无法及时完成它)</span><span class="sxs-lookup"><span data-stu-id="90492-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|





