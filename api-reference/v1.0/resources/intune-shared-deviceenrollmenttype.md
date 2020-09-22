---
title: deviceEnrollmentType 枚举类型
description: 向管理层添加移动设备的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f0e309126d48646fb67446270353566be23ec9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059101"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="26ae8-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="26ae8-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="26ae8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26ae8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26ae8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26ae8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26ae8-106">向管理层添加移动设备的可能方法。</span><span class="sxs-lookup"><span data-stu-id="26ae8-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="26ae8-107">成员</span><span class="sxs-lookup"><span data-stu-id="26ae8-107">Members</span></span>
|<span data-ttu-id="26ae8-108">成员</span><span class="sxs-lookup"><span data-stu-id="26ae8-108">Member</span></span>|<span data-ttu-id="26ae8-109">值</span><span class="sxs-lookup"><span data-stu-id="26ae8-109">Value</span></span>|<span data-ttu-id="26ae8-110">说明</span><span class="sxs-lookup"><span data-stu-id="26ae8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26ae8-111">unknown</span><span class="sxs-lookup"><span data-stu-id="26ae8-111">unknown</span></span>|<span data-ttu-id="26ae8-112">0</span><span class="sxs-lookup"><span data-stu-id="26ae8-112">0</span></span>|<span data-ttu-id="26ae8-113">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="26ae8-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="26ae8-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="26ae8-114">userEnrollment</span></span>|<span data-ttu-id="26ae8-115">1 </span><span class="sxs-lookup"><span data-stu-id="26ae8-115">1</span></span>|<span data-ttu-id="26ae8-116">通过 BYOD 通道的用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="26ae8-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="26ae8-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="26ae8-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="26ae8-118">2 </span><span class="sxs-lookup"><span data-stu-id="26ae8-118">2</span></span>|<span data-ttu-id="26ae8-119">具有设备注册管理员帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="26ae8-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="26ae8-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="26ae8-120">appleBulkWithUser</span></span>|<span data-ttu-id="26ae8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="26ae8-121">3</span></span>|<span data-ttu-id="26ae8-122">使用用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="26ae8-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="26ae8-123"> (DEP、Apple 配置器) </span><span class="sxs-lookup"><span data-stu-id="26ae8-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="26ae8-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="26ae8-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="26ae8-125">4 </span><span class="sxs-lookup"><span data-stu-id="26ae8-125">4</span></span>|<span data-ttu-id="26ae8-126">没有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="26ae8-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="26ae8-127"> (DEP、Apple 配置器、移动配置) </span><span class="sxs-lookup"><span data-stu-id="26ae8-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="26ae8-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="26ae8-128">windowsAzureADJoin</span></span>|<span data-ttu-id="26ae8-129">5 </span><span class="sxs-lookup"><span data-stu-id="26ae8-129">5</span></span>|<span data-ttu-id="26ae8-130">Windows 10 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="26ae8-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="26ae8-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="26ae8-131">windowsBulkUserless</span></span>|<span data-ttu-id="26ae8-132">6 </span><span class="sxs-lookup"><span data-stu-id="26ae8-132">6</span></span>|<span data-ttu-id="26ae8-133">通过带证书的 ICD 通过 ICD 进行的 Windows 10 批量注册。</span><span class="sxs-lookup"><span data-stu-id="26ae8-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="26ae8-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="26ae8-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="26ae8-135">7 </span><span class="sxs-lookup"><span data-stu-id="26ae8-135">7</span></span>|<span data-ttu-id="26ae8-136">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="26ae8-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="26ae8-137"> (添加工作帐户) </span><span class="sxs-lookup"><span data-stu-id="26ae8-137">(Add work account)</span></span>|
|<span data-ttu-id="26ae8-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="26ae8-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="26ae8-139">8 </span><span class="sxs-lookup"><span data-stu-id="26ae8-139">8</span></span>|<span data-ttu-id="26ae8-140">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="26ae8-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="26ae8-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="26ae8-141">windowsCoManagement</span></span>|<span data-ttu-id="26ae8-142">9 </span><span class="sxs-lookup"><span data-stu-id="26ae8-142">9</span></span>|<span data-ttu-id="26ae8-143">由 AutoPilot 或组策略触发的 Windows 10 协同管理。</span><span class="sxs-lookup"><span data-stu-id="26ae8-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|









