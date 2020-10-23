---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 076c7067650d5706132e6c857a27cf50465d1e38
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684399"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="7bad9-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7bad9-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="7bad9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bad9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bad9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7bad9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bad9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7bad9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bad9-107">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="7bad9-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="7bad9-108">成员</span><span class="sxs-lookup"><span data-stu-id="7bad9-108">Members</span></span>
|<span data-ttu-id="7bad9-109">成员</span><span class="sxs-lookup"><span data-stu-id="7bad9-109">Member</span></span>|<span data-ttu-id="7bad9-110">值</span><span class="sxs-lookup"><span data-stu-id="7bad9-110">Value</span></span>|<span data-ttu-id="7bad9-111">说明</span><span class="sxs-lookup"><span data-stu-id="7bad9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bad9-112">unknown</span><span class="sxs-lookup"><span data-stu-id="7bad9-112">unknown</span></span>|<span data-ttu-id="7bad9-113">0</span><span class="sxs-lookup"><span data-stu-id="7bad9-113">0</span></span>|<span data-ttu-id="7bad9-114">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="7bad9-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="7bad9-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="7bad9-115">userEnrollment</span></span>|<span data-ttu-id="7bad9-116">1</span><span class="sxs-lookup"><span data-stu-id="7bad9-116">1</span></span>|<span data-ttu-id="7bad9-117">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="7bad9-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="7bad9-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="7bad9-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="7bad9-119">双面</span><span class="sxs-lookup"><span data-stu-id="7bad9-119">2</span></span>|<span data-ttu-id="7bad9-120">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="7bad9-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="7bad9-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="7bad9-121">appleBulkWithUser</span></span>|<span data-ttu-id="7bad9-122">第三章</span><span class="sxs-lookup"><span data-stu-id="7bad9-122">3</span></span>|<span data-ttu-id="7bad9-123">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="7bad9-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="7bad9-124"> (DEP、Apple 配置器) </span><span class="sxs-lookup"><span data-stu-id="7bad9-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="7bad9-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="7bad9-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="7bad9-126">4 </span><span class="sxs-lookup"><span data-stu-id="7bad9-126">4</span></span>|<span data-ttu-id="7bad9-127">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="7bad9-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="7bad9-128"> (DEP、Apple 配置器、移动配置) </span><span class="sxs-lookup"><span data-stu-id="7bad9-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="7bad9-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="7bad9-129">windowsAzureADJoin</span></span>|<span data-ttu-id="7bad9-130">5 </span><span class="sxs-lookup"><span data-stu-id="7bad9-130">5</span></span>|<span data-ttu-id="7bad9-131">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="7bad9-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="7bad9-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="7bad9-132">windowsBulkUserless</span></span>|<span data-ttu-id="7bad9-133">6 </span><span class="sxs-lookup"><span data-stu-id="7bad9-133">6</span></span>|<span data-ttu-id="7bad9-134">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="7bad9-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="7bad9-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="7bad9-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="7bad9-136">7 </span><span class="sxs-lookup"><span data-stu-id="7bad9-136">7</span></span>|<span data-ttu-id="7bad9-137">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="7bad9-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="7bad9-138"> (添加工作帐户) </span><span class="sxs-lookup"><span data-stu-id="7bad9-138">(Add work account)</span></span>|
|<span data-ttu-id="7bad9-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="7bad9-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="7bad9-140">8 </span><span class="sxs-lookup"><span data-stu-id="7bad9-140">8</span></span>|<span data-ttu-id="7bad9-141">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="7bad9-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="7bad9-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="7bad9-142">windowsCoManagement</span></span>|<span data-ttu-id="7bad9-143">9 </span><span class="sxs-lookup"><span data-stu-id="7bad9-143">9</span></span>|<span data-ttu-id="7bad9-144">由 AutoPilot 或组策略触发的 Windows 10 Co-Management。</span><span class="sxs-lookup"><span data-stu-id="7bad9-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|
|<span data-ttu-id="7bad9-145">appleUserEnrollment</span><span class="sxs-lookup"><span data-stu-id="7bad9-145">appleUserEnrollment</span></span>|<span data-ttu-id="7bad9-146">11x17</span><span class="sxs-lookup"><span data-stu-id="7bad9-146">11</span></span>|<span data-ttu-id="7bad9-147">由 Apple 用户注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="7bad9-147">Device managed by Apple user enrollment</span></span>|
|<span data-ttu-id="7bad9-148">appleUserEnrollmentWithServiceAccount</span><span class="sxs-lookup"><span data-stu-id="7bad9-148">appleUserEnrollmentWithServiceAccount</span></span>|<span data-ttu-id="7bad9-149">12 </span><span class="sxs-lookup"><span data-stu-id="7bad9-149">12</span></span>|<span data-ttu-id="7bad9-150">由 Apple 用户使用服务帐户进行注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="7bad9-150">Device managed by Apple user enrollment with service account</span></span>|
|<span data-ttu-id="7bad9-151">azureAdJoinUsingAzureVmExtension</span><span class="sxs-lookup"><span data-stu-id="7bad9-151">azureAdJoinUsingAzureVmExtension</span></span>|<span data-ttu-id="7bad9-152">14 </span><span class="sxs-lookup"><span data-stu-id="7bad9-152">14</span></span>|<span data-ttu-id="7bad9-153">预配 Azure VM 时的 azure AD 加入注册</span><span class="sxs-lookup"><span data-stu-id="7bad9-153">Azure AD Join enrollment when an Azure VM is provisioned</span></span>|
|<span data-ttu-id="7bad9-154">androidEnterpriseDedicatedDevice</span><span class="sxs-lookup"><span data-stu-id="7bad9-154">androidEnterpriseDedicatedDevice</span></span>|<span data-ttu-id="7bad9-155">15 </span><span class="sxs-lookup"><span data-stu-id="7bad9-155">15</span></span>|<span data-ttu-id="7bad9-156">Android 企业专用设备</span><span class="sxs-lookup"><span data-stu-id="7bad9-156">Android Enterprise Dedicated Device</span></span>|
|<span data-ttu-id="7bad9-157">androidEnterpriseFullyManaged</span><span class="sxs-lookup"><span data-stu-id="7bad9-157">androidEnterpriseFullyManaged</span></span>|<span data-ttu-id="7bad9-158">16 </span><span class="sxs-lookup"><span data-stu-id="7bad9-158">16</span></span>|<span data-ttu-id="7bad9-159">完全管理的 Android 企业版</span><span class="sxs-lookup"><span data-stu-id="7bad9-159">Android Enterprise Fully Managed</span></span>|
|<span data-ttu-id="7bad9-160">androidEnterpriseCorporateWorkProfile</span><span class="sxs-lookup"><span data-stu-id="7bad9-160">androidEnterpriseCorporateWorkProfile</span></span>|<span data-ttu-id="7bad9-161">17 </span><span class="sxs-lookup"><span data-stu-id="7bad9-161">17</span></span>|<span data-ttu-id="7bad9-162">Android 企业公司工作配置文件</span><span class="sxs-lookup"><span data-stu-id="7bad9-162">Android Enterprise Corporate Work Profile</span></span>|





