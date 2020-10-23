---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5bb7f877662021a0aa632d2b89c7bc29d47c2d7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732049"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="c1635-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c1635-103">Get deviceManagement</span></span>

<span data-ttu-id="c1635-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1635-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1635-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c1635-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1635-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c1635-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1635-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c1635-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1635-108">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c1635-108">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1635-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="c1635-109">Prerequisites</span></span>

<span data-ttu-id="c1635-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1635-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1635-112">&nbsp; &nbsp; 工作流)  (的权限类型 &nbsp;</span><span class="sxs-lookup"><span data-stu-id="c1635-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="c1635-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c1635-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="c1635-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1635-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="c1635-115">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="c1635-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="c1635-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-117">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="c1635-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="c1635-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="c1635-119">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="c1635-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="c1635-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="c1635-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c1635-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-123">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="c1635-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="c1635-124">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="c1635-125">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c1635-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c1635-126">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c1635-127">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="c1635-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="c1635-128">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-129">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="c1635-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c1635-130">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-131">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="c1635-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="c1635-132">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-133">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="c1635-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="c1635-134">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="c1635-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="c1635-136">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-137">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="c1635-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c1635-138">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-139">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="c1635-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c1635-140">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-141">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="c1635-141">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="c1635-142">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="c1635-143">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="c1635-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="c1635-144">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-145">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="c1635-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="c1635-146">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-147">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="c1635-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c1635-148">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-149">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="c1635-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="c1635-150">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-151">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="c1635-151">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c1635-152">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c1635-153">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="c1635-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="c1635-154">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="c1635-155">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1635-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1635-156">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1635-156">Not supported.</span></span>|
| <span data-ttu-id="c1635-157">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1635-157">Application</span></span> | |
| <span data-ttu-id="c1635-158">&nbsp;&nbsp;**适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="c1635-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="c1635-159">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-160">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="c1635-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="c1635-161">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="c1635-162">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="c1635-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="c1635-163">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-164">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="c1635-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c1635-165">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-166">&nbsp;&nbsp;**设备意向**</span><span class="sxs-lookup"><span data-stu-id="c1635-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="c1635-167">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="c1635-168">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="c1635-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c1635-169">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c1635-170">&nbsp;&nbsp;**电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="c1635-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="c1635-171">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-172">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="c1635-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c1635-173">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-174">&nbsp;&nbsp;**防护**</span><span class="sxs-lookup"><span data-stu-id="c1635-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="c1635-175">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-176">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="c1635-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="c1635-177">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="c1635-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="c1635-179">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-180">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="c1635-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c1635-181">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-182">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="c1635-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c1635-183">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-184">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="c1635-184">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="c1635-185">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="c1635-186">&nbsp;&nbsp;**远程访问**</span><span class="sxs-lookup"><span data-stu-id="c1635-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="c1635-187">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="c1635-188">&nbsp;&nbsp;**远程协助**</span><span class="sxs-lookup"><span data-stu-id="c1635-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="c1635-189">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-190">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="c1635-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="c1635-191">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-192">&nbsp;&nbsp;**电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="c1635-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="c1635-193">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="c1635-194">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="c1635-194">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c1635-195">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="c1635-196">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="c1635-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="c1635-197">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1635-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1635-198">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1635-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1635-199">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1635-199">Optional query parameters</span></span>

<span data-ttu-id="c1635-200">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1635-200">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1635-201">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1635-201">Request headers</span></span>
|<span data-ttu-id="c1635-202">标头</span><span class="sxs-lookup"><span data-stu-id="c1635-202">Header</span></span>|<span data-ttu-id="c1635-203">值</span><span class="sxs-lookup"><span data-stu-id="c1635-203">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1635-204">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1635-204">Authorization</span></span>|<span data-ttu-id="c1635-205">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c1635-205">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1635-206">接受</span><span class="sxs-lookup"><span data-stu-id="c1635-206">Accept</span></span>|<span data-ttu-id="c1635-207">application/json</span><span class="sxs-lookup"><span data-stu-id="c1635-207">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1635-208">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1635-208">Request body</span></span>

<span data-ttu-id="c1635-209">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1635-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1635-210">响应</span><span class="sxs-lookup"><span data-stu-id="c1635-210">Response</span></span>

<span data-ttu-id="c1635-211">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1635-211">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1635-212">示例</span><span class="sxs-lookup"><span data-stu-id="c1635-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1635-213">请求</span><span class="sxs-lookup"><span data-stu-id="c1635-213">Request</span></span>

<span data-ttu-id="c1635-214">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1635-214">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="c1635-215">响应</span><span class="sxs-lookup"><span data-stu-id="c1635-215">Response</span></span>

<span data-ttu-id="c1635-216">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="c1635-216">Here are example of the response.</span></span>

<span data-ttu-id="c1635-217">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c1635-217">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="c1635-218">将返回适用于工作流的属性。</span><span class="sxs-lookup"><span data-stu-id="c1635-218">Properties appropriate for the workflow are returned.</span></span>

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











