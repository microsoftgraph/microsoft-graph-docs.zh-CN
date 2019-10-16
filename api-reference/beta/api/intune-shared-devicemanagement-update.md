---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18ba331637a151531e6a4dcec9e794a01c927aef
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538271"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="4550a-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4550a-103">Update deviceManagement</span></span>

> <span data-ttu-id="4550a-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4550a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4550a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4550a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4550a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4550a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4550a-107">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4550a-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4550a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4550a-108">Prerequisites</span></span>

<span data-ttu-id="4550a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4550a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4550a-111">请注意，该权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="4550a-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="4550a-112">权限&nbsp;类型&nbsp;（按&nbsp;工作流）</span><span class="sxs-lookup"><span data-stu-id="4550a-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="4550a-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4550a-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="4550a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4550a-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="4550a-115">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="4550a-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="4550a-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="4550a-117">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="4550a-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="4550a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-119">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="4550a-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="4550a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4550a-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4550a-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-123">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="4550a-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="4550a-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="4550a-125">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4550a-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4550a-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-127">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="4550a-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="4550a-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-129">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="4550a-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="4550a-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-131">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="4550a-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="4550a-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-133">&nbsp;&nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="4550a-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="4550a-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="4550a-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="4550a-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-137">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="4550a-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4550a-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-139">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="4550a-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4550a-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-141">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="4550a-141">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="4550a-142">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-142">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-143">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="4550a-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="4550a-144">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4550a-144">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4550a-145">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="4550a-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="4550a-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-147">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="4550a-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4550a-148">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-148">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-149">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="4550a-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="4550a-150">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-150">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-151">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="4550a-151">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="4550a-152">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-152">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-153">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="4550a-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="4550a-154">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-154">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-155">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4550a-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4550a-156">不支持。</span><span class="sxs-lookup"><span data-stu-id="4550a-156">Not supported.</span></span>|
| <span data-ttu-id="4550a-157">应用程序</span><span class="sxs-lookup"><span data-stu-id="4550a-157">Application</span></span> ||
| <span data-ttu-id="4550a-158">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="4550a-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="4550a-159">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-159">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="4550a-160">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="4550a-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="4550a-161">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-161">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-162">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="4550a-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="4550a-163">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-163">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-164">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4550a-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4550a-165">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-165">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-166">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="4550a-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="4550a-167">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-167">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="4550a-168">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4550a-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4550a-169">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-169">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-170">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="4550a-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="4550a-171">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-171">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-172">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="4550a-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="4550a-173">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-173">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-174">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="4550a-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="4550a-175">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-175">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-176">&nbsp;&nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="4550a-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="4550a-177">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-177">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="4550a-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="4550a-179">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-179">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-180">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="4550a-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4550a-181">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-181">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-182">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="4550a-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4550a-183">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-183">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-184">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="4550a-184">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="4550a-185">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-185">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-186">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="4550a-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="4550a-187">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4550a-187">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4550a-188">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="4550a-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="4550a-189">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-189">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-190">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="4550a-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4550a-191">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-191">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-192">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="4550a-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="4550a-193">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-193">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-194">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="4550a-194">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="4550a-195">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-195">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="4550a-196">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="4550a-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="4550a-197">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4550a-197">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4550a-198">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4550a-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="4550a-199">请求标头</span><span class="sxs-lookup"><span data-stu-id="4550a-199">Request headers</span></span>

|<span data-ttu-id="4550a-200">标头</span><span class="sxs-lookup"><span data-stu-id="4550a-200">Header</span></span>|<span data-ttu-id="4550a-201">值</span><span class="sxs-lookup"><span data-stu-id="4550a-201">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4550a-202">授权</span><span class="sxs-lookup"><span data-stu-id="4550a-202">Authorization</span></span>|<span data-ttu-id="4550a-203">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4550a-203">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4550a-204">接受</span><span class="sxs-lookup"><span data-stu-id="4550a-204">Accept</span></span>|<span data-ttu-id="4550a-205">application/json</span><span class="sxs-lookup"><span data-stu-id="4550a-205">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4550a-206">请求正文</span><span class="sxs-lookup"><span data-stu-id="4550a-206">Request body</span></span>

<span data-ttu-id="4550a-207">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4550a-207">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="4550a-208">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4550a-208">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="4550a-209">属性</span><span class="sxs-lookup"><span data-stu-id="4550a-209">Property</span></span>|<span data-ttu-id="4550a-210">类型</span><span class="sxs-lookup"><span data-stu-id="4550a-210">Type</span></span>|<span data-ttu-id="4550a-211">说明</span><span class="sxs-lookup"><span data-stu-id="4550a-211">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4550a-212">id</span><span class="sxs-lookup"><span data-stu-id="4550a-212">id</span></span>|<span data-ttu-id="4550a-213">字符串</span><span class="sxs-lookup"><span data-stu-id="4550a-213">String</span></span>|<span data-ttu-id="4550a-214">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4550a-214">Unique identifier for the device.</span></span>|
|<span data-ttu-id="4550a-215">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="4550a-215">**Device configuration**</span></span>|
|<span data-ttu-id="4550a-216">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="4550a-216">intuneAccountId</span></span>|<span data-ttu-id="4550a-217">GUID</span><span class="sxs-lookup"><span data-stu-id="4550a-217">GUID</span></span>|<span data-ttu-id="4550a-218">给定租户的 Intune 帐户 ID</span><span class="sxs-lookup"><span data-stu-id="4550a-218">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="4550a-219">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="4550a-219">legacyPcManangementEnabled</span></span>|<span data-ttu-id="4550a-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="4550a-220">Boolean</span></span>|<span data-ttu-id="4550a-221">用于为此帐户启用非 MDM 托管旧版 PC 管理的属性。</span><span class="sxs-lookup"><span data-stu-id="4550a-221">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="4550a-222">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4550a-222">This property is read-only.</span></span>|
|<span data-ttu-id="4550a-223">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="4550a-223">maximumDepTokens</span></span>|<span data-ttu-id="4550a-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4550a-224">Int32</span></span>|<span data-ttu-id="4550a-225">每个租户允许的最大 DEP 令牌数。</span><span class="sxs-lookup"><span data-stu-id="4550a-225">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="4550a-226">settings</span><span class="sxs-lookup"><span data-stu-id="4550a-226">settings</span></span>|[<span data-ttu-id="4550a-227">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="4550a-227">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="4550a-228">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="4550a-228">Account level settings.</span></span>|
|<span data-ttu-id="4550a-229">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="4550a-229">**Device management**</span></span>|
|<span data-ttu-id="4550a-230">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="4550a-230">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="4550a-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4550a-231">DateTimeOffset</span></span>|<span data-ttu-id="4550a-232">租户数据在 scaleunits 之间移动的日期 & 时间。</span><span class="sxs-lookup"><span data-stu-id="4550a-232">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="4550a-233">adminConsent</span><span class="sxs-lookup"><span data-stu-id="4550a-233">adminConsent</span></span>|[<span data-ttu-id="4550a-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="4550a-234">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="4550a-235">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="4550a-235">Admin consent information.</span></span>|
|<span data-ttu-id="4550a-236">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="4550a-236">deviceProtectionOverview</span></span>|[<span data-ttu-id="4550a-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="4550a-237">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="4550a-238">设备保护概述。</span><span class="sxs-lookup"><span data-stu-id="4550a-238">Device protection overview.</span></span>|
|<span data-ttu-id="4550a-239">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="4550a-239">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="4550a-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="4550a-240">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="4550a-241">设备清理规则</span><span class="sxs-lookup"><span data-stu-id="4550a-241">Device cleanup rule</span></span>|
|<span data-ttu-id="4550a-242">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="4550a-242">subscriptionState</span></span>|[<span data-ttu-id="4550a-243">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="4550a-243">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="4550a-244">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="4550a-244">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="4550a-245">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="4550a-245">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="4550a-246">订阅</span><span class="sxs-lookup"><span data-stu-id="4550a-246">subscriptions</span></span>|[<span data-ttu-id="4550a-247">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="4550a-247">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="4550a-248">租户的订阅。</span><span class="sxs-lookup"><span data-stu-id="4550a-248">Tenant's Subscription.</span></span> <span data-ttu-id="4550a-249">可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="4550a-249">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="4550a-250">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="4550a-250">windowsMalwareOverview</span></span>|[<span data-ttu-id="4550a-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="4550a-251">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="4550a-252">Windows 设备的恶意软件概述。</span><span class="sxs-lookup"><span data-stu-id="4550a-252">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="4550a-253">**载入**</span><span class="sxs-lookup"><span data-stu-id="4550a-253">**Onboarding**</span></span>|
|<span data-ttu-id="4550a-254">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="4550a-254">intuneBrand</span></span>|[<span data-ttu-id="4550a-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="4550a-255">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="4550a-256">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="4550a-256">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="4550a-257">请求正文属性支持因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="4550a-257">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="4550a-258">响应</span><span class="sxs-lookup"><span data-stu-id="4550a-258">Response</span></span>
<span data-ttu-id="4550a-259">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4550a-259">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4550a-260">示例</span><span class="sxs-lookup"><span data-stu-id="4550a-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="4550a-261">请求</span><span class="sxs-lookup"><span data-stu-id="4550a-261">Request</span></span>

<span data-ttu-id="4550a-262">下面的示例展示了设备管理工作流后的请求：</span><span class="sxs-lookup"><span data-stu-id="4550a-262">Here is an example of a request following the device management workflow:</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a><span data-ttu-id="4550a-263">响应</span><span class="sxs-lookup"><span data-stu-id="4550a-263">Response</span></span>

<span data-ttu-id="4550a-264">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4550a-264">Here is an example of the response.</span></span> 

<span data-ttu-id="4550a-265">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4550a-265">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4550a-266">返回的属性根据工作流和上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="4550a-266">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```









