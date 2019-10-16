---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 54aab638728ba11ab3c0147c54263bdd1096416f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538768"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="945e5-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="945e5-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="945e5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="945e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="945e5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="945e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="945e5-106">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="945e5-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="945e5-107">成员</span><span class="sxs-lookup"><span data-stu-id="945e5-107">Members</span></span>
|<span data-ttu-id="945e5-108">成员</span><span class="sxs-lookup"><span data-stu-id="945e5-108">Member</span></span>|<span data-ttu-id="945e5-109">值</span><span class="sxs-lookup"><span data-stu-id="945e5-109">Value</span></span>|<span data-ttu-id="945e5-110">说明</span><span class="sxs-lookup"><span data-stu-id="945e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="945e5-111">unknown</span><span class="sxs-lookup"><span data-stu-id="945e5-111">unknown</span></span>|<span data-ttu-id="945e5-112">0</span><span class="sxs-lookup"><span data-stu-id="945e5-112">0</span></span>|<span data-ttu-id="945e5-113">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="945e5-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="945e5-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="945e5-114">userEnrollment</span></span>|<span data-ttu-id="945e5-115">1</span><span class="sxs-lookup"><span data-stu-id="945e5-115">1</span></span>|<span data-ttu-id="945e5-116">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="945e5-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="945e5-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="945e5-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="945e5-118">双面</span><span class="sxs-lookup"><span data-stu-id="945e5-118">2</span></span>|<span data-ttu-id="945e5-119">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="945e5-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="945e5-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="945e5-120">appleBulkWithUser</span></span>|<span data-ttu-id="945e5-121">第三章</span><span class="sxs-lookup"><span data-stu-id="945e5-121">3</span></span>|<span data-ttu-id="945e5-122">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="945e5-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="945e5-123">（DEP、Apple 配置器）</span><span class="sxs-lookup"><span data-stu-id="945e5-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="945e5-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="945e5-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="945e5-125">4 </span><span class="sxs-lookup"><span data-stu-id="945e5-125">4</span></span>|<span data-ttu-id="945e5-126">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="945e5-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="945e5-127">（DEP、Apple 配置器、移动配置）</span><span class="sxs-lookup"><span data-stu-id="945e5-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="945e5-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="945e5-128">windowsAzureADJoin</span></span>|<span data-ttu-id="945e5-129">5 </span><span class="sxs-lookup"><span data-stu-id="945e5-129">5</span></span>|<span data-ttu-id="945e5-130">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="945e5-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="945e5-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="945e5-131">windowsBulkUserless</span></span>|<span data-ttu-id="945e5-132">6 </span><span class="sxs-lookup"><span data-stu-id="945e5-132">6</span></span>|<span data-ttu-id="945e5-133">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="945e5-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="945e5-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="945e5-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="945e5-135">7 </span><span class="sxs-lookup"><span data-stu-id="945e5-135">7</span></span>|<span data-ttu-id="945e5-136">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="945e5-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="945e5-137">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="945e5-137">(Add work account)</span></span>|
|<span data-ttu-id="945e5-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="945e5-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="945e5-139">8 </span><span class="sxs-lookup"><span data-stu-id="945e5-139">8</span></span>|<span data-ttu-id="945e5-140">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="945e5-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="945e5-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="945e5-141">windowsCoManagement</span></span>|<span data-ttu-id="945e5-142">9 </span><span class="sxs-lookup"><span data-stu-id="945e5-142">9</span></span>|<span data-ttu-id="945e5-143">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="945e5-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|
|<span data-ttu-id="945e5-144">appleUserEnrollment</span><span class="sxs-lookup"><span data-stu-id="945e5-144">appleUserEnrollment</span></span>|<span data-ttu-id="945e5-145">11x17</span><span class="sxs-lookup"><span data-stu-id="945e5-145">11</span></span>|<span data-ttu-id="945e5-146">由 Apple 用户注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="945e5-146">Device managed by Apple user enrollment</span></span>|
|<span data-ttu-id="945e5-147">appleUserEnrollmentWithServiceAccount</span><span class="sxs-lookup"><span data-stu-id="945e5-147">appleUserEnrollmentWithServiceAccount</span></span>|<span data-ttu-id="945e5-148">12</span><span class="sxs-lookup"><span data-stu-id="945e5-148">12</span></span>|<span data-ttu-id="945e5-149">由 Apple 用户使用服务帐户进行注册管理的设备</span><span class="sxs-lookup"><span data-stu-id="945e5-149">Device managed by Apple user enrollment with service account</span></span>|



