---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec55bac63a2f50af2511c0199917d30f03cd897c
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402683"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="630d3-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="630d3-103">Get deviceManagement</span></span>

<span data-ttu-id="630d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="630d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="630d3-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="630d3-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="630d3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="630d3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="630d3-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="630d3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="630d3-108">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="630d3-108">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="630d3-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="630d3-109">Prerequisites</span></span>

<span data-ttu-id="630d3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="630d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="630d3-112">&nbsp; &nbsp; 工作流)  (的权限类型 &nbsp;</span><span class="sxs-lookup"><span data-stu-id="630d3-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="630d3-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="630d3-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="630d3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="630d3-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="630d3-115">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="630d3-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="630d3-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-117">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="630d3-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="630d3-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="630d3-119">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="630d3-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="630d3-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="630d3-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="630d3-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-123">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="630d3-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="630d3-124">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="630d3-125">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="630d3-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="630d3-126">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="630d3-127">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="630d3-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="630d3-128">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-129">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="630d3-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="630d3-130">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-131">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="630d3-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="630d3-132">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-133">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="630d3-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="630d3-134">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="630d3-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="630d3-136">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-137">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="630d3-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="630d3-138">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-139">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="630d3-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="630d3-140">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-141">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="630d3-141">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="630d3-142">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="630d3-143">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="630d3-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="630d3-144">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-145">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="630d3-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="630d3-146">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-147">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="630d3-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="630d3-148">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-149">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="630d3-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="630d3-150">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-151">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="630d3-151">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="630d3-152">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="630d3-153">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="630d3-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="630d3-154">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="630d3-155">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="630d3-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="630d3-156">不支持。</span><span class="sxs-lookup"><span data-stu-id="630d3-156">Not supported.</span></span>|
| <span data-ttu-id="630d3-157">应用程序</span><span class="sxs-lookup"><span data-stu-id="630d3-157">Application</span></span> | |
| <span data-ttu-id="630d3-158">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="630d3-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="630d3-159">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-160">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="630d3-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="630d3-161">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="630d3-162">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="630d3-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="630d3-163">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-164">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="630d3-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="630d3-165">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-166">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="630d3-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="630d3-167">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="630d3-168">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="630d3-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="630d3-169">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="630d3-170">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="630d3-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="630d3-171">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-172">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="630d3-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="630d3-173">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-174">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="630d3-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="630d3-175">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-176">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="630d3-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="630d3-177">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="630d3-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="630d3-179">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-180">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="630d3-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="630d3-181">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-182">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="630d3-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="630d3-183">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-184">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="630d3-184">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="630d3-185">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="630d3-186">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="630d3-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="630d3-187">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="630d3-188">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="630d3-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="630d3-189">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-190">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="630d3-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="630d3-191">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-192">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="630d3-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="630d3-193">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="630d3-194">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="630d3-194">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="630d3-195">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="630d3-196">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="630d3-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="630d3-197">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="630d3-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="630d3-198">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="630d3-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="630d3-199">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="630d3-199">Optional query parameters</span></span>

<span data-ttu-id="630d3-200">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="630d3-200">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="630d3-201">请求标头</span><span class="sxs-lookup"><span data-stu-id="630d3-201">Request headers</span></span>
|<span data-ttu-id="630d3-202">标头</span><span class="sxs-lookup"><span data-stu-id="630d3-202">Header</span></span>|<span data-ttu-id="630d3-203">值</span><span class="sxs-lookup"><span data-stu-id="630d3-203">Value</span></span>|
|:---|:---|
|<span data-ttu-id="630d3-204">Authorization</span><span class="sxs-lookup"><span data-stu-id="630d3-204">Authorization</span></span>|<span data-ttu-id="630d3-205">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="630d3-205">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="630d3-206">接受</span><span class="sxs-lookup"><span data-stu-id="630d3-206">Accept</span></span>|<span data-ttu-id="630d3-207">application/json</span><span class="sxs-lookup"><span data-stu-id="630d3-207">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="630d3-208">请求正文</span><span class="sxs-lookup"><span data-stu-id="630d3-208">Request body</span></span>

<span data-ttu-id="630d3-209">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="630d3-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="630d3-210">响应</span><span class="sxs-lookup"><span data-stu-id="630d3-210">Response</span></span>

<span data-ttu-id="630d3-211">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="630d3-211">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="630d3-212">示例</span><span class="sxs-lookup"><span data-stu-id="630d3-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="630d3-213">请求</span><span class="sxs-lookup"><span data-stu-id="630d3-213">Request</span></span>

<span data-ttu-id="630d3-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="630d3-214">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="630d3-215">响应</span><span class="sxs-lookup"><span data-stu-id="630d3-215">Response</span></span>

<span data-ttu-id="630d3-216">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="630d3-216">Here are example of the response.</span></span> 

<span data-ttu-id="630d3-217">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="630d3-217">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="630d3-218">将返回适用于工作流的属性。</span><span class="sxs-lookup"><span data-stu-id="630d3-218">Properties appropriate for the workflow are returned.</span></span>

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