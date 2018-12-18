---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
author: tfitzmac
ms.openlocfilehash: db66ca30758c11230282f7f3a1f6966089d6883b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339324"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="57ba4-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="57ba4-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="57ba4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="57ba4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57ba4-105">将移动设备添加到管理的可能方式。</span><span class="sxs-lookup"><span data-stu-id="57ba4-105">Possible ways of adding a mobile device to management.</span></span>
## <a name="members"></a><span data-ttu-id="57ba4-106">成员</span><span class="sxs-lookup"><span data-stu-id="57ba4-106">Members</span></span>
|<span data-ttu-id="57ba4-107">成员</span><span class="sxs-lookup"><span data-stu-id="57ba4-107">Member</span></span>|<span data-ttu-id="57ba4-108">值</span><span class="sxs-lookup"><span data-stu-id="57ba4-108">Value</span></span>|<span data-ttu-id="57ba4-109">说明</span><span class="sxs-lookup"><span data-stu-id="57ba4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57ba4-110">unknown</span><span class="sxs-lookup"><span data-stu-id="57ba4-110">unknown</span></span>|<span data-ttu-id="57ba4-111">0</span><span class="sxs-lookup"><span data-stu-id="57ba4-111">0</span></span>|<span data-ttu-id="57ba4-112">默认值，注册类型不是收集的。</span><span class="sxs-lookup"><span data-stu-id="57ba4-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="57ba4-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="57ba4-113">userEnrollment</span></span>|<span data-ttu-id="57ba4-114">1</span><span class="sxs-lookup"><span data-stu-id="57ba4-114">1</span></span>|<span data-ttu-id="57ba4-115">通过 BYOD 通道用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="57ba4-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="57ba4-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="57ba4-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="57ba4-117">2</span><span class="sxs-lookup"><span data-stu-id="57ba4-117">2</span></span>|<span data-ttu-id="57ba4-118">用户注册使用设备注册管理器帐户。</span><span class="sxs-lookup"><span data-stu-id="57ba4-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="57ba4-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="57ba4-119">appleBulkWithUser</span></span>|<span data-ttu-id="57ba4-120">3</span><span class="sxs-lookup"><span data-stu-id="57ba4-120">3</span></span>|<span data-ttu-id="57ba4-121">与用户质询 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="57ba4-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="57ba4-122">(DEP，Apple 配置器)</span><span class="sxs-lookup"><span data-stu-id="57ba4-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="57ba4-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="57ba4-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="57ba4-124">4</span><span class="sxs-lookup"><span data-stu-id="57ba4-124">4</span></span>|<span data-ttu-id="57ba4-125">没有用户质询 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="57ba4-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="57ba4-126">（DEP，Apple 配置器移动配置）</span><span class="sxs-lookup"><span data-stu-id="57ba4-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="57ba4-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="57ba4-127">windowsAzureADJoin</span></span>|<span data-ttu-id="57ba4-128">5</span><span class="sxs-lookup"><span data-stu-id="57ba4-128">5</span></span>|<span data-ttu-id="57ba4-129">Windows Azure AD 10 加入。</span><span class="sxs-lookup"><span data-stu-id="57ba4-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="57ba4-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="57ba4-130">windowsBulkUserless</span></span>|<span data-ttu-id="57ba4-131">6</span><span class="sxs-lookup"><span data-stu-id="57ba4-131">6</span></span>|<span data-ttu-id="57ba4-132">Windows 10 批量注册通过 ICD 证书。</span><span class="sxs-lookup"><span data-stu-id="57ba4-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="57ba4-133">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="57ba4-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="57ba4-134">7</span><span class="sxs-lookup"><span data-stu-id="57ba4-134">7</span></span>|<span data-ttu-id="57ba4-135">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="57ba4-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="57ba4-136">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="57ba4-136">(Add work account)</span></span>|
|<span data-ttu-id="57ba4-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="57ba4-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="57ba4-138">8</span><span class="sxs-lookup"><span data-stu-id="57ba4-138">8</span></span>|<span data-ttu-id="57ba4-139">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="57ba4-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="57ba4-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="57ba4-140">windowsCoManagement</span></span>|<span data-ttu-id="57ba4-141">9</span><span class="sxs-lookup"><span data-stu-id="57ba4-141">9</span></span>|<span data-ttu-id="57ba4-142">由自动执行某些操作或组策略触发 Windows 10 共同管理。</span><span class="sxs-lookup"><span data-stu-id="57ba4-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



