---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d301c62b5e740976337ab98c5b1f4ea264eb860
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814425"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="b3288-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b3288-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="b3288-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b3288-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3288-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3288-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3288-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3288-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3288-107">将移动设备添加到管理的可能方式。</span><span class="sxs-lookup"><span data-stu-id="b3288-107">Possible ways of adding a mobile device to management.</span></span>
## <a name="members"></a><span data-ttu-id="b3288-108">成员</span><span class="sxs-lookup"><span data-stu-id="b3288-108">Members</span></span>
|<span data-ttu-id="b3288-109">成员</span><span class="sxs-lookup"><span data-stu-id="b3288-109">Member</span></span>|<span data-ttu-id="b3288-110">值</span><span class="sxs-lookup"><span data-stu-id="b3288-110">Value</span></span>|<span data-ttu-id="b3288-111">Description</span><span class="sxs-lookup"><span data-stu-id="b3288-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3288-112">unknown</span><span class="sxs-lookup"><span data-stu-id="b3288-112">unknown</span></span>|<span data-ttu-id="b3288-113">0</span><span class="sxs-lookup"><span data-stu-id="b3288-113">0</span></span>|<span data-ttu-id="b3288-114">默认值，注册类型不是收集的。</span><span class="sxs-lookup"><span data-stu-id="b3288-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="b3288-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="b3288-115">userEnrollment</span></span>|<span data-ttu-id="b3288-116">1</span><span class="sxs-lookup"><span data-stu-id="b3288-116">1</span></span>|<span data-ttu-id="b3288-117">通过 BYOD 通道用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="b3288-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="b3288-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="b3288-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="b3288-119">2</span><span class="sxs-lookup"><span data-stu-id="b3288-119">2</span></span>|<span data-ttu-id="b3288-120">用户注册使用设备注册管理器帐户。</span><span class="sxs-lookup"><span data-stu-id="b3288-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="b3288-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="b3288-121">appleBulkWithUser</span></span>|<span data-ttu-id="b3288-122">3</span><span class="sxs-lookup"><span data-stu-id="b3288-122">3</span></span>|<span data-ttu-id="b3288-123">与用户质询 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="b3288-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="b3288-124">(DEP，Apple 配置器)</span><span class="sxs-lookup"><span data-stu-id="b3288-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="b3288-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="b3288-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="b3288-126">4</span><span class="sxs-lookup"><span data-stu-id="b3288-126">4</span></span>|<span data-ttu-id="b3288-127">没有用户质询 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="b3288-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="b3288-128">（DEP，Apple 配置器移动配置）</span><span class="sxs-lookup"><span data-stu-id="b3288-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="b3288-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="b3288-129">windowsAzureADJoin</span></span>|<span data-ttu-id="b3288-130">5</span><span class="sxs-lookup"><span data-stu-id="b3288-130">5</span></span>|<span data-ttu-id="b3288-131">Windows Azure AD 10 加入。</span><span class="sxs-lookup"><span data-stu-id="b3288-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="b3288-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="b3288-132">windowsBulkUserless</span></span>|<span data-ttu-id="b3288-133">6</span><span class="sxs-lookup"><span data-stu-id="b3288-133">6</span></span>|<span data-ttu-id="b3288-134">Windows 10 批量注册通过 ICD 证书。</span><span class="sxs-lookup"><span data-stu-id="b3288-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="b3288-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="b3288-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="b3288-136">7</span><span class="sxs-lookup"><span data-stu-id="b3288-136">7</span></span>|<span data-ttu-id="b3288-137">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="b3288-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="b3288-138">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="b3288-138">(Add work account)</span></span>|
|<span data-ttu-id="b3288-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="b3288-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="b3288-140">8</span><span class="sxs-lookup"><span data-stu-id="b3288-140">8</span></span>|<span data-ttu-id="b3288-141">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="b3288-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="b3288-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="b3288-142">windowsCoManagement</span></span>|<span data-ttu-id="b3288-143">9</span><span class="sxs-lookup"><span data-stu-id="b3288-143">9</span></span>|<span data-ttu-id="b3288-144">由自动执行某些操作或组策略触发 Windows 10 共同管理。</span><span class="sxs-lookup"><span data-stu-id="b3288-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|





