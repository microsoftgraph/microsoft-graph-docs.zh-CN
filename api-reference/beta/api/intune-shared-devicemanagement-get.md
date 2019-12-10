---
title: 获取 deviceManagement
description: 读取 deviceManagement 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96c7667e34812e34f1ddf12bc25425ffecc147a0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939996"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="4a392-103">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="4a392-103">Get deviceManagement</span></span>

> <span data-ttu-id="4a392-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4a392-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a392-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a392-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a392-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a392-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a392-107">读取 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a392-107">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a392-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a392-108">Prerequisites</span></span>

<span data-ttu-id="4a392-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a392-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a392-111">权限&nbsp;类型&nbsp;（按&nbsp;工作流）</span><span class="sxs-lookup"><span data-stu-id="4a392-111">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="4a392-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a392-112">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="4a392-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a392-113">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="4a392-114">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="4a392-114">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="4a392-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-116">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="4a392-116">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="4a392-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="4a392-118">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="4a392-118">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="4a392-119">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-119">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4a392-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4a392-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-122">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="4a392-122">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="4a392-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4a392-124">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4a392-124">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4a392-125">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4a392-126">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="4a392-126">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="4a392-127">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-127">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-128">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="4a392-128">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="4a392-129">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-129">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-130">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="4a392-130">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="4a392-131">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-131">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-132">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="4a392-132">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="4a392-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-134">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="4a392-134">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="4a392-135">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-135">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-136">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="4a392-136">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4a392-137">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-137">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-138">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="4a392-138">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4a392-139">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-139">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-140">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="4a392-140">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="4a392-141">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-141">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="4a392-142">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="4a392-142">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="4a392-143">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-143">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-144">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="4a392-144">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="4a392-145">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-145">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-146">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="4a392-146">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4a392-147">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-147">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-148">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="4a392-148">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="4a392-149">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-149">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-150">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="4a392-150">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4a392-151">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-151">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4a392-152">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="4a392-152">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="4a392-153">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-153">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="4a392-154">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a392-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a392-155">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a392-155">Not supported.</span></span>|
| <span data-ttu-id="4a392-156">Application</span><span class="sxs-lookup"><span data-stu-id="4a392-156">Application</span></span> | |
| <span data-ttu-id="4a392-157">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="4a392-157">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="4a392-158">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-158">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-159">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="4a392-159">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="4a392-160">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-160">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="4a392-161">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="4a392-161">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="4a392-162">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-162">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-163">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="4a392-163">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4a392-164">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-164">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-165">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="4a392-165">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="4a392-166">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-166">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4a392-167">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="4a392-167">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="4a392-168">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-168">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4a392-169">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="4a392-169">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="4a392-170">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-170">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-171">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="4a392-171">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="4a392-172">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-172">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-173">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="4a392-173">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="4a392-174">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-174">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-175">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="4a392-175">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="4a392-176">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-176">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-177">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="4a392-177">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="4a392-178">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-178">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-179">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="4a392-179">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4a392-180">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-180">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-181">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="4a392-181">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="4a392-182">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-182">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-183">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="4a392-183">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="4a392-184">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-184">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="4a392-185">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="4a392-185">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="4a392-186">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-186">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="4a392-187">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="4a392-187">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="4a392-188">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-188">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-189">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="4a392-189">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="4a392-190">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-190">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-191">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="4a392-191">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="4a392-192">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-192">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="4a392-193">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="4a392-193">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="4a392-194">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-194">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="4a392-195">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="4a392-195">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="4a392-196">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a392-196">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a392-197">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a392-197">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a392-198">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4a392-198">Optional query parameters</span></span>

<span data-ttu-id="4a392-199">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4a392-199">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a392-200">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a392-200">Request headers</span></span>
|<span data-ttu-id="4a392-201">标头</span><span class="sxs-lookup"><span data-stu-id="4a392-201">Header</span></span>|<span data-ttu-id="4a392-202">值</span><span class="sxs-lookup"><span data-stu-id="4a392-202">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a392-203">授权</span><span class="sxs-lookup"><span data-stu-id="4a392-203">Authorization</span></span>|<span data-ttu-id="4a392-204">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a392-204">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a392-205">接受</span><span class="sxs-lookup"><span data-stu-id="4a392-205">Accept</span></span>|<span data-ttu-id="4a392-206">application/json</span><span class="sxs-lookup"><span data-stu-id="4a392-206">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a392-207">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a392-207">Request body</span></span>

<span data-ttu-id="4a392-208">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4a392-208">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a392-209">响应</span><span class="sxs-lookup"><span data-stu-id="4a392-209">Response</span></span>

<span data-ttu-id="4a392-210">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a392-210">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a392-211">示例</span><span class="sxs-lookup"><span data-stu-id="4a392-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a392-212">请求</span><span class="sxs-lookup"><span data-stu-id="4a392-212">Request</span></span>

<span data-ttu-id="4a392-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a392-213">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="4a392-214">响应</span><span class="sxs-lookup"><span data-stu-id="4a392-214">Response</span></span>

<span data-ttu-id="4a392-215">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="4a392-215">Here are example of the response.</span></span> 

<span data-ttu-id="4a392-216">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4a392-216">Note: The response objects shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="4a392-217">将返回适用于工作流的属性。</span><span class="sxs-lookup"><span data-stu-id="4a392-217">Properties appropriate for the workflow are returned.</span></span>

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











