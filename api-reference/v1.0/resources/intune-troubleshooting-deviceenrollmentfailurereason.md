---
title: deviceEnrollmentFailureReason 枚举类型
description: 用于注册的顶级失败类别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ee798d2cd9c21038cff177320b3a3ae37d05f2e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732348"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="93358-103">deviceEnrollmentFailureReason 枚举类型</span><span class="sxs-lookup"><span data-stu-id="93358-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="93358-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93358-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93358-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93358-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93358-106">用于注册的顶级失败类别。</span><span class="sxs-lookup"><span data-stu-id="93358-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="93358-107">成员</span><span class="sxs-lookup"><span data-stu-id="93358-107">Members</span></span>
|<span data-ttu-id="93358-108">成员</span><span class="sxs-lookup"><span data-stu-id="93358-108">Member</span></span>|<span data-ttu-id="93358-109">值</span><span class="sxs-lookup"><span data-stu-id="93358-109">Value</span></span>|<span data-ttu-id="93358-110">Description</span><span class="sxs-lookup"><span data-stu-id="93358-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93358-111">unknown</span><span class="sxs-lookup"><span data-stu-id="93358-111">unknown</span></span>|<span data-ttu-id="93358-112">0</span><span class="sxs-lookup"><span data-stu-id="93358-112">0</span></span>|<span data-ttu-id="93358-113">默认值，失败原因未知。</span><span class="sxs-lookup"><span data-stu-id="93358-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="93358-114">身份验证</span><span class="sxs-lookup"><span data-stu-id="93358-114">authentication</span></span>|<span data-ttu-id="93358-115">1</span><span class="sxs-lookup"><span data-stu-id="93358-115">1</span></span>|<span data-ttu-id="93358-116">身份验证失败</span><span class="sxs-lookup"><span data-stu-id="93358-116">Authentication failed</span></span>|
|<span data-ttu-id="93358-117">authorization</span><span class="sxs-lookup"><span data-stu-id="93358-117">authorization</span></span>|<span data-ttu-id="93358-118">2</span><span class="sxs-lookup"><span data-stu-id="93358-118">2</span></span>|<span data-ttu-id="93358-119">呼叫已通过身份验证，但无权注册。</span><span class="sxs-lookup"><span data-stu-id="93358-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="93358-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="93358-120">accountValidation</span></span>|<span data-ttu-id="93358-121">3</span><span class="sxs-lookup"><span data-stu-id="93358-121">3</span></span>|<span data-ttu-id="93358-122">未能验证帐户注册。</span><span class="sxs-lookup"><span data-stu-id="93358-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="93358-123"> (帐户被阻止，未启用) </span><span class="sxs-lookup"><span data-stu-id="93358-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="93358-124">userValidation</span><span class="sxs-lookup"><span data-stu-id="93358-124">userValidation</span></span>|<span data-ttu-id="93358-125">4 </span><span class="sxs-lookup"><span data-stu-id="93358-125">4</span></span>|<span data-ttu-id="93358-126">无法验证用户。</span><span class="sxs-lookup"><span data-stu-id="93358-126">User could not be validated.</span></span> <span data-ttu-id="93358-127"> (用户不存在，缺少许可证) </span><span class="sxs-lookup"><span data-stu-id="93358-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="93358-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="93358-128">deviceNotSupported</span></span>|<span data-ttu-id="93358-129">5 </span><span class="sxs-lookup"><span data-stu-id="93358-129">5</span></span>|<span data-ttu-id="93358-130">移动设备管理不支持设备。</span><span class="sxs-lookup"><span data-stu-id="93358-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="93358-131">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="93358-131">inMaintenance</span></span>|<span data-ttu-id="93358-132">6 </span><span class="sxs-lookup"><span data-stu-id="93358-132">6</span></span>|<span data-ttu-id="93358-133">帐户在维护中。</span><span class="sxs-lookup"><span data-stu-id="93358-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="93358-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="93358-134">badRequest</span></span>|<span data-ttu-id="93358-135">7 </span><span class="sxs-lookup"><span data-stu-id="93358-135">7</span></span>|<span data-ttu-id="93358-136">客户端发送了服务无法理解/不支持的请求。</span><span class="sxs-lookup"><span data-stu-id="93358-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="93358-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="93358-137">featureNotSupported</span></span>|<span data-ttu-id="93358-138">8 </span><span class="sxs-lookup"><span data-stu-id="93358-138">8</span></span>|<span data-ttu-id="93358-139">此 () 不支持此注册使用的功能。</span><span class="sxs-lookup"><span data-stu-id="93358-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="93358-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="93358-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="93358-141">9 </span><span class="sxs-lookup"><span data-stu-id="93358-141">9</span></span>|<span data-ttu-id="93358-142">管理员配置的注册限制阻止了此注册。</span><span class="sxs-lookup"><span data-stu-id="93358-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="93358-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="93358-143">clientDisconnected</span></span>|<span data-ttu-id="93358-144">10  </span><span class="sxs-lookup"><span data-stu-id="93358-144">10</span></span>|<span data-ttu-id="93358-145">客户端已暂停或注册已由最终用户中止。</span><span class="sxs-lookup"><span data-stu-id="93358-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="93358-146">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="93358-146">userAbandonment</span></span>|<span data-ttu-id="93358-147">11</span><span class="sxs-lookup"><span data-stu-id="93358-147">11</span></span>|<span data-ttu-id="93358-148">最终用户已放弃注册。</span><span class="sxs-lookup"><span data-stu-id="93358-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="93358-149"> (Enduser 开始载入，但未能及时完成) </span><span class="sxs-lookup"><span data-stu-id="93358-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->







