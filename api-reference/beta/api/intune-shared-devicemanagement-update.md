---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e0dc83489ede464eb9da000acb8db4e6af13f8d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527047"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="d7327-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="d7327-103">Update deviceManagement</span></span>

> <span data-ttu-id="d7327-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d7327-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d7327-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d7327-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7327-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7327-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7327-107">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d7327-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7327-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d7327-108">Prerequisites</span></span>

<span data-ttu-id="d7327-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7327-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d7327-111">请注意, 该权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="d7327-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="d7327-112">权限&nbsp;类型&nbsp;(按&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="d7327-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="d7327-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d7327-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="d7327-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7327-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="d7327-115">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="d7327-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="d7327-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="d7327-117">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="d7327-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="d7327-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-119">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="d7327-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="d7327-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="d7327-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d7327-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-123">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="d7327-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="d7327-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="d7327-125">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="d7327-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="d7327-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-127">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="d7327-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="d7327-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-129">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="d7327-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="d7327-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-131">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="d7327-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="d7327-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-133">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="d7327-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="d7327-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-135">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="d7327-135">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d7327-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-137">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="d7327-137">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="d7327-138">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-138">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-139">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="d7327-139">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="d7327-140">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7327-140">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="d7327-141">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="d7327-141">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="d7327-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-143">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="d7327-143">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="d7327-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-145">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="d7327-145">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="d7327-146">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-146">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-147">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="d7327-147">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="d7327-148">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7327-148">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d7327-149">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7327-149">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7327-150">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7327-150">Not supported.</span></span>|
| <span data-ttu-id="d7327-151">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7327-151">Application</span></span> | <span data-ttu-id="d7327-152">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7327-152">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7327-153">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7327-153">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="d7327-154">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7327-154">Request headers</span></span>

|<span data-ttu-id="d7327-155">标头</span><span class="sxs-lookup"><span data-stu-id="d7327-155">Header</span></span>|<span data-ttu-id="d7327-156">值</span><span class="sxs-lookup"><span data-stu-id="d7327-156">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7327-157">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7327-157">Authorization</span></span>|<span data-ttu-id="d7327-158">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d7327-158">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7327-159">接受</span><span class="sxs-lookup"><span data-stu-id="d7327-159">Accept</span></span>|<span data-ttu-id="d7327-160">application/json</span><span class="sxs-lookup"><span data-stu-id="d7327-160">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7327-161">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7327-161">Request body</span></span>

<span data-ttu-id="d7327-162">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7327-162">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="d7327-163">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d7327-163">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="d7327-164">属性</span><span class="sxs-lookup"><span data-stu-id="d7327-164">Property</span></span>|<span data-ttu-id="d7327-165">类型</span><span class="sxs-lookup"><span data-stu-id="d7327-165">Type</span></span>|<span data-ttu-id="d7327-166">说明</span><span class="sxs-lookup"><span data-stu-id="d7327-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7327-167">id</span><span class="sxs-lookup"><span data-stu-id="d7327-167">id</span></span>|<span data-ttu-id="d7327-168">String</span><span class="sxs-lookup"><span data-stu-id="d7327-168">String</span></span>|<span data-ttu-id="d7327-169">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d7327-169">Unique identifier for the device.</span></span>|
|<span data-ttu-id="d7327-170">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="d7327-170">**Device configuration**</span></span>|
|<span data-ttu-id="d7327-171">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="d7327-171">intuneAccountId</span></span>|<span data-ttu-id="d7327-172">GUID</span><span class="sxs-lookup"><span data-stu-id="d7327-172">GUID</span></span>|<span data-ttu-id="d7327-173">给定租户的 Intune 帐户 ID</span><span class="sxs-lookup"><span data-stu-id="d7327-173">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="d7327-174">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="d7327-174">legacyPcManangementEnabled</span></span>|<span data-ttu-id="d7327-175">布尔值</span><span class="sxs-lookup"><span data-stu-id="d7327-175">Boolean</span></span>|<span data-ttu-id="d7327-176">用于为此帐户启用非 MDM 托管旧版 PC 管理的属性。</span><span class="sxs-lookup"><span data-stu-id="d7327-176">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="d7327-177">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d7327-177">This property is read-only.</span></span>|
|<span data-ttu-id="d7327-178">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="d7327-178">maximumDepTokens</span></span>|<span data-ttu-id="d7327-179">Int32</span><span class="sxs-lookup"><span data-stu-id="d7327-179">Int32</span></span>|<span data-ttu-id="d7327-180">每个租户允许的最大 DEP 令牌数。</span><span class="sxs-lookup"><span data-stu-id="d7327-180">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="d7327-181">settings</span><span class="sxs-lookup"><span data-stu-id="d7327-181">settings</span></span>|[<span data-ttu-id="d7327-182">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="d7327-182">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="d7327-183">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="d7327-183">Account level settings.</span></span>|
|<span data-ttu-id="d7327-184">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="d7327-184">**Device management**</span></span>|
|<span data-ttu-id="d7327-185">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="d7327-185">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="d7327-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7327-186">DateTimeOffset</span></span>|<span data-ttu-id="d7327-187">在 scaleunits 之间移动租户数据的日期 & 时间。</span><span class="sxs-lookup"><span data-stu-id="d7327-187">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="d7327-188">adminConsent</span><span class="sxs-lookup"><span data-stu-id="d7327-188">adminConsent</span></span>|[<span data-ttu-id="d7327-189">adminConsent</span><span class="sxs-lookup"><span data-stu-id="d7327-189">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="d7327-190">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="d7327-190">Admin consent information.</span></span>|
|<span data-ttu-id="d7327-191">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="d7327-191">deviceProtectionOverview</span></span>|[<span data-ttu-id="d7327-192">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="d7327-192">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="d7327-193">设备保护概述。</span><span class="sxs-lookup"><span data-stu-id="d7327-193">Device protection overview.</span></span>|
|<span data-ttu-id="d7327-194">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="d7327-194">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="d7327-195">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="d7327-195">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="d7327-196">设备清理规则</span><span class="sxs-lookup"><span data-stu-id="d7327-196">Device cleanup rule</span></span>|
|<span data-ttu-id="d7327-197">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="d7327-197">subscriptionState</span></span>|[<span data-ttu-id="d7327-198">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="d7327-198">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="d7327-199">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="d7327-199">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="d7327-200">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="d7327-200">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="d7327-201">订阅</span><span class="sxs-lookup"><span data-stu-id="d7327-201">subscriptions</span></span>|[<span data-ttu-id="d7327-202">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="d7327-202">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="d7327-203">租户的订阅。</span><span class="sxs-lookup"><span data-stu-id="d7327-203">Tenant's Subscription.</span></span> <span data-ttu-id="d7327-204">可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="d7327-204">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="d7327-205">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="d7327-205">windowsMalwareOverview</span></span>|[<span data-ttu-id="d7327-206">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="d7327-206">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="d7327-207">windows 设备的恶意软件概述。</span><span class="sxs-lookup"><span data-stu-id="d7327-207">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="d7327-208">**载入**</span><span class="sxs-lookup"><span data-stu-id="d7327-208">**Onboarding**</span></span>|
|<span data-ttu-id="d7327-209">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="d7327-209">intuneBrand</span></span>|[<span data-ttu-id="d7327-210">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="d7327-210">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="d7327-211">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="d7327-211">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="d7327-212">请求正文属性支持因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="d7327-212">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="d7327-213">响应</span><span class="sxs-lookup"><span data-stu-id="d7327-213">Response</span></span>
<span data-ttu-id="d7327-214">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d7327-214">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7327-215">示例</span><span class="sxs-lookup"><span data-stu-id="d7327-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7327-216">请求</span><span class="sxs-lookup"><span data-stu-id="d7327-216">Request</span></span>

<span data-ttu-id="d7327-217">下面的示例展示了设备管理工作流后的请求:</span><span class="sxs-lookup"><span data-stu-id="d7327-217">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="d7327-218">响应</span><span class="sxs-lookup"><span data-stu-id="d7327-218">Response</span></span>

<span data-ttu-id="d7327-219">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d7327-219">Here is an example of the response.</span></span> 

<span data-ttu-id="d7327-220">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d7327-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d7327-221">返回的属性根据工作流和上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="d7327-221">Returned properties vary according to workflow and context.</span></span>

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



