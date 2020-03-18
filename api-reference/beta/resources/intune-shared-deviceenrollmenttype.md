---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c87f87b6f13d81589788c1c7e0b2834866a94690
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42771122"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="85049-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="85049-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="85049-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85049-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85049-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85049-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85049-106">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="85049-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="85049-107">成员</span><span class="sxs-lookup"><span data-stu-id="85049-107">Members</span></span>
|<span data-ttu-id="85049-108">成员</span><span class="sxs-lookup"><span data-stu-id="85049-108">Member</span></span>|<span data-ttu-id="85049-109">值</span><span class="sxs-lookup"><span data-stu-id="85049-109">Value</span></span>|<span data-ttu-id="85049-110">说明</span><span class="sxs-lookup"><span data-stu-id="85049-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85049-111">unknown</span><span class="sxs-lookup"><span data-stu-id="85049-111">unknown</span></span>|<span data-ttu-id="85049-112">0</span><span class="sxs-lookup"><span data-stu-id="85049-112">0</span></span>|<span data-ttu-id="85049-113">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="85049-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="85049-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="85049-114">userEnrollment</span></span>|<span data-ttu-id="85049-115">1</span><span class="sxs-lookup"><span data-stu-id="85049-115">1</span></span>|<span data-ttu-id="85049-116">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="85049-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="85049-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="85049-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="85049-118">双面</span><span class="sxs-lookup"><span data-stu-id="85049-118">2</span></span>|<span data-ttu-id="85049-119">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="85049-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="85049-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="85049-120">appleBulkWithUser</span></span>|<span data-ttu-id="85049-121">第三章</span><span class="sxs-lookup"><span data-stu-id="85049-121">3</span></span>|<span data-ttu-id="85049-122">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="85049-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="85049-123">（DEP、Apple 配置器）</span><span class="sxs-lookup"><span data-stu-id="85049-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="85049-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="85049-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="85049-125">4 </span><span class="sxs-lookup"><span data-stu-id="85049-125">4</span></span>|<span data-ttu-id="85049-126">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="85049-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="85049-127">（DEP、Apple 配置器、移动配置）</span><span class="sxs-lookup"><span data-stu-id="85049-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="85049-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="85049-128">windowsAzureADJoin</span></span>|<span data-ttu-id="85049-129">5 </span><span class="sxs-lookup"><span data-stu-id="85049-129">5</span></span>|<span data-ttu-id="85049-130">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="85049-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="85049-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="85049-131">windowsBulkUserless</span></span>|<span data-ttu-id="85049-132">6 </span><span class="sxs-lookup"><span data-stu-id="85049-132">6</span></span>|<span data-ttu-id="85049-133">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="85049-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="85049-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="85049-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="85049-135">7 </span><span class="sxs-lookup"><span data-stu-id="85049-135">7</span></span>|<span data-ttu-id="85049-136">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="85049-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="85049-137">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="85049-137">(Add work account)</span></span>|
|<span data-ttu-id="85049-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="85049-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="85049-139">8 </span><span class="sxs-lookup"><span data-stu-id="85049-139">8</span></span>|<span data-ttu-id="85049-140">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="85049-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="85049-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="85049-141">windowsCoManagement</span></span>|<span data-ttu-id="85049-142">9 </span><span class="sxs-lookup"><span data-stu-id="85049-142">9</span></span>|<span data-ttu-id="85049-143">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="85049-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|
|<span data-ttu-id="85049-144">appleUserEnrollment</span><span class="sxs-lookup"><span data-stu-id="85049-144">appleUserEnrollment</span></span>|<span data-ttu-id="85049-145">11x17</span><span class="sxs-lookup"><span data-stu-id="85049-145">11</span></span>|<span data-ttu-id="85049-146">由 Apple 用户注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="85049-146">Device managed by Apple user enrollment</span></span>|
|<span data-ttu-id="85049-147">appleUserEnrollmentWithServiceAccount</span><span class="sxs-lookup"><span data-stu-id="85049-147">appleUserEnrollmentWithServiceAccount</span></span>|<span data-ttu-id="85049-148">12 </span><span class="sxs-lookup"><span data-stu-id="85049-148">12</span></span>|<span data-ttu-id="85049-149">由 Apple 用户使用服务帐户进行注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="85049-149">Device managed by Apple user enrollment with service account</span></span>|



