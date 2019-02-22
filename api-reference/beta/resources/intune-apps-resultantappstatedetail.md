---
title: resultantAppStateDetail 枚举类型
description: 指示有关应用程序为何具有特定安装状态的其他详细信息的枚举。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d6b7e6a665229d02033cd1c0c25469a83dfc37d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167212"
---
# <a name="resultantappstatedetail-enum-type"></a><span data-ttu-id="ab751-103">resultantAppStateDetail 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ab751-103">resultantAppStateDetail enum type</span></span>

> <span data-ttu-id="ab751-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab751-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab751-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab751-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab751-106">指示有关应用程序为何具有特定安装状态的其他详细信息的枚举。</span><span class="sxs-lookup"><span data-stu-id="ab751-106">Enum indicating additional details regarding why an application has a particular install state.</span></span>

## <a name="members"></a><span data-ttu-id="ab751-107">成员</span><span class="sxs-lookup"><span data-stu-id="ab751-107">Members</span></span>
|<span data-ttu-id="ab751-108">成员</span><span class="sxs-lookup"><span data-stu-id="ab751-108">Member</span></span>|<span data-ttu-id="ab751-109">值</span><span class="sxs-lookup"><span data-stu-id="ab751-109">Value</span></span>|<span data-ttu-id="ab751-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab751-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab751-111">noAdditionalDetails</span><span class="sxs-lookup"><span data-stu-id="ab751-111">noAdditionalDetails</span></span>|<span data-ttu-id="ab751-112">0</span><span class="sxs-lookup"><span data-stu-id="ab751-112">0</span></span>|<span data-ttu-id="ab751-113">没有可用的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="ab751-113">No additional details are available.</span></span>|
|<span data-ttu-id="ab751-114">seeInstallErrorCode</span><span class="sxs-lookup"><span data-stu-id="ab751-114">seeInstallErrorCode</span></span>|<span data-ttu-id="ab751-115">2000</span><span class="sxs-lookup"><span data-stu-id="ab751-115">2000</span></span>|<span data-ttu-id="ab751-116">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="ab751-116">Application failed to install.</span></span> <span data-ttu-id="ab751-117">有关更多详细信息, 请参阅错误代码属性。</span><span class="sxs-lookup"><span data-stu-id="ab751-117">See error code property for more details.</span></span>|
|<span data-ttu-id="ab751-118">seeUninstallErrorCode</span><span class="sxs-lookup"><span data-stu-id="ab751-118">seeUninstallErrorCode</span></span>|<span data-ttu-id="ab751-119">4000</span><span class="sxs-lookup"><span data-stu-id="ab751-119">4000</span></span>|<span data-ttu-id="ab751-120">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="ab751-120">Application failed to uninstall.</span></span> <span data-ttu-id="ab751-121">有关更多详细信息, 请参阅错误代码属性。</span><span class="sxs-lookup"><span data-stu-id="ab751-121">See error code property for more details.</span></span>|
|<span data-ttu-id="ab751-122">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="ab751-122">pendingReboot</span></span>|<span data-ttu-id="ab751-123">5000</span><span class="sxs-lookup"><span data-stu-id="ab751-123">5000</span></span>|<span data-ttu-id="ab751-124">必须重新启动设备才能完成应用程序的安装。</span><span class="sxs-lookup"><span data-stu-id="ab751-124">Device must be rebooted to complete installation of the application.</span></span>|
|<span data-ttu-id="ab751-125">platformNotApplicable</span><span class="sxs-lookup"><span data-stu-id="ab751-125">platformNotApplicable</span></span>|<span data-ttu-id="ab751-126">-1006</span><span class="sxs-lookup"><span data-stu-id="ab751-126">-1006</span></span>|<span data-ttu-id="ab751-127">应用程序不适用于此平台。</span><span class="sxs-lookup"><span data-stu-id="ab751-127">Application is not applicable to this platform.</span></span> <span data-ttu-id="ab751-128">(例如, 面向 IOS 的 Android 应用)</span><span class="sxs-lookup"><span data-stu-id="ab751-128">(e.g. Android app targeted to IOS)</span></span>|
|<span data-ttu-id="ab751-129">minimumCpuSpeedNotMet</span><span class="sxs-lookup"><span data-stu-id="ab751-129">minimumCpuSpeedNotMet</span></span>|<span data-ttu-id="ab751-130">-1005</span><span class="sxs-lookup"><span data-stu-id="ab751-130">-1005</span></span>|<span data-ttu-id="ab751-131">目标设备上的 CPU 速度小于配置的最小值。</span><span class="sxs-lookup"><span data-stu-id="ab751-131">CPU speed on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="ab751-132">minimumLogicalProcessorCountNotMet</span><span class="sxs-lookup"><span data-stu-id="ab751-132">minimumLogicalProcessorCountNotMet</span></span>|<span data-ttu-id="ab751-133">-1004</span><span class="sxs-lookup"><span data-stu-id="ab751-133">-1004</span></span>|<span data-ttu-id="ab751-134">目标设备上的逻辑处理器计数小于配置的最小值。</span><span class="sxs-lookup"><span data-stu-id="ab751-134">Count of logical processors on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="ab751-135">minimumPhysicalMemoryNotMet</span><span class="sxs-lookup"><span data-stu-id="ab751-135">minimumPhysicalMemoryNotMet</span></span>|<span data-ttu-id="ab751-136">-1003</span><span class="sxs-lookup"><span data-stu-id="ab751-136">-1003</span></span>|<span data-ttu-id="ab751-137">目标设备上的 RAM 量小于配置的最小值。</span><span class="sxs-lookup"><span data-stu-id="ab751-137">Amount of RAM on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="ab751-138">minimumOsVersionNotMet</span><span class="sxs-lookup"><span data-stu-id="ab751-138">minimumOsVersionNotMet</span></span>|<span data-ttu-id="ab751-139">-1002</span><span class="sxs-lookup"><span data-stu-id="ab751-139">-1002</span></span>|<span data-ttu-id="ab751-140">目标设备上的 OS 版本小于配置的最小值。</span><span class="sxs-lookup"><span data-stu-id="ab751-140">OS version on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="ab751-141">minimumDiskSpaceNotMet</span><span class="sxs-lookup"><span data-stu-id="ab751-141">minimumDiskSpaceNotMet</span></span>|<span data-ttu-id="ab751-142">-1001</span><span class="sxs-lookup"><span data-stu-id="ab751-142">-1001</span></span>|<span data-ttu-id="ab751-143">目标设备上的可用磁盘空间小于配置的最小值。</span><span class="sxs-lookup"><span data-stu-id="ab751-143">Available disk space on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="ab751-144">processorArchitectureNotApplicable</span><span class="sxs-lookup"><span data-stu-id="ab751-144">processorArchitectureNotApplicable</span></span>|<span data-ttu-id="ab751-145">-1000</span><span class="sxs-lookup"><span data-stu-id="ab751-145">-1000</span></span>|<span data-ttu-id="ab751-146">设备体系结构 (例如, x86/amd64) 不适用于应用程序。</span><span class="sxs-lookup"><span data-stu-id="ab751-146">Device architecture (e.g. x86/amd64) is not applicable for the application.</span></span>|




