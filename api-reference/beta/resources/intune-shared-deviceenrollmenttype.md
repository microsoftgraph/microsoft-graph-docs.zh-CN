---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 709b19896f2742f33878999ab59c1b4953ef2ca1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523707"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="5ddcf-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5ddcf-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="5ddcf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5ddcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ddcf-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ddcf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ddcf-107">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="5ddcf-108">成员</span><span class="sxs-lookup"><span data-stu-id="5ddcf-108">Members</span></span>
|<span data-ttu-id="5ddcf-109">成员</span><span class="sxs-lookup"><span data-stu-id="5ddcf-109">Member</span></span>|<span data-ttu-id="5ddcf-110">值</span><span class="sxs-lookup"><span data-stu-id="5ddcf-110">Value</span></span>|<span data-ttu-id="5ddcf-111">说明</span><span class="sxs-lookup"><span data-stu-id="5ddcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ddcf-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5ddcf-112">unknown</span></span>|<span data-ttu-id="5ddcf-113">0</span><span class="sxs-lookup"><span data-stu-id="5ddcf-113">0</span></span>|<span data-ttu-id="5ddcf-114">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="5ddcf-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="5ddcf-115">userEnrollment</span></span>|<span data-ttu-id="5ddcf-116">1 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-116">1</span></span>|<span data-ttu-id="5ddcf-117">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="5ddcf-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="5ddcf-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="5ddcf-119">2 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-119">2</span></span>|<span data-ttu-id="5ddcf-120">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="5ddcf-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="5ddcf-121">appleBulkWithUser</span></span>|<span data-ttu-id="5ddcf-122">3 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-122">3</span></span>|<span data-ttu-id="5ddcf-123">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="5ddcf-124">（DEP、Apple 配置器）</span><span class="sxs-lookup"><span data-stu-id="5ddcf-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="5ddcf-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="5ddcf-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="5ddcf-126">4 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-126">4</span></span>|<span data-ttu-id="5ddcf-127">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="5ddcf-128">（DEP、Apple 配置器、移动配置）</span><span class="sxs-lookup"><span data-stu-id="5ddcf-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="5ddcf-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="5ddcf-129">windowsAzureADJoin</span></span>|<span data-ttu-id="5ddcf-130">5 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-130">5</span></span>|<span data-ttu-id="5ddcf-131">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="5ddcf-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="5ddcf-132">windowsBulkUserless</span></span>|<span data-ttu-id="5ddcf-133">6 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-133">6</span></span>|<span data-ttu-id="5ddcf-134">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="5ddcf-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="5ddcf-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="5ddcf-136">7 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-136">7</span></span>|<span data-ttu-id="5ddcf-137">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="5ddcf-138">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="5ddcf-138">(Add work account)</span></span>|
|<span data-ttu-id="5ddcf-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="5ddcf-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="5ddcf-140">8 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-140">8</span></span>|<span data-ttu-id="5ddcf-141">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="5ddcf-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="5ddcf-142">windowsCoManagement</span></span>|<span data-ttu-id="5ddcf-143">9 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-143">9</span></span>|<span data-ttu-id="5ddcf-144">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="5ddcf-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|
|<span data-ttu-id="5ddcf-145">appleUserEnrollment</span><span class="sxs-lookup"><span data-stu-id="5ddcf-145">appleUserEnrollment</span></span>|<span data-ttu-id="5ddcf-146">11 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-146">11</span></span>|<span data-ttu-id="5ddcf-147">由 Apple 用户注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="5ddcf-147">Device managed by Apple user enrollment</span></span>|
|<span data-ttu-id="5ddcf-148">appleUserEnrollmentWithServiceAccount</span><span class="sxs-lookup"><span data-stu-id="5ddcf-148">appleUserEnrollmentWithServiceAccount</span></span>|<span data-ttu-id="5ddcf-149">12 </span><span class="sxs-lookup"><span data-stu-id="5ddcf-149">12</span></span>|<span data-ttu-id="5ddcf-150">由 Apple 用户使用服务帐户进行注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="5ddcf-150">Device managed by Apple user enrollment with service account</span></span>|



