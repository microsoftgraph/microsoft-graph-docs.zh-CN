---
title: resultantAppStateDetail 枚举类型
description: 枚举指示其他详细信息有关为什么应用程序具有特定安装状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34b4d885f9ed2a23669bc2e30c91de40af8d915b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410236"
---
# <a name="resultantappstatedetail-enum-type"></a><span data-ttu-id="0dde9-103">resultantAppStateDetail 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0dde9-103">resultantAppStateDetail enum type</span></span>

> <span data-ttu-id="0dde9-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0dde9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0dde9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0dde9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0dde9-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0dde9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dde9-107">枚举指示其他详细信息有关为什么应用程序具有特定安装状态。</span><span class="sxs-lookup"><span data-stu-id="0dde9-107">Enum indicating additional details regarding why an application has a particular install state.</span></span>

## <a name="members"></a><span data-ttu-id="0dde9-108">成员</span><span class="sxs-lookup"><span data-stu-id="0dde9-108">Members</span></span>
|<span data-ttu-id="0dde9-109">成员</span><span class="sxs-lookup"><span data-stu-id="0dde9-109">Member</span></span>|<span data-ttu-id="0dde9-110">值</span><span class="sxs-lookup"><span data-stu-id="0dde9-110">Value</span></span>|<span data-ttu-id="0dde9-111">说明</span><span class="sxs-lookup"><span data-stu-id="0dde9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dde9-112">noAdditionalDetails</span><span class="sxs-lookup"><span data-stu-id="0dde9-112">noAdditionalDetails</span></span>|<span data-ttu-id="0dde9-113">0</span><span class="sxs-lookup"><span data-stu-id="0dde9-113">0</span></span>|<span data-ttu-id="0dde9-114">可用不的任何其他的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0dde9-114">No additional details are available.</span></span>|
|<span data-ttu-id="0dde9-115">seeInstallErrorCode</span><span class="sxs-lookup"><span data-stu-id="0dde9-115">seeInstallErrorCode</span></span>|<span data-ttu-id="0dde9-116">2000</span><span class="sxs-lookup"><span data-stu-id="0dde9-116">2000</span></span>|<span data-ttu-id="0dde9-117">应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="0dde9-117">Application failed to install.</span></span> <span data-ttu-id="0dde9-118">请参阅错误代码的详细信息的属性。</span><span class="sxs-lookup"><span data-stu-id="0dde9-118">See error code property for more details.</span></span>|
|<span data-ttu-id="0dde9-119">seeUninstallErrorCode</span><span class="sxs-lookup"><span data-stu-id="0dde9-119">seeUninstallErrorCode</span></span>|<span data-ttu-id="0dde9-120">4000</span><span class="sxs-lookup"><span data-stu-id="0dde9-120">4000</span></span>|<span data-ttu-id="0dde9-121">应用程序卸载失败。</span><span class="sxs-lookup"><span data-stu-id="0dde9-121">Application failed to uninstall.</span></span> <span data-ttu-id="0dde9-122">请参阅错误代码的详细信息的属性。</span><span class="sxs-lookup"><span data-stu-id="0dde9-122">See error code property for more details.</span></span>|
|<span data-ttu-id="0dde9-123">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="0dde9-123">pendingReboot</span></span>|<span data-ttu-id="0dde9-124">5000</span><span class="sxs-lookup"><span data-stu-id="0dde9-124">5000</span></span>|<span data-ttu-id="0dde9-125">必须重新启动设备，以完成安装的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0dde9-125">Device must be rebooted to complete installation of the application.</span></span>|
|<span data-ttu-id="0dde9-126">platformNotApplicable</span><span class="sxs-lookup"><span data-stu-id="0dde9-126">platformNotApplicable</span></span>|<span data-ttu-id="0dde9-127">-1006</span><span class="sxs-lookup"><span data-stu-id="0dde9-127">-1006</span></span>|<span data-ttu-id="0dde9-128">应用程序不适用于此平台。</span><span class="sxs-lookup"><span data-stu-id="0dde9-128">Application is not applicable to this platform.</span></span> <span data-ttu-id="0dde9-129">（例如 Android 应用程序针对 IOS）</span><span class="sxs-lookup"><span data-stu-id="0dde9-129">(e.g. Android app targeted to IOS)</span></span>|
|<span data-ttu-id="0dde9-130">minimumCpuSpeedNotMet</span><span class="sxs-lookup"><span data-stu-id="0dde9-130">minimumCpuSpeedNotMet</span></span>|<span data-ttu-id="0dde9-131">-1005</span><span class="sxs-lookup"><span data-stu-id="0dde9-131">-1005</span></span>|<span data-ttu-id="0dde9-132">配置最小值小于目标设备上的 CPU 速度。</span><span class="sxs-lookup"><span data-stu-id="0dde9-132">CPU speed on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="0dde9-133">minimumLogicalProcessorCountNotMet</span><span class="sxs-lookup"><span data-stu-id="0dde9-133">minimumLogicalProcessorCountNotMet</span></span>|<span data-ttu-id="0dde9-134">-1004</span><span class="sxs-lookup"><span data-stu-id="0dde9-134">-1004</span></span>|<span data-ttu-id="0dde9-135">配置最小值小于目标设备上的逻辑处理器的计数。</span><span class="sxs-lookup"><span data-stu-id="0dde9-135">Count of logical processors on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="0dde9-136">minimumPhysicalMemoryNotMet</span><span class="sxs-lookup"><span data-stu-id="0dde9-136">minimumPhysicalMemoryNotMet</span></span>|<span data-ttu-id="0dde9-137">-1003</span><span class="sxs-lookup"><span data-stu-id="0dde9-137">-1003</span></span>|<span data-ttu-id="0dde9-138">目标设备上的 RAM 量小于配置的最小值。</span><span class="sxs-lookup"><span data-stu-id="0dde9-138">Amount of RAM on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="0dde9-139">minimumOsVersionNotMet</span><span class="sxs-lookup"><span data-stu-id="0dde9-139">minimumOsVersionNotMet</span></span>|<span data-ttu-id="0dde9-140">-1002</span><span class="sxs-lookup"><span data-stu-id="0dde9-140">-1002</span></span>|<span data-ttu-id="0dde9-141">配置最小值小于目标设备上的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0dde9-141">OS version on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="0dde9-142">minimumDiskSpaceNotMet</span><span class="sxs-lookup"><span data-stu-id="0dde9-142">minimumDiskSpaceNotMet</span></span>|<span data-ttu-id="0dde9-143">-1001</span><span class="sxs-lookup"><span data-stu-id="0dde9-143">-1001</span></span>|<span data-ttu-id="0dde9-144">目标设备上的可用磁盘空间小于配置的最小值。</span><span class="sxs-lookup"><span data-stu-id="0dde9-144">Available disk space on the target device is less than the configured minimum.</span></span>|
|<span data-ttu-id="0dde9-145">processorArchitectureNotApplicable</span><span class="sxs-lookup"><span data-stu-id="0dde9-145">processorArchitectureNotApplicable</span></span>|<span data-ttu-id="0dde9-146">-1000</span><span class="sxs-lookup"><span data-stu-id="0dde9-146">-1000</span></span>|<span data-ttu-id="0dde9-147">设备体系结构 (如 x86/amd64) 不适用的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0dde9-147">Device architecture (e.g. x86/amd64) is not applicable for the application.</span></span>|




