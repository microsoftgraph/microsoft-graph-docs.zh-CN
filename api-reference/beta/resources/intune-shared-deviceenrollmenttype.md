---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3242018f288e47104e6b668beeeb5d4eb3c53964
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055322"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="6954a-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6954a-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="6954a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6954a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6954a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6954a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6954a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6954a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6954a-107">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="6954a-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="6954a-108">成员</span><span class="sxs-lookup"><span data-stu-id="6954a-108">Members</span></span>
|<span data-ttu-id="6954a-109">成员</span><span class="sxs-lookup"><span data-stu-id="6954a-109">Member</span></span>|<span data-ttu-id="6954a-110">值</span><span class="sxs-lookup"><span data-stu-id="6954a-110">Value</span></span>|<span data-ttu-id="6954a-111">说明</span><span class="sxs-lookup"><span data-stu-id="6954a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6954a-112">unknown</span><span class="sxs-lookup"><span data-stu-id="6954a-112">unknown</span></span>|<span data-ttu-id="6954a-113">0</span><span class="sxs-lookup"><span data-stu-id="6954a-113">0</span></span>|<span data-ttu-id="6954a-114">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="6954a-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="6954a-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="6954a-115">userEnrollment</span></span>|<span data-ttu-id="6954a-116">1 </span><span class="sxs-lookup"><span data-stu-id="6954a-116">1</span></span>|<span data-ttu-id="6954a-117">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="6954a-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="6954a-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="6954a-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="6954a-119">2 </span><span class="sxs-lookup"><span data-stu-id="6954a-119">2</span></span>|<span data-ttu-id="6954a-120">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="6954a-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="6954a-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="6954a-121">appleBulkWithUser</span></span>|<span data-ttu-id="6954a-122">第三章</span><span class="sxs-lookup"><span data-stu-id="6954a-122">3</span></span>|<span data-ttu-id="6954a-123">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="6954a-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="6954a-124"> (DEP、Apple 配置器) </span><span class="sxs-lookup"><span data-stu-id="6954a-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="6954a-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="6954a-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="6954a-126">4 </span><span class="sxs-lookup"><span data-stu-id="6954a-126">4</span></span>|<span data-ttu-id="6954a-127">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="6954a-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="6954a-128"> (DEP、Apple 配置器、移动配置) </span><span class="sxs-lookup"><span data-stu-id="6954a-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="6954a-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="6954a-129">windowsAzureADJoin</span></span>|<span data-ttu-id="6954a-130">5 </span><span class="sxs-lookup"><span data-stu-id="6954a-130">5</span></span>|<span data-ttu-id="6954a-131">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="6954a-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="6954a-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="6954a-132">windowsBulkUserless</span></span>|<span data-ttu-id="6954a-133">6 </span><span class="sxs-lookup"><span data-stu-id="6954a-133">6</span></span>|<span data-ttu-id="6954a-134">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="6954a-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="6954a-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="6954a-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="6954a-136">7 </span><span class="sxs-lookup"><span data-stu-id="6954a-136">7</span></span>|<span data-ttu-id="6954a-137">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="6954a-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="6954a-138"> (添加工作帐户) </span><span class="sxs-lookup"><span data-stu-id="6954a-138">(Add work account)</span></span>|
|<span data-ttu-id="6954a-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="6954a-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="6954a-140">8 </span><span class="sxs-lookup"><span data-stu-id="6954a-140">8</span></span>|<span data-ttu-id="6954a-141">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="6954a-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="6954a-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="6954a-142">windowsCoManagement</span></span>|<span data-ttu-id="6954a-143">9 </span><span class="sxs-lookup"><span data-stu-id="6954a-143">9</span></span>|<span data-ttu-id="6954a-144">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="6954a-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|
|<span data-ttu-id="6954a-145">appleUserEnrollment</span><span class="sxs-lookup"><span data-stu-id="6954a-145">appleUserEnrollment</span></span>|<span data-ttu-id="6954a-146">11 </span><span class="sxs-lookup"><span data-stu-id="6954a-146">11</span></span>|<span data-ttu-id="6954a-147">由 Apple 用户注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="6954a-147">Device managed by Apple user enrollment</span></span>|
|<span data-ttu-id="6954a-148">appleUserEnrollmentWithServiceAccount</span><span class="sxs-lookup"><span data-stu-id="6954a-148">appleUserEnrollmentWithServiceAccount</span></span>|<span data-ttu-id="6954a-149">12 </span><span class="sxs-lookup"><span data-stu-id="6954a-149">12</span></span>|<span data-ttu-id="6954a-150">由 Apple 用户使用服务帐户进行注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="6954a-150">Device managed by Apple user enrollment with service account</span></span>|
|<span data-ttu-id="6954a-151">azureAdJoinUsingAzureVmExtension</span><span class="sxs-lookup"><span data-stu-id="6954a-151">azureAdJoinUsingAzureVmExtension</span></span>|<span data-ttu-id="6954a-152">14 </span><span class="sxs-lookup"><span data-stu-id="6954a-152">14</span></span>|<span data-ttu-id="6954a-153">预配 Azure VM 时的 azure AD 加入注册</span><span class="sxs-lookup"><span data-stu-id="6954a-153">Azure AD Join enrollment when an Azure VM is provisioned</span></span>|
|<span data-ttu-id="6954a-154">androidEnterpriseDedicatedDevice</span><span class="sxs-lookup"><span data-stu-id="6954a-154">androidEnterpriseDedicatedDevice</span></span>|<span data-ttu-id="6954a-155">15 </span><span class="sxs-lookup"><span data-stu-id="6954a-155">15</span></span>|<span data-ttu-id="6954a-156">Android 企业专用设备</span><span class="sxs-lookup"><span data-stu-id="6954a-156">Android Enterprise Dedicated Device</span></span>|
|<span data-ttu-id="6954a-157">androidEnterpriseFullyManaged</span><span class="sxs-lookup"><span data-stu-id="6954a-157">androidEnterpriseFullyManaged</span></span>|<span data-ttu-id="6954a-158">16 </span><span class="sxs-lookup"><span data-stu-id="6954a-158">16</span></span>|<span data-ttu-id="6954a-159">完全管理的 Android 企业版</span><span class="sxs-lookup"><span data-stu-id="6954a-159">Android Enterprise Fully Managed</span></span>|
|<span data-ttu-id="6954a-160">androidEnterpriseCorporateWorkProfile</span><span class="sxs-lookup"><span data-stu-id="6954a-160">androidEnterpriseCorporateWorkProfile</span></span>|<span data-ttu-id="6954a-161">17 </span><span class="sxs-lookup"><span data-stu-id="6954a-161">17</span></span>|<span data-ttu-id="6954a-162">Android 企业公司工作配置文件</span><span class="sxs-lookup"><span data-stu-id="6954a-162">Android Enterprise Corporate Work Profile</span></span>|






