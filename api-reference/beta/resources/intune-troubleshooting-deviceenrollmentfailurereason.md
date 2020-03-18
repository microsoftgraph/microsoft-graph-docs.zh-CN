---
title: deviceEnrollmentFailureReason 枚举类型
description: 注册的顶级失败类别。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f8ab33a05a3af6eb349c563cfca78d580181228f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766012"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="4c737-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4c737-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="4c737-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4c737-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c737-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c737-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c737-106">注册的顶级失败类别。</span><span class="sxs-lookup"><span data-stu-id="4c737-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="4c737-107">成员</span><span class="sxs-lookup"><span data-stu-id="4c737-107">Members</span></span>
|<span data-ttu-id="4c737-108">成员</span><span class="sxs-lookup"><span data-stu-id="4c737-108">Member</span></span>|<span data-ttu-id="4c737-109">值</span><span class="sxs-lookup"><span data-stu-id="4c737-109">Value</span></span>|<span data-ttu-id="4c737-110">说明</span><span class="sxs-lookup"><span data-stu-id="4c737-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c737-111">unknown</span><span class="sxs-lookup"><span data-stu-id="4c737-111">unknown</span></span>|<span data-ttu-id="4c737-112">0</span><span class="sxs-lookup"><span data-stu-id="4c737-112">0</span></span>|<span data-ttu-id="4c737-113">默认值，失败原因未知。</span><span class="sxs-lookup"><span data-stu-id="4c737-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="4c737-114">authentication</span><span class="sxs-lookup"><span data-stu-id="4c737-114">authentication</span></span>|<span data-ttu-id="4c737-115">1</span><span class="sxs-lookup"><span data-stu-id="4c737-115">1</span></span>|<span data-ttu-id="4c737-116">身份验证失败</span><span class="sxs-lookup"><span data-stu-id="4c737-116">Authentication failed</span></span>|
|<span data-ttu-id="4c737-117">批准</span><span class="sxs-lookup"><span data-stu-id="4c737-117">authorization</span></span>|<span data-ttu-id="4c737-118">双面</span><span class="sxs-lookup"><span data-stu-id="4c737-118">2</span></span>|<span data-ttu-id="4c737-119">呼叫已通过身份验证，但未获授权进行注册。</span><span class="sxs-lookup"><span data-stu-id="4c737-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="4c737-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="4c737-120">accountValidation</span></span>|<span data-ttu-id="4c737-121">第三章</span><span class="sxs-lookup"><span data-stu-id="4c737-121">3</span></span>|<span data-ttu-id="4c737-122">无法验证注册帐户。</span><span class="sxs-lookup"><span data-stu-id="4c737-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="4c737-123">（帐户被阻止，未启用注册）</span><span class="sxs-lookup"><span data-stu-id="4c737-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="4c737-124">userValidation</span><span class="sxs-lookup"><span data-stu-id="4c737-124">userValidation</span></span>|<span data-ttu-id="4c737-125">4 </span><span class="sxs-lookup"><span data-stu-id="4c737-125">4</span></span>|<span data-ttu-id="4c737-126">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="4c737-126">User could not be validated.</span></span> <span data-ttu-id="4c737-127">（用户不存在，缺少许可证）</span><span class="sxs-lookup"><span data-stu-id="4c737-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="4c737-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="4c737-128">deviceNotSupported</span></span>|<span data-ttu-id="4c737-129">5 </span><span class="sxs-lookup"><span data-stu-id="4c737-129">5</span></span>|<span data-ttu-id="4c737-130">移动设备管理不支持设备。</span><span class="sxs-lookup"><span data-stu-id="4c737-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="4c737-131">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="4c737-131">inMaintenance</span></span>|<span data-ttu-id="4c737-132">6 </span><span class="sxs-lookup"><span data-stu-id="4c737-132">6</span></span>|<span data-ttu-id="4c737-133">帐户处于维护中。</span><span class="sxs-lookup"><span data-stu-id="4c737-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="4c737-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="4c737-134">badRequest</span></span>|<span data-ttu-id="4c737-135">7 </span><span class="sxs-lookup"><span data-stu-id="4c737-135">7</span></span>|<span data-ttu-id="4c737-136">客户端发送了服务无法理解/支持的请求。</span><span class="sxs-lookup"><span data-stu-id="4c737-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="4c737-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="4c737-137">featureNotSupported</span></span>|<span data-ttu-id="4c737-138">8 </span><span class="sxs-lookup"><span data-stu-id="4c737-138">8</span></span>|<span data-ttu-id="4c737-139">此帐户不支持此注册使用的功能。</span><span class="sxs-lookup"><span data-stu-id="4c737-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="4c737-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="4c737-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="4c737-141">9 </span><span class="sxs-lookup"><span data-stu-id="4c737-141">9</span></span>|<span data-ttu-id="4c737-142">由管理员配置的注册限制阻止了此注册。</span><span class="sxs-lookup"><span data-stu-id="4c737-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="4c737-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="4c737-143">clientDisconnected</span></span>|<span data-ttu-id="4c737-144">10 </span><span class="sxs-lookup"><span data-stu-id="4c737-144">10</span></span>|<span data-ttu-id="4c737-145">客户端超时或注册被 enduser 中止。</span><span class="sxs-lookup"><span data-stu-id="4c737-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="4c737-146">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="4c737-146">userAbandonment</span></span>|<span data-ttu-id="4c737-147">11x17</span><span class="sxs-lookup"><span data-stu-id="4c737-147">11</span></span>|<span data-ttu-id="4c737-148">注册已被 enduser 放弃。</span><span class="sxs-lookup"><span data-stu-id="4c737-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="4c737-149">（Enduser 已开始加入，但无法及时完成它）</span><span class="sxs-lookup"><span data-stu-id="4c737-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|



