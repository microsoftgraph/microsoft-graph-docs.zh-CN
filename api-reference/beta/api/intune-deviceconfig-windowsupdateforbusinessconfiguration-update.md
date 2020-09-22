---
title: 更新 windowsUpdateForBusinessConfiguration
description: 更新 windowsUpdateForBusinessConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff8bd6956b012dee4ba181cf9b27e00910b920bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011470"
---
# <a name="update-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="88952-103">更新 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="88952-103">Update windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="88952-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88952-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88952-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88952-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88952-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88952-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88952-107">更新 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88952-107">Update the properties of a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88952-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88952-108">Prerequisites</span></span>
<span data-ttu-id="88952-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88952-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88952-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88952-111">Permission type</span></span>|<span data-ttu-id="88952-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88952-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88952-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88952-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88952-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88952-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88952-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88952-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88952-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88952-116">Not supported.</span></span>|
|<span data-ttu-id="88952-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88952-117">Application</span></span>|<span data-ttu-id="88952-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88952-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88952-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88952-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="88952-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88952-120">Request headers</span></span>
|<span data-ttu-id="88952-121">标头</span><span class="sxs-lookup"><span data-stu-id="88952-121">Header</span></span>|<span data-ttu-id="88952-122">值</span><span class="sxs-lookup"><span data-stu-id="88952-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88952-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88952-123">Authorization</span></span>|<span data-ttu-id="88952-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88952-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88952-125">接受</span><span class="sxs-lookup"><span data-stu-id="88952-125">Accept</span></span>|<span data-ttu-id="88952-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88952-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88952-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88952-127">Request body</span></span>
<span data-ttu-id="88952-128">在请求正文中，提供 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88952-128">In the request body, supply a JSON representation for the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="88952-129">下表显示创建 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88952-129">The following table shows the properties that are required when you create the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="88952-130">属性</span><span class="sxs-lookup"><span data-stu-id="88952-130">Property</span></span>|<span data-ttu-id="88952-131">类型</span><span class="sxs-lookup"><span data-stu-id="88952-131">Type</span></span>|<span data-ttu-id="88952-132">说明</span><span class="sxs-lookup"><span data-stu-id="88952-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88952-133">id</span><span class="sxs-lookup"><span data-stu-id="88952-133">id</span></span>|<span data-ttu-id="88952-134">String</span><span class="sxs-lookup"><span data-stu-id="88952-134">String</span></span>|<span data-ttu-id="88952-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88952-135">Key of the entity.</span></span> <span data-ttu-id="88952-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88952-137">lastModifiedDateTime</span></span>|<span data-ttu-id="88952-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88952-138">DateTimeOffset</span></span>|<span data-ttu-id="88952-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88952-139">DateTime the object was last modified.</span></span> <span data-ttu-id="88952-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88952-141">roleScopeTagIds</span></span>|<span data-ttu-id="88952-142">String collection</span><span class="sxs-lookup"><span data-stu-id="88952-142">String collection</span></span>|<span data-ttu-id="88952-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="88952-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="88952-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="88952-145">supportsScopeTags</span></span>|<span data-ttu-id="88952-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-146">Boolean</span></span>|<span data-ttu-id="88952-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="88952-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="88952-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="88952-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="88952-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="88952-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="88952-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88952-150">This property is read-only.</span></span> <span data-ttu-id="88952-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88952-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="88952-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88952-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="88952-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="88952-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="88952-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88952-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="88952-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88952-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="88952-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="88952-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="88952-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88952-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="88952-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88952-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="88952-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="88952-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="88952-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88952-164">createdDateTime</span></span>|<span data-ttu-id="88952-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88952-165">DateTimeOffset</span></span>|<span data-ttu-id="88952-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88952-166">DateTime the object was created.</span></span> <span data-ttu-id="88952-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-168">description</span><span class="sxs-lookup"><span data-stu-id="88952-168">description</span></span>|<span data-ttu-id="88952-169">String</span><span class="sxs-lookup"><span data-stu-id="88952-169">String</span></span>|<span data-ttu-id="88952-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="88952-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88952-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-172">displayName</span><span class="sxs-lookup"><span data-stu-id="88952-172">displayName</span></span>|<span data-ttu-id="88952-173">String</span><span class="sxs-lookup"><span data-stu-id="88952-173">String</span></span>|<span data-ttu-id="88952-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="88952-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88952-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-176">version</span><span class="sxs-lookup"><span data-stu-id="88952-176">version</span></span>|<span data-ttu-id="88952-177">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-177">Int32</span></span>|<span data-ttu-id="88952-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="88952-178">Version of the device configuration.</span></span> <span data-ttu-id="88952-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88952-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88952-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="88952-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="88952-181">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="88952-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="88952-182">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="88952-182">Delivery Optimization Mode.</span></span> <span data-ttu-id="88952-183">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="88952-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="88952-184">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="88952-184">prereleaseFeatures</span></span>|[<span data-ttu-id="88952-185">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="88952-185">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="88952-186">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="88952-186">The pre-release features.</span></span> <span data-ttu-id="88952-187">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="88952-187">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="88952-188">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="88952-188">automaticUpdateMode</span></span>|[<span data-ttu-id="88952-189">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="88952-189">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="88952-190">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="88952-190">Automatic update mode.</span></span> <span data-ttu-id="88952-191">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl` 或 `windowsDefault`。</span><span class="sxs-lookup"><span data-stu-id="88952-191">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`, `windowsDefault`.</span></span>|
|<span data-ttu-id="88952-192">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="88952-192">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="88952-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-193">Boolean</span></span>|<span data-ttu-id="88952-194">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="88952-194">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="88952-195">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="88952-195">driversExcluded</span></span>|<span data-ttu-id="88952-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-196">Boolean</span></span>|<span data-ttu-id="88952-197">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="88952-197">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="88952-198">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="88952-198">installationSchedule</span></span>|[<span data-ttu-id="88952-199">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="88952-199">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="88952-200">安装计划</span><span class="sxs-lookup"><span data-stu-id="88952-200">Installation schedule</span></span>|
|<span data-ttu-id="88952-201">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="88952-201">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="88952-202">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-202">Int32</span></span>|<span data-ttu-id="88952-203">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="88952-203">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="88952-204">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="88952-204">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="88952-205">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-205">Int32</span></span>|<span data-ttu-id="88952-206">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="88952-206">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="88952-207">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="88952-207">qualityUpdatesPaused</span></span>|<span data-ttu-id="88952-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-208">Boolean</span></span>|<span data-ttu-id="88952-209">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="88952-209">Pause Quality Updates</span></span>|
|<span data-ttu-id="88952-210">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="88952-210">featureUpdatesPaused</span></span>|<span data-ttu-id="88952-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-211">Boolean</span></span>|<span data-ttu-id="88952-212">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="88952-212">Pause Feature Updates</span></span>|
|<span data-ttu-id="88952-213">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="88952-213">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="88952-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88952-214">DateTimeOffset</span></span>|<span data-ttu-id="88952-215">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="88952-215">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="88952-216">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="88952-216">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="88952-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88952-217">DateTimeOffset</span></span>|<span data-ttu-id="88952-218">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="88952-218">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="88952-219">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="88952-219">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="88952-220">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="88952-220">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="88952-221">确定将从哪些分支设备接收其更新。</span><span class="sxs-lookup"><span data-stu-id="88952-221">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="88952-222">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="88952-222">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|
|<span data-ttu-id="88952-223">skipChecksBeforeRestart</span><span class="sxs-lookup"><span data-stu-id="88952-223">skipChecksBeforeRestart</span></span>|<span data-ttu-id="88952-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-224">Boolean</span></span>|<span data-ttu-id="88952-225">设置为在重新启动之前跳过所有复选：电池级别 = 40%、用户状态、需要显示、演示模式、全屏模式、电话呼叫状态、游戏模式等。</span><span class="sxs-lookup"><span data-stu-id="88952-225">Set to skip all check before restart: Battery level = 40%, User presence, Display Needed, Presentation mode, Full screen mode, phone call state, game mode etc.</span></span> |
|<span data-ttu-id="88952-226">updateWeeks</span><span class="sxs-lookup"><span data-stu-id="88952-226">updateWeeks</span></span>|[<span data-ttu-id="88952-227">windowsUpdateForBusinessUpdateWeeks</span><span class="sxs-lookup"><span data-stu-id="88952-227">windowsUpdateForBusinessUpdateWeeks</span></span>](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|<span data-ttu-id="88952-228">在每月的几周安排更新安装。</span><span class="sxs-lookup"><span data-stu-id="88952-228">Scheduled the update installation on the weeks of the month.</span></span> <span data-ttu-id="88952-229">可取值为：`userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。</span><span class="sxs-lookup"><span data-stu-id="88952-229">Possible values are: `userDefined`, `firstWeek`, `secondWeek`, `thirdWeek`, `fourthWeek`, `everyWeek`.</span></span>|
|<span data-ttu-id="88952-230">qualityUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="88952-230">qualityUpdatesPauseStartDate</span></span>|<span data-ttu-id="88952-231">日期</span><span class="sxs-lookup"><span data-stu-id="88952-231">Date</span></span>|<span data-ttu-id="88952-232">质量更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="88952-232">Quality Updates Pause start date.</span></span> <span data-ttu-id="88952-233">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88952-233">This property is read-only.</span></span>|
|<span data-ttu-id="88952-234">featureUpdatesPauseStartDate</span><span class="sxs-lookup"><span data-stu-id="88952-234">featureUpdatesPauseStartDate</span></span>|<span data-ttu-id="88952-235">日期</span><span class="sxs-lookup"><span data-stu-id="88952-235">Date</span></span>|<span data-ttu-id="88952-236">功能更新暂停开始日期。</span><span class="sxs-lookup"><span data-stu-id="88952-236">Feature Updates Pause start date.</span></span> <span data-ttu-id="88952-237">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88952-237">This property is read-only.</span></span>|
|<span data-ttu-id="88952-238">featureUpdatesRollbackWindowInDays</span><span class="sxs-lookup"><span data-stu-id="88952-238">featureUpdatesRollbackWindowInDays</span></span>|<span data-ttu-id="88952-239">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-239">Int32</span></span>|<span data-ttu-id="88952-240">回滚对其有效的功能更新后的天数</span><span class="sxs-lookup"><span data-stu-id="88952-240">The number of days after a Feature Update for which a rollback is valid</span></span>|
|<span data-ttu-id="88952-241">qualityUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="88952-241">qualityUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="88952-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-242">Boolean</span></span>|<span data-ttu-id="88952-243">指定是否在下一个设备签入时回滚质量更新</span><span class="sxs-lookup"><span data-stu-id="88952-243">Specifies whether to rollback Quality Updates on the next device check in</span></span>|
|<span data-ttu-id="88952-244">featureUpdatesWillBeRolledBack</span><span class="sxs-lookup"><span data-stu-id="88952-244">featureUpdatesWillBeRolledBack</span></span>|<span data-ttu-id="88952-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-245">Boolean</span></span>|<span data-ttu-id="88952-246">指定是否在下一个设备签入时回滚功能更新</span><span class="sxs-lookup"><span data-stu-id="88952-246">Specifies whether to rollback Feature Updates on the next device check in</span></span>|
|<span data-ttu-id="88952-247">qualityUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="88952-247">qualityUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="88952-248">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88952-248">DateTimeOffset</span></span>|<span data-ttu-id="88952-249">质量更新回滚开始日期/时间</span><span class="sxs-lookup"><span data-stu-id="88952-249">Quality Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="88952-250">featureUpdatesRollbackStartDateTime</span><span class="sxs-lookup"><span data-stu-id="88952-250">featureUpdatesRollbackStartDateTime</span></span>|<span data-ttu-id="88952-251">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88952-251">DateTimeOffset</span></span>|<span data-ttu-id="88952-252">功能更新回滚的开始日期时间</span><span class="sxs-lookup"><span data-stu-id="88952-252">Feature Updates Rollback Start datetime</span></span>|
|<span data-ttu-id="88952-253">engagedRestartDeadlineInDays</span><span class="sxs-lookup"><span data-stu-id="88952-253">engagedRestartDeadlineInDays</span></span>|<span data-ttu-id="88952-254">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-254">Int32</span></span>|<span data-ttu-id="88952-255">在非活动时段自动安排和执行挂起的重启的期限（以天为单位），有效范围为2到30天</span><span class="sxs-lookup"><span data-stu-id="88952-255">Deadline in days before automatically scheduling and executing a pending restart outside of active hours, with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="88952-256">engagedRestartSnoozeScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="88952-256">engagedRestartSnoozeScheduleInDays</span></span>|<span data-ttu-id="88952-257">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-257">Int32</span></span>|<span data-ttu-id="88952-258">用户可推迟预定重启提醒通知的天数，有效范围为1到3天</span><span class="sxs-lookup"><span data-stu-id="88952-258">Number of days a user can snooze Engaged Restart reminder notifications with valid range from 1 to 3 days</span></span>|
|<span data-ttu-id="88952-259">engagedRestartTransitionScheduleInDays</span><span class="sxs-lookup"><span data-stu-id="88952-259">engagedRestartTransitionScheduleInDays</span></span>|<span data-ttu-id="88952-260">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-260">Int32</span></span>|<span data-ttu-id="88952-261">从主动时段之外的计划的自动重启转换为预定重启（需要用户进行计划，有效范围为0到30天）的天数</span><span class="sxs-lookup"><span data-stu-id="88952-261">Number of days before transitioning from Auto Restarts scheduled outside of active hours to Engaged Restart, which requires the user to schedule, with valid range from 0 to 30 days</span></span>|
|<span data-ttu-id="88952-262">deadlineForFeatureUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="88952-262">deadlineForFeatureUpdatesInDays</span></span>|<span data-ttu-id="88952-263">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-263">Int32</span></span>|<span data-ttu-id="88952-264">自动安装具有介于2到30天的有效范围的功能更新之前的天数</span><span class="sxs-lookup"><span data-stu-id="88952-264">Number of days before feature updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="88952-265">deadlineForQualityUpdatesInDays</span><span class="sxs-lookup"><span data-stu-id="88952-265">deadlineForQualityUpdatesInDays</span></span>|<span data-ttu-id="88952-266">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-266">Int32</span></span>|<span data-ttu-id="88952-267">自动安装质量更新前的天数介于2到30天的有效范围内</span><span class="sxs-lookup"><span data-stu-id="88952-267">Number of days before quality updates are installed automatically with valid range from 2 to 30 days</span></span>|
|<span data-ttu-id="88952-268">deadlineGracePeriodInDays</span><span class="sxs-lookup"><span data-stu-id="88952-268">deadlineGracePeriodInDays</span></span>|<span data-ttu-id="88952-269">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-269">Int32</span></span>|<span data-ttu-id="88952-270">使用有效范围（范围为0到7天）自动重新启动之前的最后期限的天数</span><span class="sxs-lookup"><span data-stu-id="88952-270">Number of days after deadline  until restarts occur automatically with valid range from 0 to 7 days</span></span>|
|<span data-ttu-id="88952-271">postponeRebootUntilAfterDeadline</span><span class="sxs-lookup"><span data-stu-id="88952-271">postponeRebootUntilAfterDeadline</span></span>|<span data-ttu-id="88952-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="88952-272">Boolean</span></span>|<span data-ttu-id="88952-273">指定设备是否应等到最后期限结束后才能在 active 时段之外进行重新启动</span><span class="sxs-lookup"><span data-stu-id="88952-273">Specifies if the device should wait until deadline for rebooting outside of active hours</span></span>|
|<span data-ttu-id="88952-274">autoRestartNotificationDismissal</span><span class="sxs-lookup"><span data-stu-id="88952-274">autoRestartNotificationDismissal</span></span>|[<span data-ttu-id="88952-275">autoRestartNotificationDismissalMethod</span><span class="sxs-lookup"><span data-stu-id="88952-275">autoRestartNotificationDismissalMethod</span></span>](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|<span data-ttu-id="88952-276">指定用于消除 "需要自动重新启动" 通知的方法。</span><span class="sxs-lookup"><span data-stu-id="88952-276">Specify the method by which the auto-restart required notification is dismissed.</span></span> <span data-ttu-id="88952-277">可取值为：`notConfigured`、`automatic`、`user`。</span><span class="sxs-lookup"><span data-stu-id="88952-277">Possible values are: `notConfigured`, `automatic`, `user`.</span></span>|
|<span data-ttu-id="88952-278">scheduleRestartWarningInHours</span><span class="sxs-lookup"><span data-stu-id="88952-278">scheduleRestartWarningInHours</span></span>|<span data-ttu-id="88952-279">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-279">Int32</span></span>|<span data-ttu-id="88952-280">指定自动重新启动警告提醒通知的期限。</span><span class="sxs-lookup"><span data-stu-id="88952-280">Specify the period for auto-restart warning reminder notifications.</span></span> <span data-ttu-id="88952-281">受支持的值：2、4、8、12或 24 (小时) 。</span><span class="sxs-lookup"><span data-stu-id="88952-281">Supported values: 2, 4, 8, 12 or 24 (hours).</span></span>|
|<span data-ttu-id="88952-282">scheduleImminentRestartWarningInMinutes</span><span class="sxs-lookup"><span data-stu-id="88952-282">scheduleImminentRestartWarningInMinutes</span></span>|<span data-ttu-id="88952-283">Int32</span><span class="sxs-lookup"><span data-stu-id="88952-283">Int32</span></span>|<span data-ttu-id="88952-284">指定自动重启即将发生的警告通知的期限。</span><span class="sxs-lookup"><span data-stu-id="88952-284">Specify the period for auto-restart imminent warning notifications.</span></span> <span data-ttu-id="88952-285">支持的值：15、30或 60 (分钟) 。</span><span class="sxs-lookup"><span data-stu-id="88952-285">Supported values: 15, 30 or 60 (minutes).</span></span>|
|<span data-ttu-id="88952-286">userPauseAccess</span><span class="sxs-lookup"><span data-stu-id="88952-286">userPauseAccess</span></span>|[<span data-ttu-id="88952-287">启用</span><span class="sxs-lookup"><span data-stu-id="88952-287">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="88952-288">指定是否允许最终用户访问暂停软件更新。</span><span class="sxs-lookup"><span data-stu-id="88952-288">Specifies whether to enable end user’s access to pause software updates.</span></span> <span data-ttu-id="88952-289">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="88952-289">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="88952-290">userWindowsUpdateScanAccess</span><span class="sxs-lookup"><span data-stu-id="88952-290">userWindowsUpdateScanAccess</span></span>|[<span data-ttu-id="88952-291">启用</span><span class="sxs-lookup"><span data-stu-id="88952-291">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="88952-292">指定是否禁用用户对扫描 Windows 更新的访问权限。</span><span class="sxs-lookup"><span data-stu-id="88952-292">Specifies whether to disable user’s access to scan Windows Update.</span></span> <span data-ttu-id="88952-293">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="88952-293">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="88952-294">updateNotificationLevel</span><span class="sxs-lookup"><span data-stu-id="88952-294">updateNotificationLevel</span></span>|[<span data-ttu-id="88952-295">windowsUpdateNotificationDisplayOption</span><span class="sxs-lookup"><span data-stu-id="88952-295">windowsUpdateNotificationDisplayOption</span></span>](../resources/intune-deviceconfig-windowsupdatenotificationdisplayoption.md)|<span data-ttu-id="88952-296">指定用户看到的 Windows 更新通知的具体内容。</span><span class="sxs-lookup"><span data-stu-id="88952-296">Specifies what Windows Update notifications users see.</span></span> <span data-ttu-id="88952-297">可取值为：`notConfigured`、`defaultNotifications`、`restartWarningsOnly`、`disableAllNotifications`。</span><span class="sxs-lookup"><span data-stu-id="88952-297">Possible values are: `notConfigured`, `defaultNotifications`, `restartWarningsOnly`, `disableAllNotifications`.</span></span>|



## <a name="response"></a><span data-ttu-id="88952-298">响应</span><span class="sxs-lookup"><span data-stu-id="88952-298">Response</span></span>
<span data-ttu-id="88952-299">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88952-299">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88952-300">示例</span><span class="sxs-lookup"><span data-stu-id="88952-300">Example</span></span>

### <a name="request"></a><span data-ttu-id="88952-301">请求</span><span class="sxs-lookup"><span data-stu-id="88952-301">Request</span></span>
<span data-ttu-id="88952-302">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88952-302">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2794

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```

### <a name="response"></a><span data-ttu-id="88952-303">响应</span><span class="sxs-lookup"><span data-stu-id="88952-303">Response</span></span>
<span data-ttu-id="88952-p126">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88952-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2966

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "firstWeek",
  "qualityUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesPauseStartDate": "2016-12-31",
  "featureUpdatesRollbackWindowInDays": 2,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
  "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
  "engagedRestartDeadlineInDays": 12,
  "engagedRestartSnoozeScheduleInDays": 2,
  "engagedRestartTransitionScheduleInDays": 6,
  "deadlineForFeatureUpdatesInDays": 15,
  "deadlineForQualityUpdatesInDays": 15,
  "deadlineGracePeriodInDays": 9,
  "postponeRebootUntilAfterDeadline": true,
  "autoRestartNotificationDismissal": "automatic",
  "scheduleRestartWarningInHours": 13,
  "scheduleImminentRestartWarningInMinutes": 7,
  "userPauseAccess": "enabled",
  "userWindowsUpdateScanAccess": "enabled",
  "updateNotificationLevel": "defaultNotifications"
}
```






