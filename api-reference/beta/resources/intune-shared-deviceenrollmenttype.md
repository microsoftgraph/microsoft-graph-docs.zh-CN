---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bffe0e592240cbeee22a63dac8c339a0d3b3ff3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946836"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="1b7e0-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1b7e0-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="1b7e0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b7e0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b7e0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b7e0-107">将移动设备添加到管理的可能方式。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-107">Possible ways of adding a mobile device to management.</span></span>
## <a name="members"></a><span data-ttu-id="1b7e0-108">成员</span><span class="sxs-lookup"><span data-stu-id="1b7e0-108">Members</span></span>
|<span data-ttu-id="1b7e0-109">成员</span><span class="sxs-lookup"><span data-stu-id="1b7e0-109">Member</span></span>|<span data-ttu-id="1b7e0-110">值</span><span class="sxs-lookup"><span data-stu-id="1b7e0-110">Value</span></span>|<span data-ttu-id="1b7e0-111">说明</span><span class="sxs-lookup"><span data-stu-id="1b7e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b7e0-112">unknown</span><span class="sxs-lookup"><span data-stu-id="1b7e0-112">unknown</span></span>|<span data-ttu-id="1b7e0-113">0</span><span class="sxs-lookup"><span data-stu-id="1b7e0-113">0</span></span>|<span data-ttu-id="1b7e0-114">默认值，注册类型不是收集的。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="1b7e0-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="1b7e0-115">userEnrollment</span></span>|<span data-ttu-id="1b7e0-116">1</span><span class="sxs-lookup"><span data-stu-id="1b7e0-116">1</span></span>|<span data-ttu-id="1b7e0-117">通过 BYOD 通道用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="1b7e0-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="1b7e0-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="1b7e0-119">2</span><span class="sxs-lookup"><span data-stu-id="1b7e0-119">2</span></span>|<span data-ttu-id="1b7e0-120">用户注册使用设备注册管理器帐户。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="1b7e0-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="1b7e0-121">appleBulkWithUser</span></span>|<span data-ttu-id="1b7e0-122">3</span><span class="sxs-lookup"><span data-stu-id="1b7e0-122">3</span></span>|<span data-ttu-id="1b7e0-123">与用户质询 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="1b7e0-124">(DEP，Apple 配置器)</span><span class="sxs-lookup"><span data-stu-id="1b7e0-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="1b7e0-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="1b7e0-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="1b7e0-126">4</span><span class="sxs-lookup"><span data-stu-id="1b7e0-126">4</span></span>|<span data-ttu-id="1b7e0-127">没有用户质询 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="1b7e0-128">（DEP，Apple 配置器移动配置）</span><span class="sxs-lookup"><span data-stu-id="1b7e0-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="1b7e0-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="1b7e0-129">windowsAzureADJoin</span></span>|<span data-ttu-id="1b7e0-130">5</span><span class="sxs-lookup"><span data-stu-id="1b7e0-130">5</span></span>|<span data-ttu-id="1b7e0-131">Windows Azure AD 10 加入。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="1b7e0-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="1b7e0-132">windowsBulkUserless</span></span>|<span data-ttu-id="1b7e0-133">6</span><span class="sxs-lookup"><span data-stu-id="1b7e0-133">6</span></span>|<span data-ttu-id="1b7e0-134">Windows 10 批量注册通过 ICD 证书。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="1b7e0-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="1b7e0-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="1b7e0-136">7</span><span class="sxs-lookup"><span data-stu-id="1b7e0-136">7</span></span>|<span data-ttu-id="1b7e0-137">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="1b7e0-138">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="1b7e0-138">(Add work account)</span></span>|
|<span data-ttu-id="1b7e0-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="1b7e0-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="1b7e0-140">8</span><span class="sxs-lookup"><span data-stu-id="1b7e0-140">8</span></span>|<span data-ttu-id="1b7e0-141">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="1b7e0-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="1b7e0-142">windowsCoManagement</span></span>|<span data-ttu-id="1b7e0-143">9</span><span class="sxs-lookup"><span data-stu-id="1b7e0-143">9</span></span>|<span data-ttu-id="1b7e0-144">由自动执行某些操作或组策略触发 Windows 10 共同管理。</span><span class="sxs-lookup"><span data-stu-id="1b7e0-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|





