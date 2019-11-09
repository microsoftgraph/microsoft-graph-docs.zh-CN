---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 89fbc5f549b86838eace46e4d5a0c182d6b3a44d
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086072"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="b9e15-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="b9e15-103">Get deviceManagement</span></span>

> <span data-ttu-id="b9e15-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b9e15-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b9e15-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b9e15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9e15-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9e15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9e15-107">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9e15-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9e15-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9e15-108">Prerequisites</span></span>

<span data-ttu-id="b9e15-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9e15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9e15-111">权限&nbsp;类型&nbsp;（按&nbsp;工作流）</span><span class="sxs-lookup"><span data-stu-id="b9e15-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="b9e15-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9e15-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="b9e15-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e15-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="b9e15-114">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="b9e15-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="b9e15-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-116">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="b9e15-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="b9e15-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b9e15-118">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="b9e15-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="b9e15-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="b9e15-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b9e15-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-122">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="b9e15-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="b9e15-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b9e15-124">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="b9e15-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b9e15-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b9e15-126">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="b9e15-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="b9e15-127">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-128">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="b9e15-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="b9e15-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-130">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="b9e15-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="b9e15-131">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-132">&nbsp;&nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="b9e15-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="b9e15-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-134">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="b9e15-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="b9e15-135">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-136">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="b9e15-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b9e15-137">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-138">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="b9e15-138">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b9e15-139">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-140">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="b9e15-140">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="b9e15-141">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-141">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="b9e15-142">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="b9e15-142">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="b9e15-143">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-143">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-144">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="b9e15-144">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="b9e15-145">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-146">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="b9e15-146">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="b9e15-147">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-147">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-148">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="b9e15-148">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="b9e15-149">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-149">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-150">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="b9e15-150">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b9e15-151">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-151">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b9e15-152">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="b9e15-152">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="b9e15-153">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-153">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b9e15-154">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e15-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9e15-155">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e15-155">Not supported.</span></span>|
| <span data-ttu-id="b9e15-156">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e15-156">Application</span></span> | |
| <span data-ttu-id="b9e15-157">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="b9e15-157">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="b9e15-158">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-158">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-159">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="b9e15-159">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="b9e15-160">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-160">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b9e15-161">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="b9e15-161">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="b9e15-162">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-162">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-163">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="b9e15-163">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b9e15-164">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-164">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-165">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="b9e15-165">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="b9e15-166">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-166">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b9e15-167">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="b9e15-167">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b9e15-168">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-168">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b9e15-169">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="b9e15-169">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="b9e15-170">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-170">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-171">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="b9e15-171">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="b9e15-172">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-172">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-173">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="b9e15-173">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="b9e15-174">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-174">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-175">&nbsp;&nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="b9e15-175">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="b9e15-176">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-176">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-177">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="b9e15-177">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="b9e15-178">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-178">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-179">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="b9e15-179">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b9e15-180">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-180">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-181">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="b9e15-181">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b9e15-182">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-182">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-183">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="b9e15-183">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="b9e15-184">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-184">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="b9e15-185">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="b9e15-185">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="b9e15-186">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-186">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b9e15-187">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="b9e15-187">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="b9e15-188">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-188">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-189">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="b9e15-189">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="b9e15-190">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-190">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-191">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="b9e15-191">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="b9e15-192">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-192">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b9e15-193">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="b9e15-193">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b9e15-194">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-194">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b9e15-195">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="b9e15-195">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="b9e15-196">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e15-196">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9e15-197">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e15-197">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9e15-198">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b9e15-198">Optional query parameters</span></span>

<span data-ttu-id="b9e15-199">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b9e15-199">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9e15-200">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e15-200">Request headers</span></span>
|<span data-ttu-id="b9e15-201">标头</span><span class="sxs-lookup"><span data-stu-id="b9e15-201">Header</span></span>|<span data-ttu-id="b9e15-202">值</span><span class="sxs-lookup"><span data-stu-id="b9e15-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9e15-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e15-203">Authorization</span></span>|<span data-ttu-id="b9e15-204">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e15-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9e15-205">接受</span><span class="sxs-lookup"><span data-stu-id="b9e15-205">Accept</span></span>|<span data-ttu-id="b9e15-206">application/json</span><span class="sxs-lookup"><span data-stu-id="b9e15-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e15-207">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e15-207">Request body</span></span>

<span data-ttu-id="b9e15-208">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9e15-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e15-209">响应</span><span class="sxs-lookup"><span data-stu-id="b9e15-209">Response</span></span>

<span data-ttu-id="b9e15-210">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9e15-210">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e15-211">示例</span><span class="sxs-lookup"><span data-stu-id="b9e15-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9e15-212">请求</span><span class="sxs-lookup"><span data-stu-id="b9e15-212">Request</span></span>

<span data-ttu-id="b9e15-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9e15-213">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="b9e15-214">响应</span><span class="sxs-lookup"><span data-stu-id="b9e15-214">Response</span></span>

<span data-ttu-id="b9e15-215">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="b9e15-215">Here are example of the response.</span></span> 

<span data-ttu-id="b9e15-216">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9e15-216">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="b9e15-217">将返回适用于工作流的属性。</span><span class="sxs-lookup"><span data-stu-id="b9e15-217">Properties appropriate for the workflow are returned.</span></span>

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












