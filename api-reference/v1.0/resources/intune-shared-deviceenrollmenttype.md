---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d27e57538927966ea741ae1da57f0a02f9de862d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807199"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="8fdbb-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8fdbb-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="8fdbb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fdbb-105">将移动设备添加到管理的可能方式。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="8fdbb-106">成员</span><span class="sxs-lookup"><span data-stu-id="8fdbb-106">Members</span></span>
|<span data-ttu-id="8fdbb-107">成员</span><span class="sxs-lookup"><span data-stu-id="8fdbb-107">Member</span></span>|<span data-ttu-id="8fdbb-108">值</span><span class="sxs-lookup"><span data-stu-id="8fdbb-108">Value</span></span>|<span data-ttu-id="8fdbb-109">Description</span><span class="sxs-lookup"><span data-stu-id="8fdbb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fdbb-110">unknown</span><span class="sxs-lookup"><span data-stu-id="8fdbb-110">unknown</span></span>|<span data-ttu-id="8fdbb-111">0</span><span class="sxs-lookup"><span data-stu-id="8fdbb-111">0</span></span>|<span data-ttu-id="8fdbb-112">默认值，注册类型不是收集的。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="8fdbb-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="8fdbb-113">userEnrollment</span></span>|<span data-ttu-id="8fdbb-114">1</span><span class="sxs-lookup"><span data-stu-id="8fdbb-114">1</span></span>|<span data-ttu-id="8fdbb-115">通过 BYOD 通道用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="8fdbb-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="8fdbb-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="8fdbb-117">2</span><span class="sxs-lookup"><span data-stu-id="8fdbb-117">2</span></span>|<span data-ttu-id="8fdbb-118">用户注册使用设备注册管理器帐户。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="8fdbb-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="8fdbb-119">appleBulkWithUser</span></span>|<span data-ttu-id="8fdbb-120">3</span><span class="sxs-lookup"><span data-stu-id="8fdbb-120">3</span></span>|<span data-ttu-id="8fdbb-121">Apple 批量注册及用户质询 （DEP、 Apple 配置器）。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-121">Apple bulk enrollment with user challenge (DEP, Apple Configurator).</span></span>|
|<span data-ttu-id="8fdbb-122">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="8fdbb-122">appleBulkWithoutUser</span></span>|<span data-ttu-id="8fdbb-123">4</span><span class="sxs-lookup"><span data-stu-id="8fdbb-123">4</span></span>|<span data-ttu-id="8fdbb-124">Apple 批量注册没有用户质询 （DEP，Apple 配置器 Mobile 配置）。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-124">Apple bulk enrollment without user challenge (DEP, Apple Configurator, Mobile Config).</span></span>|
|<span data-ttu-id="8fdbb-125">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="8fdbb-125">windowsAzureADJoin</span></span>|<span data-ttu-id="8fdbb-126">5</span><span class="sxs-lookup"><span data-stu-id="8fdbb-126">5</span></span>|<span data-ttu-id="8fdbb-127">Windows Azure AD 10 加入。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-127">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="8fdbb-128">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="8fdbb-128">windowsBulkUserless</span></span>|<span data-ttu-id="8fdbb-129">6</span><span class="sxs-lookup"><span data-stu-id="8fdbb-129">6</span></span>|<span data-ttu-id="8fdbb-130">Windows 10 批量注册通过 ICD 证书。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-130">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="8fdbb-131">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="8fdbb-131">windowsAutoEnrollment</span></span>|<span data-ttu-id="8fdbb-132">7</span><span class="sxs-lookup"><span data-stu-id="8fdbb-132">7</span></span>|<span data-ttu-id="8fdbb-133">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-133">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="8fdbb-134">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="8fdbb-134">(Add work account)</span></span>|
|<span data-ttu-id="8fdbb-135">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="8fdbb-135">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="8fdbb-136">8</span><span class="sxs-lookup"><span data-stu-id="8fdbb-136">8</span></span>|<span data-ttu-id="8fdbb-137">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-137">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="8fdbb-138">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="8fdbb-138">windowsCoManagement</span></span>|<span data-ttu-id="8fdbb-139">9</span><span class="sxs-lookup"><span data-stu-id="8fdbb-139">9</span></span>|<span data-ttu-id="8fdbb-140">Windows 10 共同管理触发自动执行某些操作或组策略。</span><span class="sxs-lookup"><span data-stu-id="8fdbb-140">Windows 10 co-management triggered by AutoPilot or Group Policy.</span></span>|



