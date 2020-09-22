---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b7e739a1e3fd2929ba2f133199bd5872c26dd25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044807"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="e2b83-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e2b83-103">Get deviceManagement</span></span>

<span data-ttu-id="e2b83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2b83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2b83-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2b83-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2b83-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2b83-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2b83-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2b83-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2b83-108">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e2b83-108">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2b83-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2b83-109">Prerequisites</span></span>

<span data-ttu-id="e2b83-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2b83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2b83-112">&nbsp; &nbsp; 工作流)  (的权限类型 &nbsp;</span><span class="sxs-lookup"><span data-stu-id="e2b83-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="e2b83-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e2b83-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="e2b83-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2b83-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="e2b83-115">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="e2b83-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="e2b83-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-117">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="e2b83-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="e2b83-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e2b83-119">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="e2b83-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="e2b83-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="e2b83-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e2b83-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-123">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="e2b83-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="e2b83-124">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="e2b83-125">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="e2b83-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e2b83-126">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e2b83-127">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="e2b83-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="e2b83-128">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-129">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="e2b83-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="e2b83-130">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-131">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="e2b83-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="e2b83-132">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-133">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="e2b83-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="e2b83-134">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="e2b83-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="e2b83-136">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-137">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="e2b83-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e2b83-138">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-139">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="e2b83-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e2b83-140">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-141">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="e2b83-141">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="e2b83-142">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="e2b83-143">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="e2b83-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="e2b83-144">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-145">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="e2b83-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="e2b83-146">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-147">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="e2b83-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="e2b83-148">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-149">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="e2b83-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="e2b83-150">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-151">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="e2b83-151">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e2b83-152">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e2b83-153">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="e2b83-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="e2b83-154">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e2b83-155">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2b83-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2b83-156">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2b83-156">Not supported.</span></span>|
| <span data-ttu-id="e2b83-157">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2b83-157">Application</span></span> | |
| <span data-ttu-id="e2b83-158">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="e2b83-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="e2b83-159">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-160">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="e2b83-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="e2b83-161">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="e2b83-162">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="e2b83-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="e2b83-163">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-164">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="e2b83-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e2b83-165">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-166">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="e2b83-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="e2b83-167">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="e2b83-168">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="e2b83-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e2b83-169">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e2b83-170">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="e2b83-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="e2b83-171">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-172">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="e2b83-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="e2b83-173">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-174">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="e2b83-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="e2b83-175">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-176">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="e2b83-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="e2b83-177">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="e2b83-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="e2b83-179">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-180">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="e2b83-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e2b83-181">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-182">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="e2b83-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e2b83-183">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-184">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="e2b83-184">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="e2b83-185">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="e2b83-186">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="e2b83-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="e2b83-187">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e2b83-188">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="e2b83-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="e2b83-189">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-190">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="e2b83-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="e2b83-191">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-192">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="e2b83-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="e2b83-193">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="e2b83-194">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="e2b83-194">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e2b83-195">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="e2b83-196">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="e2b83-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="e2b83-197">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2b83-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2b83-198">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2b83-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2b83-199">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e2b83-199">Optional query parameters</span></span>

<span data-ttu-id="e2b83-200">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e2b83-200">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2b83-201">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2b83-201">Request headers</span></span>
|<span data-ttu-id="e2b83-202">标头</span><span class="sxs-lookup"><span data-stu-id="e2b83-202">Header</span></span>|<span data-ttu-id="e2b83-203">值</span><span class="sxs-lookup"><span data-stu-id="e2b83-203">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2b83-204">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2b83-204">Authorization</span></span>|<span data-ttu-id="e2b83-205">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e2b83-205">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2b83-206">接受</span><span class="sxs-lookup"><span data-stu-id="e2b83-206">Accept</span></span>|<span data-ttu-id="e2b83-207">application/json</span><span class="sxs-lookup"><span data-stu-id="e2b83-207">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2b83-208">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2b83-208">Request body</span></span>

<span data-ttu-id="e2b83-209">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2b83-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2b83-210">响应</span><span class="sxs-lookup"><span data-stu-id="e2b83-210">Response</span></span>

<span data-ttu-id="e2b83-211">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2b83-211">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2b83-212">示例</span><span class="sxs-lookup"><span data-stu-id="e2b83-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2b83-213">请求</span><span class="sxs-lookup"><span data-stu-id="e2b83-213">Request</span></span>

<span data-ttu-id="e2b83-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2b83-214">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="e2b83-215">响应</span><span class="sxs-lookup"><span data-stu-id="e2b83-215">Response</span></span>

<span data-ttu-id="e2b83-216">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="e2b83-216">Here are example of the response.</span></span> 

<span data-ttu-id="e2b83-217">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e2b83-217">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="e2b83-218">将返回适用于工作流的属性。</span><span class="sxs-lookup"><span data-stu-id="e2b83-218">Properties appropriate for the workflow are returned.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```












