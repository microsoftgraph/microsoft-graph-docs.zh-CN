---
title: deviceEnrollmentType 枚举类型
description: 将移动设备添加到管理的可能方式。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72acbdf412ebb91269fcdc3f851ffbc204e0274b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987753"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="283f5-103">deviceEnrollmentType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="283f5-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="283f5-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="283f5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="283f5-105">将移动设备添加到管理的可能方式。</span><span class="sxs-lookup"><span data-stu-id="283f5-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="283f5-106">成员</span><span class="sxs-lookup"><span data-stu-id="283f5-106">Members</span></span>
|<span data-ttu-id="283f5-107">成员</span><span class="sxs-lookup"><span data-stu-id="283f5-107">Member</span></span>|<span data-ttu-id="283f5-108">值</span><span class="sxs-lookup"><span data-stu-id="283f5-108">Value</span></span>|<span data-ttu-id="283f5-109">说明</span><span class="sxs-lookup"><span data-stu-id="283f5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="283f5-110">unknown</span><span class="sxs-lookup"><span data-stu-id="283f5-110">unknown</span></span>|<span data-ttu-id="283f5-111">0</span><span class="sxs-lookup"><span data-stu-id="283f5-111">0</span></span>|<span data-ttu-id="283f5-112">默认值，注册类型不是收集的。</span><span class="sxs-lookup"><span data-stu-id="283f5-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="283f5-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="283f5-113">userEnrollment</span></span>|<span data-ttu-id="283f5-114">1</span><span class="sxs-lookup"><span data-stu-id="283f5-114">1</span></span>|<span data-ttu-id="283f5-115">通过 BYOD 通道用户驱动的注册。</span><span class="sxs-lookup"><span data-stu-id="283f5-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="283f5-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="283f5-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="283f5-117">2</span><span class="sxs-lookup"><span data-stu-id="283f5-117">2</span></span>|<span data-ttu-id="283f5-118">用户注册使用设备注册管理器帐户。</span><span class="sxs-lookup"><span data-stu-id="283f5-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="283f5-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="283f5-119">appleBulkWithUser</span></span>|<span data-ttu-id="283f5-120">3</span><span class="sxs-lookup"><span data-stu-id="283f5-120">3</span></span>|<span data-ttu-id="283f5-121">Apple 批量注册及用户质询 （DEP、 Apple 配置器）。</span><span class="sxs-lookup"><span data-stu-id="283f5-121">Apple bulk enrollment with user challenge (DEP, Apple Configurator).</span></span>|
|<span data-ttu-id="283f5-122">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="283f5-122">appleBulkWithoutUser</span></span>|<span data-ttu-id="283f5-123">4</span><span class="sxs-lookup"><span data-stu-id="283f5-123">4</span></span>|<span data-ttu-id="283f5-124">Apple 批量注册没有用户质询 （DEP，Apple 配置器 Mobile 配置）。</span><span class="sxs-lookup"><span data-stu-id="283f5-124">Apple bulk enrollment without user challenge (DEP, Apple Configurator, Mobile Config).</span></span>|
|<span data-ttu-id="283f5-125">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="283f5-125">windowsAzureADJoin</span></span>|<span data-ttu-id="283f5-126">5</span><span class="sxs-lookup"><span data-stu-id="283f5-126">5</span></span>|<span data-ttu-id="283f5-127">Windows Azure AD 10 加入。</span><span class="sxs-lookup"><span data-stu-id="283f5-127">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="283f5-128">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="283f5-128">windowsBulkUserless</span></span>|<span data-ttu-id="283f5-129">6</span><span class="sxs-lookup"><span data-stu-id="283f5-129">6</span></span>|<span data-ttu-id="283f5-130">Windows 10 批量注册通过 ICD 证书。</span><span class="sxs-lookup"><span data-stu-id="283f5-130">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="283f5-131">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="283f5-131">windowsAutoEnrollment</span></span>|<span data-ttu-id="283f5-132">7</span><span class="sxs-lookup"><span data-stu-id="283f5-132">7</span></span>|<span data-ttu-id="283f5-133">Windows 10 自动注册。</span><span class="sxs-lookup"><span data-stu-id="283f5-133">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="283f5-134">（添加工作帐户）</span><span class="sxs-lookup"><span data-stu-id="283f5-134">(Add work account)</span></span>|
|<span data-ttu-id="283f5-135">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="283f5-135">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="283f5-136">8</span><span class="sxs-lookup"><span data-stu-id="283f5-136">8</span></span>|<span data-ttu-id="283f5-137">Windows 10 批量 Azure AD 加入。</span><span class="sxs-lookup"><span data-stu-id="283f5-137">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="283f5-138">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="283f5-138">windowsCoManagement</span></span>|<span data-ttu-id="283f5-139">9</span><span class="sxs-lookup"><span data-stu-id="283f5-139">9</span></span>|<span data-ttu-id="283f5-140">Windows 10 共同管理触发自动执行某些操作或组策略。</span><span class="sxs-lookup"><span data-stu-id="283f5-140">Windows 10 co-management triggered by AutoPilot or Group Policy.</span></span>|



