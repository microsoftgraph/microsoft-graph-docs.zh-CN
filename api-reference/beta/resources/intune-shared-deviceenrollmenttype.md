---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f96ba12380e67ee97909b2c6ef1787ba9fcc7a3a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196327"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="9c251-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9c251-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="9c251-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c251-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c251-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c251-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c251-106">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="9c251-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="9c251-107">成员</span><span class="sxs-lookup"><span data-stu-id="9c251-107">Members</span></span>
|<span data-ttu-id="9c251-108">成员</span><span class="sxs-lookup"><span data-stu-id="9c251-108">Member</span></span>|<span data-ttu-id="9c251-109">值</span><span class="sxs-lookup"><span data-stu-id="9c251-109">Value</span></span>|<span data-ttu-id="9c251-110">说明</span><span class="sxs-lookup"><span data-stu-id="9c251-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c251-111">unknown</span><span class="sxs-lookup"><span data-stu-id="9c251-111">unknown</span></span>|<span data-ttu-id="9c251-112">0</span><span class="sxs-lookup"><span data-stu-id="9c251-112">0</span></span>|<span data-ttu-id="9c251-113">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="9c251-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="9c251-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="9c251-114">userEnrollment</span></span>|<span data-ttu-id="9c251-115">1</span><span class="sxs-lookup"><span data-stu-id="9c251-115">1</span></span>|<span data-ttu-id="9c251-116">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="9c251-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="9c251-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="9c251-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="9c251-118">双面</span><span class="sxs-lookup"><span data-stu-id="9c251-118">2</span></span>|<span data-ttu-id="9c251-119">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="9c251-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="9c251-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="9c251-120">appleBulkWithUser</span></span>|<span data-ttu-id="9c251-121">第三章</span><span class="sxs-lookup"><span data-stu-id="9c251-121">3</span></span>|<span data-ttu-id="9c251-122">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="9c251-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="9c251-123">（DEP、Apple 配置器）</span><span class="sxs-lookup"><span data-stu-id="9c251-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="9c251-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="9c251-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="9c251-125">4</span><span class="sxs-lookup"><span data-stu-id="9c251-125">4</span></span>|<span data-ttu-id="9c251-126">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="9c251-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="9c251-127">（DEP、Apple 配置器、移动配置）</span><span class="sxs-lookup"><span data-stu-id="9c251-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="9c251-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="9c251-128">windowsAzureADJoin</span></span>|<span data-ttu-id="9c251-129">5</span><span class="sxs-lookup"><span data-stu-id="9c251-129">5</span></span>|<span data-ttu-id="9c251-130">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="9c251-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="9c251-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="9c251-131">windowsBulkUserless</span></span>|<span data-ttu-id="9c251-132">型</span><span class="sxs-lookup"><span data-stu-id="9c251-132">6</span></span>|<span data-ttu-id="9c251-133">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="9c251-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="9c251-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="9c251-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="9c251-135">步</span><span class="sxs-lookup"><span data-stu-id="9c251-135">7</span></span>|<span data-ttu-id="9c251-136">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="9c251-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="9c251-137">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="9c251-137">(Add work account)</span></span>|
|<span data-ttu-id="9c251-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="9c251-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="9c251-139">utf-8</span><span class="sxs-lookup"><span data-stu-id="9c251-139">8</span></span>|<span data-ttu-id="9c251-140">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="9c251-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="9c251-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="9c251-141">windowsCoManagement</span></span>|<span data-ttu-id="9c251-142">第</span><span class="sxs-lookup"><span data-stu-id="9c251-142">9</span></span>|<span data-ttu-id="9c251-143">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="9c251-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|
|<span data-ttu-id="9c251-144">appleUserEnrollment</span><span class="sxs-lookup"><span data-stu-id="9c251-144">appleUserEnrollment</span></span>|<span data-ttu-id="9c251-145">11x17</span><span class="sxs-lookup"><span data-stu-id="9c251-145">11</span></span>|<span data-ttu-id="9c251-146">由 Apple 用户注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="9c251-146">Device managed by Apple user enrollment</span></span>|
|<span data-ttu-id="9c251-147">appleUserEnrollmentWithServiceAccount</span><span class="sxs-lookup"><span data-stu-id="9c251-147">appleUserEnrollmentWithServiceAccount</span></span>|<span data-ttu-id="9c251-148">12</span><span class="sxs-lookup"><span data-stu-id="9c251-148">12</span></span>|<span data-ttu-id="9c251-149">由 Apple 用户使用服务帐户进行注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="9c251-149">Device managed by Apple user enrollment with service account</span></span>|
|<span data-ttu-id="9c251-150">appleUserEnrollmentWithAzureAD</span><span class="sxs-lookup"><span data-stu-id="9c251-150">appleUserEnrollmentWithAzureAD</span></span>|<span data-ttu-id="9c251-151">13</span><span class="sxs-lookup"><span data-stu-id="9c251-151">13</span></span>|<span data-ttu-id="9c251-152">由使用 Azure active directory 的 Apple 用户注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="9c251-152">Device managed by Apple user enrollment with Azure active directory</span></span>|



