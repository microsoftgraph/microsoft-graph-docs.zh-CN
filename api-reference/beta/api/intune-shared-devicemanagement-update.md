---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6bf6b5031c53da45af63517e52f03d344f71a4c3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49210128"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="e21dd-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e21dd-103">Update deviceManagement</span></span>

<span data-ttu-id="e21dd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e21dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e21dd-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e21dd-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e21dd-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e21dd-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e21dd-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e21dd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e21dd-108">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e21dd-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e21dd-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="e21dd-109">Prerequisites</span></span>

<span data-ttu-id="e21dd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e21dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e21dd-112">请注意，该权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="e21dd-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="e21dd-113">&nbsp; &nbsp; 工作流)  (的权限类型 &nbsp;</span><span class="sxs-lookup"><span data-stu-id="e21dd-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="e21dd-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e21dd-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="e21dd-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e21dd-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="e21dd-116">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="e21dd-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="e21dd-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="e21dd-118">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="e21dd-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="e21dd-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-120">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="e21dd-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="e21dd-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-122">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="e21dd-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e21dd-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-124">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="e21dd-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="e21dd-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="e21dd-126">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="e21dd-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e21dd-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-128">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="e21dd-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="e21dd-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-130">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="e21dd-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="e21dd-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-132">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="e21dd-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="e21dd-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-134">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="e21dd-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="e21dd-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-136">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="e21dd-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="e21dd-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-138">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="e21dd-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e21dd-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-140">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="e21dd-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e21dd-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-142">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="e21dd-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="e21dd-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-144">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="e21dd-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="e21dd-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e21dd-146">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="e21dd-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="e21dd-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-148">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="e21dd-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="e21dd-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-150">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="e21dd-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="e21dd-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-152">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="e21dd-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="e21dd-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-154">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="e21dd-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="e21dd-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-156">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e21dd-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e21dd-157">不支持。</span><span class="sxs-lookup"><span data-stu-id="e21dd-157">Not supported.</span></span>|
| <span data-ttu-id="e21dd-158">应用程序</span><span class="sxs-lookup"><span data-stu-id="e21dd-158">Application</span></span> ||
| <span data-ttu-id="e21dd-159">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="e21dd-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="e21dd-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="e21dd-161">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="e21dd-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="e21dd-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-163">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="e21dd-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="e21dd-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-165">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="e21dd-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e21dd-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-167">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="e21dd-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="e21dd-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="e21dd-169">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="e21dd-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="e21dd-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-171">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="e21dd-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="e21dd-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-173">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="e21dd-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="e21dd-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-175">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="e21dd-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="e21dd-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-177">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="e21dd-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="e21dd-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-179">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="e21dd-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="e21dd-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-181">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="e21dd-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="e21dd-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-183">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="e21dd-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="e21dd-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-185">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="e21dd-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="e21dd-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-187">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="e21dd-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="e21dd-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="e21dd-189">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="e21dd-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="e21dd-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-191">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="e21dd-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="e21dd-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-193">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="e21dd-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="e21dd-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-195">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="e21dd-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="e21dd-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="e21dd-197">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="e21dd-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="e21dd-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e21dd-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e21dd-199">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e21dd-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="e21dd-200">请求标头</span><span class="sxs-lookup"><span data-stu-id="e21dd-200">Request headers</span></span>

|<span data-ttu-id="e21dd-201">标头</span><span class="sxs-lookup"><span data-stu-id="e21dd-201">Header</span></span>|<span data-ttu-id="e21dd-202">值</span><span class="sxs-lookup"><span data-stu-id="e21dd-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e21dd-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="e21dd-203">Authorization</span></span>|<span data-ttu-id="e21dd-204">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e21dd-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e21dd-205">接受</span><span class="sxs-lookup"><span data-stu-id="e21dd-205">Accept</span></span>|<span data-ttu-id="e21dd-206">application/json</span><span class="sxs-lookup"><span data-stu-id="e21dd-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e21dd-207">请求正文</span><span class="sxs-lookup"><span data-stu-id="e21dd-207">Request body</span></span>

<span data-ttu-id="e21dd-208">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e21dd-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="e21dd-209">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e21dd-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="e21dd-210">属性</span><span class="sxs-lookup"><span data-stu-id="e21dd-210">Property</span></span>|<span data-ttu-id="e21dd-211">类型</span><span class="sxs-lookup"><span data-stu-id="e21dd-211">Type</span></span>|<span data-ttu-id="e21dd-212">说明</span><span class="sxs-lookup"><span data-stu-id="e21dd-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e21dd-213">id</span><span class="sxs-lookup"><span data-stu-id="e21dd-213">id</span></span>|<span data-ttu-id="e21dd-214">String</span><span class="sxs-lookup"><span data-stu-id="e21dd-214">String</span></span>|<span data-ttu-id="e21dd-215">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e21dd-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="e21dd-216">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="e21dd-216">**Device configuration**</span></span>|
|<span data-ttu-id="e21dd-217">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="e21dd-217">intuneAccountId</span></span>|<span data-ttu-id="e21dd-218">GUID</span><span class="sxs-lookup"><span data-stu-id="e21dd-218">GUID</span></span>|<span data-ttu-id="e21dd-219">给定租户的 Intune 帐户 ID</span><span class="sxs-lookup"><span data-stu-id="e21dd-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="e21dd-220">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="e21dd-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="e21dd-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="e21dd-221">Boolean</span></span>|<span data-ttu-id="e21dd-222">用于为此帐户启用非 MDM 托管旧版 PC 管理的属性。</span><span class="sxs-lookup"><span data-stu-id="e21dd-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="e21dd-223">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e21dd-223">This property is read-only.</span></span>|
|<span data-ttu-id="e21dd-224">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="e21dd-224">maximumDepTokens</span></span>|<span data-ttu-id="e21dd-225">Int32</span><span class="sxs-lookup"><span data-stu-id="e21dd-225">Int32</span></span>|<span data-ttu-id="e21dd-226">每个租户允许的最大 DEP 令牌数。</span><span class="sxs-lookup"><span data-stu-id="e21dd-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="e21dd-227">settings</span><span class="sxs-lookup"><span data-stu-id="e21dd-227">settings</span></span>|[<span data-ttu-id="e21dd-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="e21dd-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="e21dd-229">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="e21dd-229">Account level settings.</span></span>|
|<span data-ttu-id="e21dd-230">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="e21dd-230">**Device management**</span></span>|
|<span data-ttu-id="e21dd-231">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="e21dd-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="e21dd-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e21dd-232">DateTimeOffset</span></span>|<span data-ttu-id="e21dd-233">租户数据在 scaleunits 之间移动的日期 & 时间。</span><span class="sxs-lookup"><span data-stu-id="e21dd-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="e21dd-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="e21dd-234">adminConsent</span></span>|[<span data-ttu-id="e21dd-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="e21dd-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="e21dd-236">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="e21dd-236">Admin consent information.</span></span>|
|<span data-ttu-id="e21dd-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="e21dd-237">deviceProtectionOverview</span></span>|[<span data-ttu-id="e21dd-238">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="e21dd-238">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="e21dd-239">设备保护概述。</span><span class="sxs-lookup"><span data-stu-id="e21dd-239">Device protection overview.</span></span>|
|<span data-ttu-id="e21dd-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="e21dd-240">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="e21dd-241">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="e21dd-241">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="e21dd-242">设备清理规则</span><span class="sxs-lookup"><span data-stu-id="e21dd-242">Device cleanup rule</span></span>|
|<span data-ttu-id="e21dd-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="e21dd-243">subscriptionState</span></span>|[<span data-ttu-id="e21dd-244">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="e21dd-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="e21dd-245">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="e21dd-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="e21dd-246">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="e21dd-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="e21dd-247">订阅</span><span class="sxs-lookup"><span data-stu-id="e21dd-247">subscriptions</span></span>|[<span data-ttu-id="e21dd-248">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="e21dd-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="e21dd-249">租户的订阅。</span><span class="sxs-lookup"><span data-stu-id="e21dd-249">Tenant's Subscription.</span></span> <span data-ttu-id="e21dd-250">可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="e21dd-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="e21dd-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="e21dd-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="e21dd-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="e21dd-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="e21dd-253">Windows 设备的恶意软件概述。</span><span class="sxs-lookup"><span data-stu-id="e21dd-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="e21dd-254">**载入**</span><span class="sxs-lookup"><span data-stu-id="e21dd-254">**Onboarding**</span></span>|
|<span data-ttu-id="e21dd-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="e21dd-255">intuneBrand</span></span>|[<span data-ttu-id="e21dd-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="e21dd-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="e21dd-257">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="e21dd-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="e21dd-258">请求正文属性支持因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="e21dd-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="e21dd-259">响应</span><span class="sxs-lookup"><span data-stu-id="e21dd-259">Response</span></span>
<span data-ttu-id="e21dd-260">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e21dd-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e21dd-261">示例</span><span class="sxs-lookup"><span data-stu-id="e21dd-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="e21dd-262">请求</span><span class="sxs-lookup"><span data-stu-id="e21dd-262">Request</span></span>

<span data-ttu-id="e21dd-263">下面的示例展示了设备管理工作流后的请求：</span><span class="sxs-lookup"><span data-stu-id="e21dd-263">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="e21dd-264">响应</span><span class="sxs-lookup"><span data-stu-id="e21dd-264">Response</span></span>

<span data-ttu-id="e21dd-265">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e21dd-265">Here is an example of the response.</span></span> 

<span data-ttu-id="e21dd-266">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e21dd-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e21dd-267">返回的属性根据工作流和上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="e21dd-267">Returned properties vary according to workflow and context.</span></span>

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










