---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62ff257e2f758776265f52a0d64cde52dbc26115
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261962"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="f76fe-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f76fe-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="f76fe-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f76fe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f76fe-105">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="f76fe-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="f76fe-106">成员</span><span class="sxs-lookup"><span data-stu-id="f76fe-106">Members</span></span>
|<span data-ttu-id="f76fe-107">成员</span><span class="sxs-lookup"><span data-stu-id="f76fe-107">Member</span></span>|<span data-ttu-id="f76fe-108">值</span><span class="sxs-lookup"><span data-stu-id="f76fe-108">Value</span></span>|<span data-ttu-id="f76fe-109">说明</span><span class="sxs-lookup"><span data-stu-id="f76fe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f76fe-110">unknown</span><span class="sxs-lookup"><span data-stu-id="f76fe-110">unknown</span></span>|<span data-ttu-id="f76fe-111">0</span><span class="sxs-lookup"><span data-stu-id="f76fe-111">0</span></span>|<span data-ttu-id="f76fe-112">默认值, 未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="f76fe-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="f76fe-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="f76fe-113">userEnrollment</span></span>|<span data-ttu-id="f76fe-114">1</span><span class="sxs-lookup"><span data-stu-id="f76fe-114">1</span></span>|<span data-ttu-id="f76fe-115">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="f76fe-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="f76fe-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="f76fe-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="f76fe-117">双面</span><span class="sxs-lookup"><span data-stu-id="f76fe-117">2</span></span>|<span data-ttu-id="f76fe-118">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="f76fe-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="f76fe-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="f76fe-119">appleBulkWithUser</span></span>|<span data-ttu-id="f76fe-120">第三章</span><span class="sxs-lookup"><span data-stu-id="f76fe-120">3</span></span>|<span data-ttu-id="f76fe-121">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="f76fe-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="f76fe-122">(DEP、Apple 配置器)</span><span class="sxs-lookup"><span data-stu-id="f76fe-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="f76fe-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="f76fe-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="f76fe-124">4</span><span class="sxs-lookup"><span data-stu-id="f76fe-124">4</span></span>|<span data-ttu-id="f76fe-125">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="f76fe-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="f76fe-126">(DEP、Apple 配置器、移动配置)</span><span class="sxs-lookup"><span data-stu-id="f76fe-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="f76fe-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="f76fe-127">windowsAzureADJoin</span></span>|<span data-ttu-id="f76fe-128">5</span><span class="sxs-lookup"><span data-stu-id="f76fe-128">5</span></span>|<span data-ttu-id="f76fe-129">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="f76fe-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="f76fe-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="f76fe-130">windowsBulkUserless</span></span>|<span data-ttu-id="f76fe-131">型</span><span class="sxs-lookup"><span data-stu-id="f76fe-131">6</span></span>|<span data-ttu-id="f76fe-132">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="f76fe-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="f76fe-133">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="f76fe-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="f76fe-134">步</span><span class="sxs-lookup"><span data-stu-id="f76fe-134">7</span></span>|<span data-ttu-id="f76fe-135">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="f76fe-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="f76fe-136">(添加工作帐户)</span><span class="sxs-lookup"><span data-stu-id="f76fe-136">(Add work account)</span></span>|
|<span data-ttu-id="f76fe-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="f76fe-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="f76fe-138">utf-8</span><span class="sxs-lookup"><span data-stu-id="f76fe-138">8</span></span>|<span data-ttu-id="f76fe-139">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="f76fe-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="f76fe-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="f76fe-140">windowsCoManagement</span></span>|<span data-ttu-id="f76fe-141">第</span><span class="sxs-lookup"><span data-stu-id="f76fe-141">9</span></span>|<span data-ttu-id="f76fe-142">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="f76fe-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



