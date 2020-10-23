---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02ece544ac7b4b78beb8e49bb67e33035a0d0bf9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706322"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="9ef0f-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="9ef0f-103">Update deviceManagement</span></span>

<span data-ttu-id="9ef0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ef0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ef0f-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ef0f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ef0f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ef0f-108">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-108">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ef0f-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ef0f-109">Prerequisites</span></span>

<span data-ttu-id="9ef0f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9ef0f-112">请注意，该权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-112">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="9ef0f-113">&nbsp; &nbsp; 工作流)  (的权限类型 &nbsp;</span><span class="sxs-lookup"><span data-stu-id="9ef0f-113">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="9ef0f-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ef0f-114">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="9ef0f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ef0f-115">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="9ef0f-116">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-116">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="9ef0f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="9ef0f-118">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-118">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="9ef0f-119">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-119">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-120">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-120">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="9ef0f-121">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-121">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-122">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="9ef0f-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-124">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-124">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="9ef0f-125">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-125">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="9ef0f-126">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9ef0f-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-127">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-128">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-128">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="9ef0f-129">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-129">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-130">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-130">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="9ef0f-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-131">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-132">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-132">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="9ef0f-133">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-133">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-134">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-134">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="9ef0f-135">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-135">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-136">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-136">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="9ef0f-137">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-137">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-138">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-138">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9ef0f-139">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-139">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-140">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-140">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="9ef0f-141">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-141">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-142">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-142">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="9ef0f-143">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-143">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-144">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-144">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="9ef0f-145">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-145">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="9ef0f-146">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-146">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="9ef0f-147">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-147">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-148">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-148">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="9ef0f-149">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-149">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-150">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-150">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="9ef0f-151">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-151">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-152">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-152">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="9ef0f-153">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-153">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-154">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-154">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="9ef0f-155">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-155">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-156">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ef0f-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ef0f-157">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-157">Not supported.</span></span>|
| <span data-ttu-id="9ef0f-158">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ef0f-158">Application</span></span> ||
| <span data-ttu-id="9ef0f-159">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-159">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="9ef0f-160">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-160">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="9ef0f-161">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-161">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="9ef0f-162">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-162">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-163">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-163">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="9ef0f-164">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-164">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-165">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-165">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="9ef0f-166">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-166">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-167">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-167">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="9ef0f-168">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-168">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="9ef0f-169">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-169">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="9ef0f-170">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-170">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-171">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-171">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="9ef0f-172">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-172">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-173">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-173">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="9ef0f-174">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-174">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-175">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-175">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="9ef0f-176">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-176">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-177">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-177">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="9ef0f-178">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-178">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-179">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-179">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="9ef0f-180">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-180">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-181">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-181">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9ef0f-182">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-182">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-183">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-183">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="9ef0f-184">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-184">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-185">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-185">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="9ef0f-186">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-186">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-187">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-187">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="9ef0f-188">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-188">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="9ef0f-189">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-189">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="9ef0f-190">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-190">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-191">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-191">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="9ef0f-192">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-192">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-193">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-193">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="9ef0f-194">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-194">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-195">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-195">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="9ef0f-196">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-196">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef0f-197">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-197">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="9ef0f-198">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef0f-198">DeviceManagementApps.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ef0f-199">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ef0f-199">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="9ef0f-200">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ef0f-200">Request headers</span></span>

|<span data-ttu-id="9ef0f-201">标头</span><span class="sxs-lookup"><span data-stu-id="9ef0f-201">Header</span></span>|<span data-ttu-id="9ef0f-202">值</span><span class="sxs-lookup"><span data-stu-id="9ef0f-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ef0f-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ef0f-203">Authorization</span></span>|<span data-ttu-id="9ef0f-204">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ef0f-205">接受</span><span class="sxs-lookup"><span data-stu-id="9ef0f-205">Accept</span></span>|<span data-ttu-id="9ef0f-206">application/json</span><span class="sxs-lookup"><span data-stu-id="9ef0f-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ef0f-207">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ef0f-207">Request body</span></span>

<span data-ttu-id="9ef0f-208">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-208">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="9ef0f-209">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-209">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="9ef0f-210">属性</span><span class="sxs-lookup"><span data-stu-id="9ef0f-210">Property</span></span>|<span data-ttu-id="9ef0f-211">类型</span><span class="sxs-lookup"><span data-stu-id="9ef0f-211">Type</span></span>|<span data-ttu-id="9ef0f-212">说明</span><span class="sxs-lookup"><span data-stu-id="9ef0f-212">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef0f-213">id</span><span class="sxs-lookup"><span data-stu-id="9ef0f-213">id</span></span>|<span data-ttu-id="9ef0f-214">String</span><span class="sxs-lookup"><span data-stu-id="9ef0f-214">String</span></span>|<span data-ttu-id="9ef0f-215">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-215">Unique identifier for the device.</span></span>|
|<span data-ttu-id="9ef0f-216">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-216">**Device configuration**</span></span>|
|<span data-ttu-id="9ef0f-217">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="9ef0f-217">intuneAccountId</span></span>|<span data-ttu-id="9ef0f-218">GUID</span><span class="sxs-lookup"><span data-stu-id="9ef0f-218">GUID</span></span>|<span data-ttu-id="9ef0f-219">给定租户的 Intune 帐户 ID</span><span class="sxs-lookup"><span data-stu-id="9ef0f-219">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="9ef0f-220">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="9ef0f-220">legacyPcManangementEnabled</span></span>|<span data-ttu-id="9ef0f-221">布尔</span><span class="sxs-lookup"><span data-stu-id="9ef0f-221">Boolean</span></span>|<span data-ttu-id="9ef0f-222">用于为此帐户启用非 MDM 托管旧版 PC 管理的属性。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-222">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="9ef0f-223">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-223">This property is read-only.</span></span>|
|<span data-ttu-id="9ef0f-224">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="9ef0f-224">maximumDepTokens</span></span>|<span data-ttu-id="9ef0f-225">Int32</span><span class="sxs-lookup"><span data-stu-id="9ef0f-225">Int32</span></span>|<span data-ttu-id="9ef0f-226">每个租户允许的最大 DEP 令牌数。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-226">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="9ef0f-227">settings</span><span class="sxs-lookup"><span data-stu-id="9ef0f-227">settings</span></span>|[<span data-ttu-id="9ef0f-228">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="9ef0f-228">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="9ef0f-229">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-229">Account level settings.</span></span>|
|<span data-ttu-id="9ef0f-230">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-230">**Device management**</span></span>|
|<span data-ttu-id="9ef0f-231">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="9ef0f-231">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="9ef0f-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ef0f-232">DateTimeOffset</span></span>|<span data-ttu-id="9ef0f-233">租户数据在 scaleunits 之间移动的日期 & 时间。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-233">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="9ef0f-234">adminConsent</span><span class="sxs-lookup"><span data-stu-id="9ef0f-234">adminConsent</span></span>|[<span data-ttu-id="9ef0f-235">adminConsent</span><span class="sxs-lookup"><span data-stu-id="9ef0f-235">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="9ef0f-236">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-236">Admin consent information.</span></span>|
|<span data-ttu-id="9ef0f-237">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="9ef0f-237">deviceProtectionOverview</span></span>|[<span data-ttu-id="9ef0f-238">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="9ef0f-238">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="9ef0f-239">设备保护概述。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-239">Device protection overview.</span></span>|
|<span data-ttu-id="9ef0f-240">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="9ef0f-240">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="9ef0f-241">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="9ef0f-241">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="9ef0f-242">设备清理规则</span><span class="sxs-lookup"><span data-stu-id="9ef0f-242">Device cleanup rule</span></span>|
|<span data-ttu-id="9ef0f-243">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="9ef0f-243">subscriptionState</span></span>|[<span data-ttu-id="9ef0f-244">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="9ef0f-244">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="9ef0f-245">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-245">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="9ef0f-246">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-246">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="9ef0f-247">订阅</span><span class="sxs-lookup"><span data-stu-id="9ef0f-247">subscriptions</span></span>|[<span data-ttu-id="9ef0f-248">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="9ef0f-248">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="9ef0f-249">租户的订阅。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-249">Tenant's Subscription.</span></span> <span data-ttu-id="9ef0f-250">可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-250">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="9ef0f-251">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="9ef0f-251">windowsMalwareOverview</span></span>|[<span data-ttu-id="9ef0f-252">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="9ef0f-252">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="9ef0f-253">Windows 设备的恶意软件概述。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-253">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="9ef0f-254">**载入**</span><span class="sxs-lookup"><span data-stu-id="9ef0f-254">**Onboarding**</span></span>|
|<span data-ttu-id="9ef0f-255">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="9ef0f-255">intuneBrand</span></span>|[<span data-ttu-id="9ef0f-256">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="9ef0f-256">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="9ef0f-257">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-257">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="9ef0f-258">请求正文属性支持因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-258">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="9ef0f-259">响应</span><span class="sxs-lookup"><span data-stu-id="9ef0f-259">Response</span></span>
<span data-ttu-id="9ef0f-260">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-260">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ef0f-261">示例</span><span class="sxs-lookup"><span data-stu-id="9ef0f-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ef0f-262">请求</span><span class="sxs-lookup"><span data-stu-id="9ef0f-262">Request</span></span>

<span data-ttu-id="9ef0f-263">下面的示例展示了设备管理工作流后的请求：</span><span class="sxs-lookup"><span data-stu-id="9ef0f-263">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="9ef0f-264">响应</span><span class="sxs-lookup"><span data-stu-id="9ef0f-264">Response</span></span>

<span data-ttu-id="9ef0f-265">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-265">Here is an example of the response.</span></span>

<span data-ttu-id="9ef0f-266">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-266">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9ef0f-267">返回的属性根据工作流和上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="9ef0f-267">Returned properties vary according to workflow and context.</span></span>

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











