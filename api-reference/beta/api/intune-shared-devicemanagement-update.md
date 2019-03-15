---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a71212652d789b08a8cb496b6b98c18b12d3e9c7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571051"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="5d945-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5d945-103">Update deviceManagement</span></span>

> <span data-ttu-id="5d945-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5d945-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5d945-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5d945-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d945-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5d945-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d945-107">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5d945-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d945-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5d945-108">Prerequisites</span></span>

<span data-ttu-id="5d945-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5d945-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

<span data-ttu-id="5d945-111">请注意, 该权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="5d945-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="5d945-112">权限&nbsp;类型&nbsp;(按&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="5d945-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="5d945-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5d945-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="5d945-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d945-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="5d945-115">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="5d945-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="5d945-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="5d945-117">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="5d945-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="5d945-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-119">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="5d945-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="5d945-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="5d945-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5d945-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-123">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="5d945-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5d945-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-125">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="5d945-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="5d945-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-127">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="5d945-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="5d945-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-129">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="5d945-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="5d945-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-131">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="5d945-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="5d945-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-133">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="5d945-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5d945-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-135">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="5d945-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="5d945-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-137">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="5d945-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="5d945-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d945-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="5d945-139">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="5d945-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="5d945-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-141">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="5d945-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="5d945-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="5d945-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="5d945-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-145">&nbsp;&nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="5d945-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="5d945-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d945-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5d945-147">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d945-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d945-148">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d945-148">Not supported.</span></span>|
| <span data-ttu-id="5d945-149">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d945-149">Application</span></span> | <span data-ttu-id="5d945-150">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d945-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d945-151">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d945-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="5d945-152">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d945-152">Request headers</span></span>

|<span data-ttu-id="5d945-153">标头</span><span class="sxs-lookup"><span data-stu-id="5d945-153">Header</span></span>|<span data-ttu-id="5d945-154">值</span><span class="sxs-lookup"><span data-stu-id="5d945-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d945-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d945-155">Authorization</span></span>|<span data-ttu-id="5d945-156">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5d945-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d945-157">接受</span><span class="sxs-lookup"><span data-stu-id="5d945-157">Accept</span></span>|<span data-ttu-id="5d945-158">application/json</span><span class="sxs-lookup"><span data-stu-id="5d945-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d945-159">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d945-159">Request body</span></span>

<span data-ttu-id="5d945-160">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d945-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="5d945-161">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5d945-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="5d945-162">属性</span><span class="sxs-lookup"><span data-stu-id="5d945-162">Property</span></span>|<span data-ttu-id="5d945-163">类型</span><span class="sxs-lookup"><span data-stu-id="5d945-163">Type</span></span>|<span data-ttu-id="5d945-164">说明</span><span class="sxs-lookup"><span data-stu-id="5d945-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d945-165">id</span><span class="sxs-lookup"><span data-stu-id="5d945-165">id</span></span>|<span data-ttu-id="5d945-166">String</span><span class="sxs-lookup"><span data-stu-id="5d945-166">String</span></span>|<span data-ttu-id="5d945-167">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5d945-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="5d945-168">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="5d945-168">**Device configuration**</span></span>|
|<span data-ttu-id="5d945-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="5d945-169">intuneAccountId</span></span>|<span data-ttu-id="5d945-170">GUID</span><span class="sxs-lookup"><span data-stu-id="5d945-170">GUID</span></span>|<span data-ttu-id="5d945-171">给定租户的 Intune 帐户 ID</span><span class="sxs-lookup"><span data-stu-id="5d945-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="5d945-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="5d945-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="5d945-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d945-173">Boolean</span></span>|<span data-ttu-id="5d945-174">用于为此帐户启用非 MDM 托管旧版 PC 管理的属性。</span><span class="sxs-lookup"><span data-stu-id="5d945-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="5d945-175">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5d945-175">This property is read-only.</span></span>|
|<span data-ttu-id="5d945-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="5d945-176">maximumDepTokens</span></span>|<span data-ttu-id="5d945-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5d945-177">Int32</span></span>|<span data-ttu-id="5d945-178">每个租户允许的最大 DEP 令牌数。</span><span class="sxs-lookup"><span data-stu-id="5d945-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="5d945-179">settings</span><span class="sxs-lookup"><span data-stu-id="5d945-179">settings</span></span>|[<span data-ttu-id="5d945-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="5d945-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="5d945-181">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="5d945-181">Account level settings.</span></span>|
|<span data-ttu-id="5d945-182">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="5d945-182">**Device management**</span></span>|
|<span data-ttu-id="5d945-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="5d945-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="5d945-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d945-184">DateTimeOffset</span></span>|<span data-ttu-id="5d945-185">在 scaleunits 之间移动租户数据的日期 & 时间。</span><span class="sxs-lookup"><span data-stu-id="5d945-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="5d945-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="5d945-186">adminConsent</span></span>|[<span data-ttu-id="5d945-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="5d945-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="5d945-188">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="5d945-188">Admin consent information.</span></span>|
|<span data-ttu-id="5d945-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="5d945-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="5d945-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="5d945-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="5d945-191">设备保护概述。</span><span class="sxs-lookup"><span data-stu-id="5d945-191">Device protection overview.</span></span>|
|<span data-ttu-id="5d945-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="5d945-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="5d945-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="5d945-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="5d945-194">设备清理规则</span><span class="sxs-lookup"><span data-stu-id="5d945-194">Device cleanup rule</span></span>|
|<span data-ttu-id="5d945-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="5d945-195">subscriptionState</span></span>|[<span data-ttu-id="5d945-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="5d945-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="5d945-197">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="5d945-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="5d945-198">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="5d945-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="5d945-199">订阅</span><span class="sxs-lookup"><span data-stu-id="5d945-199">subscriptions</span></span>|[<span data-ttu-id="5d945-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="5d945-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="5d945-201">租户的订阅。</span><span class="sxs-lookup"><span data-stu-id="5d945-201">Tenant's Subscription.</span></span> <span data-ttu-id="5d945-202">可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="5d945-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="5d945-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="5d945-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="5d945-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="5d945-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="5d945-205">windows 设备的恶意软件概述。</span><span class="sxs-lookup"><span data-stu-id="5d945-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="5d945-206">**载入**</span><span class="sxs-lookup"><span data-stu-id="5d945-206">**Onboarding**</span></span>|
|<span data-ttu-id="5d945-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="5d945-207">intuneBrand</span></span>|[<span data-ttu-id="5d945-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="5d945-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="5d945-209">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="5d945-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="5d945-210">请求正文属性支持因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="5d945-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="5d945-211">响应</span><span class="sxs-lookup"><span data-stu-id="5d945-211">Response</span></span>
<span data-ttu-id="5d945-212">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d945-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d945-213">示例</span><span class="sxs-lookup"><span data-stu-id="5d945-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d945-214">请求</span><span class="sxs-lookup"><span data-stu-id="5d945-214">Request</span></span>

<span data-ttu-id="5d945-215">下面的示例展示了设备管理工作流后的请求:</span><span class="sxs-lookup"><span data-stu-id="5d945-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="5d945-216">响应</span><span class="sxs-lookup"><span data-stu-id="5d945-216">Response</span></span>

<span data-ttu-id="5d945-217">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5d945-217">Here is an example of the response.</span></span> 

<span data-ttu-id="5d945-218">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5d945-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5d945-219">返回的属性根据工作流和上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="5d945-219">Returned properties vary according to workflow and context.</span></span>

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



