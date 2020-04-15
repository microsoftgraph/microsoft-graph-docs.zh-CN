---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 433abdb308b838980149e7bf35784159328c6d8d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387239"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="55156-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="55156-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="55156-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55156-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55156-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55156-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55156-106">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="55156-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="55156-107">成员</span><span class="sxs-lookup"><span data-stu-id="55156-107">Members</span></span>
|<span data-ttu-id="55156-108">成员</span><span class="sxs-lookup"><span data-stu-id="55156-108">Member</span></span>|<span data-ttu-id="55156-109">值</span><span class="sxs-lookup"><span data-stu-id="55156-109">Value</span></span>|<span data-ttu-id="55156-110">说明</span><span class="sxs-lookup"><span data-stu-id="55156-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55156-111">unknown</span><span class="sxs-lookup"><span data-stu-id="55156-111">unknown</span></span>|<span data-ttu-id="55156-112">0</span><span class="sxs-lookup"><span data-stu-id="55156-112">0</span></span>|<span data-ttu-id="55156-113">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="55156-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="55156-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="55156-114">userEnrollment</span></span>|<span data-ttu-id="55156-115">1</span><span class="sxs-lookup"><span data-stu-id="55156-115">1</span></span>|<span data-ttu-id="55156-116">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="55156-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="55156-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="55156-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="55156-118">双面</span><span class="sxs-lookup"><span data-stu-id="55156-118">2</span></span>|<span data-ttu-id="55156-119">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="55156-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="55156-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="55156-120">appleBulkWithUser</span></span>|<span data-ttu-id="55156-121">第三章</span><span class="sxs-lookup"><span data-stu-id="55156-121">3</span></span>|<span data-ttu-id="55156-122">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="55156-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="55156-123">（DEP、Apple 配置器）</span><span class="sxs-lookup"><span data-stu-id="55156-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="55156-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="55156-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="55156-125">4 </span><span class="sxs-lookup"><span data-stu-id="55156-125">4</span></span>|<span data-ttu-id="55156-126">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="55156-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="55156-127">（DEP、Apple 配置器、移动配置）</span><span class="sxs-lookup"><span data-stu-id="55156-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="55156-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="55156-128">windowsAzureADJoin</span></span>|<span data-ttu-id="55156-129">5 </span><span class="sxs-lookup"><span data-stu-id="55156-129">5</span></span>|<span data-ttu-id="55156-130">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="55156-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="55156-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="55156-131">windowsBulkUserless</span></span>|<span data-ttu-id="55156-132">6 </span><span class="sxs-lookup"><span data-stu-id="55156-132">6</span></span>|<span data-ttu-id="55156-133">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="55156-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="55156-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="55156-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="55156-135">7 </span><span class="sxs-lookup"><span data-stu-id="55156-135">7</span></span>|<span data-ttu-id="55156-136">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="55156-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="55156-137">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="55156-137">(Add work account)</span></span>|
|<span data-ttu-id="55156-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="55156-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="55156-139">8 </span><span class="sxs-lookup"><span data-stu-id="55156-139">8</span></span>|<span data-ttu-id="55156-140">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="55156-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="55156-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="55156-141">windowsCoManagement</span></span>|<span data-ttu-id="55156-142">9 </span><span class="sxs-lookup"><span data-stu-id="55156-142">9</span></span>|<span data-ttu-id="55156-143">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="55156-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|







