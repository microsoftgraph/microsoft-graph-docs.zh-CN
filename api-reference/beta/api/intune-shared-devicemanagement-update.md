---
title: 更新 deviceManagement
description: 更新 deviceManagement 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a77605170d7df943b0d1a96fc2fe864b9d46e4f7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989691"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="77d75-103">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="77d75-103">Update deviceManagement</span></span>

> <span data-ttu-id="77d75-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="77d75-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77d75-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="77d75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77d75-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77d75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77d75-107">更新 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77d75-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77d75-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="77d75-108">Prerequisites</span></span>

<span data-ttu-id="77d75-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77d75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="77d75-111">请注意, 该权限根据工作流的不同而有所不同。</span><span class="sxs-lookup"><span data-stu-id="77d75-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="77d75-112">权限&nbsp;类型&nbsp;(按&nbsp;工作流)</span><span class="sxs-lookup"><span data-stu-id="77d75-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="77d75-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77d75-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="77d75-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77d75-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="77d75-115">&nbsp;&nbsp; **适用于工作的 Android**</span><span class="sxs-lookup"><span data-stu-id="77d75-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="77d75-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="77d75-117">&nbsp; &nbsp; **审核**</span><span class="sxs-lookup"><span data-stu-id="77d75-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="77d75-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-119">&nbsp; &nbsp; **公司条款**</span><span class="sxs-lookup"><span data-stu-id="77d75-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="77d75-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="77d75-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="77d75-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-123">&nbsp;&nbsp; **设备意向**</span><span class="sxs-lookup"><span data-stu-id="77d75-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="77d75-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="77d75-125">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="77d75-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="77d75-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-127">&nbsp;&nbsp; **电子 SIM**</span><span class="sxs-lookup"><span data-stu-id="77d75-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="77d75-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-129">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="77d75-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="77d75-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-131">&nbsp;&nbsp; **防护**</span><span class="sxs-lookup"><span data-stu-id="77d75-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="77d75-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-133">&nbsp;&nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="77d75-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="77d75-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="77d75-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="77d75-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-137">&nbsp; &nbsp; **载入**</span><span class="sxs-lookup"><span data-stu-id="77d75-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="77d75-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-139">&nbsp; &nbsp; **基于角色的访问控制 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="77d75-139">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="77d75-140">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-140">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-141">&nbsp;&nbsp; **远程访问**</span><span class="sxs-lookup"><span data-stu-id="77d75-141">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="77d75-142">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="77d75-142">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="77d75-143">&nbsp;&nbsp; **远程协助**</span><span class="sxs-lookup"><span data-stu-id="77d75-143">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="77d75-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-145">&nbsp;&nbsp; **电信费用管理**</span><span class="sxs-lookup"><span data-stu-id="77d75-145">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="77d75-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-147">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="77d75-147">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="77d75-148">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-148">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-149">&nbsp; &nbsp; **Windows 信息保护**</span><span class="sxs-lookup"><span data-stu-id="77d75-149">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="77d75-150">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77d75-150">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="77d75-151">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77d75-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77d75-152">不支持。</span><span class="sxs-lookup"><span data-stu-id="77d75-152">Not supported.</span></span>|
| <span data-ttu-id="77d75-153">应用程序</span><span class="sxs-lookup"><span data-stu-id="77d75-153">Application</span></span> | <span data-ttu-id="77d75-154">不支持。</span><span class="sxs-lookup"><span data-stu-id="77d75-154">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77d75-155">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77d75-155">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="77d75-156">请求标头</span><span class="sxs-lookup"><span data-stu-id="77d75-156">Request headers</span></span>

|<span data-ttu-id="77d75-157">标头</span><span class="sxs-lookup"><span data-stu-id="77d75-157">Header</span></span>|<span data-ttu-id="77d75-158">值</span><span class="sxs-lookup"><span data-stu-id="77d75-158">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77d75-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="77d75-159">Authorization</span></span>|<span data-ttu-id="77d75-160">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77d75-160">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77d75-161">接受</span><span class="sxs-lookup"><span data-stu-id="77d75-161">Accept</span></span>|<span data-ttu-id="77d75-162">application/json</span><span class="sxs-lookup"><span data-stu-id="77d75-162">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77d75-163">请求正文</span><span class="sxs-lookup"><span data-stu-id="77d75-163">Request body</span></span>

<span data-ttu-id="77d75-164">在请求正文中，提供 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77d75-164">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="77d75-165">下表显示创建 [deviceManagement](../resources/intune-shared-devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="77d75-165">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="77d75-166">属性</span><span class="sxs-lookup"><span data-stu-id="77d75-166">Property</span></span>|<span data-ttu-id="77d75-167">类型</span><span class="sxs-lookup"><span data-stu-id="77d75-167">Type</span></span>|<span data-ttu-id="77d75-168">说明</span><span class="sxs-lookup"><span data-stu-id="77d75-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77d75-169">id</span><span class="sxs-lookup"><span data-stu-id="77d75-169">id</span></span>|<span data-ttu-id="77d75-170">String</span><span class="sxs-lookup"><span data-stu-id="77d75-170">String</span></span>|<span data-ttu-id="77d75-171">设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="77d75-171">Unique identifier for the device.</span></span>|
|<span data-ttu-id="77d75-172">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="77d75-172">**Device configuration**</span></span>|
|<span data-ttu-id="77d75-173">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="77d75-173">intuneAccountId</span></span>|<span data-ttu-id="77d75-174">GUID</span><span class="sxs-lookup"><span data-stu-id="77d75-174">GUID</span></span>|<span data-ttu-id="77d75-175">给定租户的 Intune 帐户 ID</span><span class="sxs-lookup"><span data-stu-id="77d75-175">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="77d75-176">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="77d75-176">legacyPcManangementEnabled</span></span>|<span data-ttu-id="77d75-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="77d75-177">Boolean</span></span>|<span data-ttu-id="77d75-178">用于为此帐户启用非 MDM 托管旧版 PC 管理的属性。</span><span class="sxs-lookup"><span data-stu-id="77d75-178">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="77d75-179">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="77d75-179">This property is read-only.</span></span>|
|<span data-ttu-id="77d75-180">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="77d75-180">maximumDepTokens</span></span>|<span data-ttu-id="77d75-181">Int32</span><span class="sxs-lookup"><span data-stu-id="77d75-181">Int32</span></span>|<span data-ttu-id="77d75-182">每个租户允许的最大 DEP 令牌数。</span><span class="sxs-lookup"><span data-stu-id="77d75-182">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="77d75-183">settings</span><span class="sxs-lookup"><span data-stu-id="77d75-183">settings</span></span>|[<span data-ttu-id="77d75-184">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="77d75-184">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="77d75-185">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="77d75-185">Account level settings.</span></span>|
|<span data-ttu-id="77d75-186">**设备管理**</span><span class="sxs-lookup"><span data-stu-id="77d75-186">**Device management**</span></span>|
|<span data-ttu-id="77d75-187">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="77d75-187">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="77d75-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77d75-188">DateTimeOffset</span></span>|<span data-ttu-id="77d75-189">租户数据在 scaleunits 之间移动的日期 & 时间。</span><span class="sxs-lookup"><span data-stu-id="77d75-189">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="77d75-190">adminConsent</span><span class="sxs-lookup"><span data-stu-id="77d75-190">adminConsent</span></span>|[<span data-ttu-id="77d75-191">adminConsent</span><span class="sxs-lookup"><span data-stu-id="77d75-191">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="77d75-192">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="77d75-192">Admin consent information.</span></span>|
|<span data-ttu-id="77d75-193">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="77d75-193">deviceProtectionOverview</span></span>|[<span data-ttu-id="77d75-194">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="77d75-194">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="77d75-195">设备保护概述。</span><span class="sxs-lookup"><span data-stu-id="77d75-195">Device protection overview.</span></span>|
|<span data-ttu-id="77d75-196">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="77d75-196">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="77d75-197">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="77d75-197">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="77d75-198">设备清理规则</span><span class="sxs-lookup"><span data-stu-id="77d75-198">Device cleanup rule</span></span>|
|<span data-ttu-id="77d75-199">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="77d75-199">subscriptionState</span></span>|[<span data-ttu-id="77d75-200">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="77d75-200">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="77d75-201">租户移动设备管理订阅状态。</span><span class="sxs-lookup"><span data-stu-id="77d75-201">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="77d75-202">可取值为：`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。</span><span class="sxs-lookup"><span data-stu-id="77d75-202">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="77d75-203">订阅</span><span class="sxs-lookup"><span data-stu-id="77d75-203">subscriptions</span></span>|[<span data-ttu-id="77d75-204">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="77d75-204">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="77d75-205">租户的订阅。</span><span class="sxs-lookup"><span data-stu-id="77d75-205">Tenant's Subscription.</span></span> <span data-ttu-id="77d75-206">可取值为：`none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="77d75-206">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="77d75-207">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="77d75-207">windowsMalwareOverview</span></span>|[<span data-ttu-id="77d75-208">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="77d75-208">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="77d75-209">Windows 设备的恶意软件概述。</span><span class="sxs-lookup"><span data-stu-id="77d75-209">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="77d75-210">**载入**</span><span class="sxs-lookup"><span data-stu-id="77d75-210">**Onboarding**</span></span>|
|<span data-ttu-id="77d75-211">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="77d75-211">intuneBrand</span></span>|[<span data-ttu-id="77d75-212">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="77d75-212">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="77d75-213">intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="77d75-213">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="77d75-214">请求正文属性支持因工作流而异。</span><span class="sxs-lookup"><span data-stu-id="77d75-214">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="77d75-215">响应</span><span class="sxs-lookup"><span data-stu-id="77d75-215">Response</span></span>
<span data-ttu-id="77d75-216">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune-shared-devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77d75-216">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77d75-217">示例</span><span class="sxs-lookup"><span data-stu-id="77d75-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="77d75-218">请求</span><span class="sxs-lookup"><span data-stu-id="77d75-218">Request</span></span>

<span data-ttu-id="77d75-219">下面的示例展示了设备管理工作流后的请求:</span><span class="sxs-lookup"><span data-stu-id="77d75-219">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="77d75-220">响应</span><span class="sxs-lookup"><span data-stu-id="77d75-220">Response</span></span>

<span data-ttu-id="77d75-221">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="77d75-221">Here is an example of the response.</span></span> 

<span data-ttu-id="77d75-222">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="77d75-222">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="77d75-223">返回的属性根据工作流和上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="77d75-223">Returned properties vary according to workflow and context.</span></span>

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



