---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68910dececddb812c8c5ac25c02020ac9370edcb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458319"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="4b3e1-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4b3e1-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="4b3e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b3e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b3e1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b3e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b3e1-107">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="4b3e1-108">成员</span><span class="sxs-lookup"><span data-stu-id="4b3e1-108">Members</span></span>
|<span data-ttu-id="4b3e1-109">成员</span><span class="sxs-lookup"><span data-stu-id="4b3e1-109">Member</span></span>|<span data-ttu-id="4b3e1-110">值</span><span class="sxs-lookup"><span data-stu-id="4b3e1-110">Value</span></span>|<span data-ttu-id="4b3e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b3e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b3e1-112">unknown</span><span class="sxs-lookup"><span data-stu-id="4b3e1-112">unknown</span></span>|<span data-ttu-id="4b3e1-113">0</span><span class="sxs-lookup"><span data-stu-id="4b3e1-113">0</span></span>|<span data-ttu-id="4b3e1-114">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="4b3e1-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="4b3e1-115">userEnrollment</span></span>|<span data-ttu-id="4b3e1-116">1</span><span class="sxs-lookup"><span data-stu-id="4b3e1-116">1</span></span>|<span data-ttu-id="4b3e1-117">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="4b3e1-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="4b3e1-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="4b3e1-119">双面</span><span class="sxs-lookup"><span data-stu-id="4b3e1-119">2</span></span>|<span data-ttu-id="4b3e1-120">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="4b3e1-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="4b3e1-121">appleBulkWithUser</span></span>|<span data-ttu-id="4b3e1-122">第三章</span><span class="sxs-lookup"><span data-stu-id="4b3e1-122">3</span></span>|<span data-ttu-id="4b3e1-123">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="4b3e1-124">（DEP、Apple 配置器）</span><span class="sxs-lookup"><span data-stu-id="4b3e1-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="4b3e1-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="4b3e1-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="4b3e1-126">4 </span><span class="sxs-lookup"><span data-stu-id="4b3e1-126">4</span></span>|<span data-ttu-id="4b3e1-127">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="4b3e1-128">（DEP、Apple 配置器、移动配置）</span><span class="sxs-lookup"><span data-stu-id="4b3e1-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="4b3e1-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="4b3e1-129">windowsAzureADJoin</span></span>|<span data-ttu-id="4b3e1-130">5 </span><span class="sxs-lookup"><span data-stu-id="4b3e1-130">5</span></span>|<span data-ttu-id="4b3e1-131">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="4b3e1-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="4b3e1-132">windowsBulkUserless</span></span>|<span data-ttu-id="4b3e1-133">6 </span><span class="sxs-lookup"><span data-stu-id="4b3e1-133">6</span></span>|<span data-ttu-id="4b3e1-134">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="4b3e1-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="4b3e1-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="4b3e1-136">7 </span><span class="sxs-lookup"><span data-stu-id="4b3e1-136">7</span></span>|<span data-ttu-id="4b3e1-137">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="4b3e1-138">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="4b3e1-138">(Add work account)</span></span>|
|<span data-ttu-id="4b3e1-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="4b3e1-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="4b3e1-140">8 </span><span class="sxs-lookup"><span data-stu-id="4b3e1-140">8</span></span>|<span data-ttu-id="4b3e1-141">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="4b3e1-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="4b3e1-142">windowsCoManagement</span></span>|<span data-ttu-id="4b3e1-143">9 </span><span class="sxs-lookup"><span data-stu-id="4b3e1-143">9</span></span>|<span data-ttu-id="4b3e1-144">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="4b3e1-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|
|<span data-ttu-id="4b3e1-145">appleUserEnrollment</span><span class="sxs-lookup"><span data-stu-id="4b3e1-145">appleUserEnrollment</span></span>|<span data-ttu-id="4b3e1-146">11x17</span><span class="sxs-lookup"><span data-stu-id="4b3e1-146">11</span></span>|<span data-ttu-id="4b3e1-147">由 Apple 用户注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="4b3e1-147">Device managed by Apple user enrollment</span></span>|
|<span data-ttu-id="4b3e1-148">appleUserEnrollmentWithServiceAccount</span><span class="sxs-lookup"><span data-stu-id="4b3e1-148">appleUserEnrollmentWithServiceAccount</span></span>|<span data-ttu-id="4b3e1-149">12 </span><span class="sxs-lookup"><span data-stu-id="4b3e1-149">12</span></span>|<span data-ttu-id="4b3e1-150">由 Apple 用户使用服务帐户进行注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="4b3e1-150">Device managed by Apple user enrollment with service account</span></span>|
|<span data-ttu-id="4b3e1-151">azureAdJoinUsingAzureVmExtension</span><span class="sxs-lookup"><span data-stu-id="4b3e1-151">azureAdJoinUsingAzureVmExtension</span></span>|<span data-ttu-id="4b3e1-152">14 </span><span class="sxs-lookup"><span data-stu-id="4b3e1-152">14</span></span>|<span data-ttu-id="4b3e1-153">预配 Azure VM 时的 azure AD 加入注册</span><span class="sxs-lookup"><span data-stu-id="4b3e1-153">Azure AD Join enrollment when an Azure VM is provisioned</span></span>|



