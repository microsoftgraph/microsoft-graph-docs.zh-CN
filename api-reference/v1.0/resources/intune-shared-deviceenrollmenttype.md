---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理中的可能方法。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f0e309126d48646fb67446270353566be23ec9a
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732360"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="5a55a-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5a55a-103">deviceEnrollmentType enum type</span></span>

<span data-ttu-id="5a55a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a55a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5a55a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a55a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a55a-106">将移动设备添加到管理中的可能方法。</span><span class="sxs-lookup"><span data-stu-id="5a55a-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="5a55a-107">成员</span><span class="sxs-lookup"><span data-stu-id="5a55a-107">Members</span></span>
|<span data-ttu-id="5a55a-108">成员</span><span class="sxs-lookup"><span data-stu-id="5a55a-108">Member</span></span>|<span data-ttu-id="5a55a-109">值</span><span class="sxs-lookup"><span data-stu-id="5a55a-109">Value</span></span>|<span data-ttu-id="5a55a-110">Description</span><span class="sxs-lookup"><span data-stu-id="5a55a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a55a-111">unknown</span><span class="sxs-lookup"><span data-stu-id="5a55a-111">unknown</span></span>|<span data-ttu-id="5a55a-112">0</span><span class="sxs-lookup"><span data-stu-id="5a55a-112">0</span></span>|<span data-ttu-id="5a55a-113">默认值，未收集注册类型。</span><span class="sxs-lookup"><span data-stu-id="5a55a-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="5a55a-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="5a55a-114">userEnrollment</span></span>|<span data-ttu-id="5a55a-115">1</span><span class="sxs-lookup"><span data-stu-id="5a55a-115">1</span></span>|<span data-ttu-id="5a55a-116">用户通过 BYOD 渠道推动注册。</span><span class="sxs-lookup"><span data-stu-id="5a55a-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="5a55a-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="5a55a-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="5a55a-118">2</span><span class="sxs-lookup"><span data-stu-id="5a55a-118">2</span></span>|<span data-ttu-id="5a55a-119">使用设备注册管理器帐户的用户注册。</span><span class="sxs-lookup"><span data-stu-id="5a55a-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="5a55a-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="5a55a-120">appleBulkWithUser</span></span>|<span data-ttu-id="5a55a-121">3</span><span class="sxs-lookup"><span data-stu-id="5a55a-121">3</span></span>|<span data-ttu-id="5a55a-122">具有用户质询的 Apple 批量注册。</span><span class="sxs-lookup"><span data-stu-id="5a55a-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="5a55a-123"> (DEP、Apple Configurator) </span><span class="sxs-lookup"><span data-stu-id="5a55a-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="5a55a-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="5a55a-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="5a55a-125">4 </span><span class="sxs-lookup"><span data-stu-id="5a55a-125">4</span></span>|<span data-ttu-id="5a55a-126">Apple 批量注册，无需用户质询。</span><span class="sxs-lookup"><span data-stu-id="5a55a-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="5a55a-127"> (DEP、Apple Configurator、Mobile Config) </span><span class="sxs-lookup"><span data-stu-id="5a55a-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="5a55a-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="5a55a-128">windowsAzureADJoin</span></span>|<span data-ttu-id="5a55a-129">5 </span><span class="sxs-lookup"><span data-stu-id="5a55a-129">5</span></span>|<span data-ttu-id="5a55a-130">Windows 10加入 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="5a55a-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="5a55a-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="5a55a-131">windowsBulkUserless</span></span>|<span data-ttu-id="5a55a-132">6 </span><span class="sxs-lookup"><span data-stu-id="5a55a-132">6</span></span>|<span data-ttu-id="5a55a-133">Windows 10使用证书通过 ICD 批量注册。</span><span class="sxs-lookup"><span data-stu-id="5a55a-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="5a55a-134">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="5a55a-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="5a55a-135">7 </span><span class="sxs-lookup"><span data-stu-id="5a55a-135">7</span></span>|<span data-ttu-id="5a55a-136">Windows 10自动注册。</span><span class="sxs-lookup"><span data-stu-id="5a55a-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="5a55a-137"> (添加工作帐户) </span><span class="sxs-lookup"><span data-stu-id="5a55a-137">(Add work account)</span></span>|
|<span data-ttu-id="5a55a-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="5a55a-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="5a55a-139">8 </span><span class="sxs-lookup"><span data-stu-id="5a55a-139">8</span></span>|<span data-ttu-id="5a55a-140">Windows 10 Azure AD 批量加入。</span><span class="sxs-lookup"><span data-stu-id="5a55a-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="5a55a-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="5a55a-141">windowsCoManagement</span></span>|<span data-ttu-id="5a55a-142">9 </span><span class="sxs-lookup"><span data-stu-id="5a55a-142">9</span></span>|<span data-ttu-id="5a55a-143">Windows 10 Co-Management AutoPilot 或组策略触发。</span><span class="sxs-lookup"><span data-stu-id="5a55a-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|









