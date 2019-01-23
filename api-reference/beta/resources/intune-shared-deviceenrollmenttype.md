---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aed1f40604a765b1a434bca35dbb356e65e8ccd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399288"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="6ca2e-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6ca2e-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="6ca2e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6ca2e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ca2e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ca2e-107">将移动设备添加到管理的可能方式。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="6ca2e-108">成员</span><span class="sxs-lookup"><span data-stu-id="6ca2e-108">Members</span></span>
|<span data-ttu-id="6ca2e-109">成员</span><span class="sxs-lookup"><span data-stu-id="6ca2e-109">Member</span></span>|<span data-ttu-id="6ca2e-110">值</span><span class="sxs-lookup"><span data-stu-id="6ca2e-110">Value</span></span>|<span data-ttu-id="6ca2e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ca2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ca2e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="6ca2e-112">unknown</span></span>|<span data-ttu-id="6ca2e-113">0</span><span class="sxs-lookup"><span data-stu-id="6ca2e-113">0</span></span>|<span data-ttu-id="6ca2e-114">默认值，注册类型不是收集的。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="6ca2e-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="6ca2e-115">userEnrollment</span></span>|<span data-ttu-id="6ca2e-116">1</span><span class="sxs-lookup"><span data-stu-id="6ca2e-116">1</span></span>|<span data-ttu-id="6ca2e-117">通过 BYOD 通道用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="6ca2e-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="6ca2e-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="6ca2e-119">2</span><span class="sxs-lookup"><span data-stu-id="6ca2e-119">2</span></span>|<span data-ttu-id="6ca2e-120">用户注册使用设备注册管理器帐户。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="6ca2e-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="6ca2e-121">appleBulkWithUser</span></span>|<span data-ttu-id="6ca2e-122">3</span><span class="sxs-lookup"><span data-stu-id="6ca2e-122">3</span></span>|<span data-ttu-id="6ca2e-123">与用户质询 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="6ca2e-124">(DEP，Apple 配置器)</span><span class="sxs-lookup"><span data-stu-id="6ca2e-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="6ca2e-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="6ca2e-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="6ca2e-126">4</span><span class="sxs-lookup"><span data-stu-id="6ca2e-126">4</span></span>|<span data-ttu-id="6ca2e-127">没有用户质询 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="6ca2e-128">（DEP，Apple 配置器移动配置）</span><span class="sxs-lookup"><span data-stu-id="6ca2e-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="6ca2e-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="6ca2e-129">windowsAzureADJoin</span></span>|<span data-ttu-id="6ca2e-130">5</span><span class="sxs-lookup"><span data-stu-id="6ca2e-130">5</span></span>|<span data-ttu-id="6ca2e-131">Windows Azure AD 10 加入。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="6ca2e-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="6ca2e-132">windowsBulkUserless</span></span>|<span data-ttu-id="6ca2e-133">6</span><span class="sxs-lookup"><span data-stu-id="6ca2e-133">6</span></span>|<span data-ttu-id="6ca2e-134">Windows 10 批量注册通过 ICD 证书。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="6ca2e-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="6ca2e-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="6ca2e-136">7</span><span class="sxs-lookup"><span data-stu-id="6ca2e-136">7</span></span>|<span data-ttu-id="6ca2e-137">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="6ca2e-138">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="6ca2e-138">(Add work account)</span></span>|
|<span data-ttu-id="6ca2e-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="6ca2e-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="6ca2e-140">8</span><span class="sxs-lookup"><span data-stu-id="6ca2e-140">8</span></span>|<span data-ttu-id="6ca2e-141">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="6ca2e-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="6ca2e-142">windowsCoManagement</span></span>|<span data-ttu-id="6ca2e-143">9</span><span class="sxs-lookup"><span data-stu-id="6ca2e-143">9</span></span>|<span data-ttu-id="6ca2e-144">由自动执行某些操作或组策略触发 Windows 10 共同管理。</span><span class="sxs-lookup"><span data-stu-id="6ca2e-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




