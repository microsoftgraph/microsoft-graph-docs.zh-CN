---
title: 更新 iosUpdateConfiguration
description: 更新 iosUpdateConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c0009cc5a5d127ee9abbdbfe97f56591e2ba1a1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137397"
---
# <a name="update-iosupdateconfiguration"></a><span data-ttu-id="86ae0-103">更新 iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="86ae0-103">Update iosUpdateConfiguration</span></span>

<span data-ttu-id="86ae0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86ae0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86ae0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86ae0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86ae0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86ae0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86ae0-107">更新 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86ae0-107">Update the properties of a [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86ae0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="86ae0-108">Prerequisites</span></span>
<span data-ttu-id="86ae0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86ae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ae0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="86ae0-111">Permission type</span></span>|<span data-ttu-id="86ae0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86ae0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86ae0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86ae0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86ae0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ae0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86ae0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86ae0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86ae0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86ae0-116">Not supported.</span></span>|
|<span data-ttu-id="86ae0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="86ae0-117">Application</span></span>|<span data-ttu-id="86ae0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86ae0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86ae0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86ae0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="86ae0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86ae0-120">Request headers</span></span>
|<span data-ttu-id="86ae0-121">标头</span><span class="sxs-lookup"><span data-stu-id="86ae0-121">Header</span></span>|<span data-ttu-id="86ae0-122">值</span><span class="sxs-lookup"><span data-stu-id="86ae0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86ae0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86ae0-123">Authorization</span></span>|<span data-ttu-id="86ae0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86ae0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86ae0-125">接受</span><span class="sxs-lookup"><span data-stu-id="86ae0-125">Accept</span></span>|<span data-ttu-id="86ae0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86ae0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86ae0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86ae0-127">Request body</span></span>
<span data-ttu-id="86ae0-128">在请求正文中，提供 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86ae0-128">In the request body, supply a JSON representation for the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

<span data-ttu-id="86ae0-129">下表显示创建 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86ae0-129">The following table shows the properties that are required when you create the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md).</span></span>

|<span data-ttu-id="86ae0-130">属性</span><span class="sxs-lookup"><span data-stu-id="86ae0-130">Property</span></span>|<span data-ttu-id="86ae0-131">类型</span><span class="sxs-lookup"><span data-stu-id="86ae0-131">Type</span></span>|<span data-ttu-id="86ae0-132">说明</span><span class="sxs-lookup"><span data-stu-id="86ae0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86ae0-133">id</span><span class="sxs-lookup"><span data-stu-id="86ae0-133">id</span></span>|<span data-ttu-id="86ae0-134">String</span><span class="sxs-lookup"><span data-stu-id="86ae0-134">String</span></span>|<span data-ttu-id="86ae0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86ae0-135">Key of the entity.</span></span> <span data-ttu-id="86ae0-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86ae0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="86ae0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ae0-138">DateTimeOffset</span></span>|<span data-ttu-id="86ae0-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86ae0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="86ae0-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86ae0-141">roleScopeTagIds</span></span>|<span data-ttu-id="86ae0-142">String collection</span><span class="sxs-lookup"><span data-stu-id="86ae0-142">String collection</span></span>|<span data-ttu-id="86ae0-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="86ae0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86ae0-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86ae0-145">supportsScopeTags</span></span>|<span data-ttu-id="86ae0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae0-146">Boolean</span></span>|<span data-ttu-id="86ae0-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="86ae0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86ae0-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="86ae0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86ae0-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="86ae0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86ae0-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="86ae0-150">This property is read-only.</span></span> <span data-ttu-id="86ae0-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86ae0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="86ae0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86ae0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="86ae0-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="86ae0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="86ae0-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86ae0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="86ae0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86ae0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="86ae0-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="86ae0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="86ae0-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86ae0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="86ae0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86ae0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="86ae0-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="86ae0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="86ae0-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86ae0-164">createdDateTime</span></span>|<span data-ttu-id="86ae0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86ae0-165">DateTimeOffset</span></span>|<span data-ttu-id="86ae0-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86ae0-166">DateTime the object was created.</span></span> <span data-ttu-id="86ae0-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-168">说明</span><span class="sxs-lookup"><span data-stu-id="86ae0-168">description</span></span>|<span data-ttu-id="86ae0-169">String</span><span class="sxs-lookup"><span data-stu-id="86ae0-169">String</span></span>|<span data-ttu-id="86ae0-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="86ae0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86ae0-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="86ae0-172">displayName</span></span>|<span data-ttu-id="86ae0-173">String</span><span class="sxs-lookup"><span data-stu-id="86ae0-173">String</span></span>|<span data-ttu-id="86ae0-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="86ae0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86ae0-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-176">version</span><span class="sxs-lookup"><span data-stu-id="86ae0-176">version</span></span>|<span data-ttu-id="86ae0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae0-177">Int32</span></span>|<span data-ttu-id="86ae0-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="86ae0-178">Version of the device configuration.</span></span> <span data-ttu-id="86ae0-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86ae0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86ae0-180">isEnabled</span><span class="sxs-lookup"><span data-stu-id="86ae0-180">isEnabled</span></span>|<span data-ttu-id="86ae0-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ae0-181">Boolean</span></span>|<span data-ttu-id="86ae0-182">在 UI 中启用设置</span><span class="sxs-lookup"><span data-stu-id="86ae0-182">Is setting enabled in UI</span></span>|
|<span data-ttu-id="86ae0-183">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="86ae0-183">activeHoursStart</span></span>|<span data-ttu-id="86ae0-184">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="86ae0-184">TimeOfDay</span></span>|<span data-ttu-id="86ae0-185">使用时段开始时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="86ae0-185">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="86ae0-186">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="86ae0-186">activeHoursEnd</span></span>|<span data-ttu-id="86ae0-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="86ae0-187">TimeOfDay</span></span>|<span data-ttu-id="86ae0-188">使用时段结束时间（使用时段表示不应发生更新安装的时间范围）</span><span class="sxs-lookup"><span data-stu-id="86ae0-188">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="86ae0-189">desiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="86ae0-189">desiredOsVersion</span></span>|<span data-ttu-id="86ae0-190">String</span><span class="sxs-lookup"><span data-stu-id="86ae0-190">String</span></span>|<span data-ttu-id="86ae0-191">如果未指定，设备将更新到最新版本的操作系统。</span><span class="sxs-lookup"><span data-stu-id="86ae0-191">If left unspecified, devices will update to the latest version of the OS.</span></span>|
|<span data-ttu-id="86ae0-192">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="86ae0-192">scheduledInstallDays</span></span>|<span data-ttu-id="86ae0-193">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86ae0-193">[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md) collection</span></span>|<span data-ttu-id="86ae0-194">配置为使用时段所对应的一周的某一天。</span><span class="sxs-lookup"><span data-stu-id="86ae0-194">Days in week for which active hours are configured.</span></span> <span data-ttu-id="86ae0-195">该集合最多可包含 7 个元素。</span><span class="sxs-lookup"><span data-stu-id="86ae0-195">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="86ae0-196">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="86ae0-196">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="86ae0-197">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="86ae0-197">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="86ae0-198">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae0-198">Int32</span></span>|<span data-ttu-id="86ae0-199">UTC 时间偏移，用分钟表示</span><span class="sxs-lookup"><span data-stu-id="86ae0-199">UTC Time Offset indicated in minutes</span></span>|
|<span data-ttu-id="86ae0-200">enforcedSoftwareUpdateDelayInDays</span><span class="sxs-lookup"><span data-stu-id="86ae0-200">enforcedSoftwareUpdateDelayInDays</span></span>|<span data-ttu-id="86ae0-201">Int32</span><span class="sxs-lookup"><span data-stu-id="86ae0-201">Int32</span></span>|<span data-ttu-id="86ae0-202">软件更新对 iOS 设备可见的天数，范围从 0 到 90（含这两者）</span><span class="sxs-lookup"><span data-stu-id="86ae0-202">Days before software updates are visible to iOS devices ranging from 0 to 90 inclusive</span></span>|
|<span data-ttu-id="86ae0-203">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="86ae0-203">updateScheduleType</span></span>|[<span data-ttu-id="86ae0-204">iosSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="86ae0-204">iosSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-iossoftwareupdatescheduletype.md)|<span data-ttu-id="86ae0-205">更新计划类型。</span><span class="sxs-lookup"><span data-stu-id="86ae0-205">Update schedule type.</span></span> <span data-ttu-id="86ae0-206">可取值为：`updateOutsideOfActiveHours`、`alwaysUpdate`、`updateDuringTimeWindows`、`updateOutsideOfTimeWindows`。</span><span class="sxs-lookup"><span data-stu-id="86ae0-206">Possible values are: `updateOutsideOfActiveHours`, `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="86ae0-207">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="86ae0-207">customUpdateTimeWindows</span></span>|<span data-ttu-id="86ae0-208">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86ae0-208">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="86ae0-209">如果将更新计划类型设置为使用时间窗口计划，则自定义时间窗口将计划更新。</span><span class="sxs-lookup"><span data-stu-id="86ae0-209">If update schedule type is set to use time window scheduling, custom time windows when updates will be scheduled.</span></span> <span data-ttu-id="86ae0-210">此集合最多可包含 20 个元素。</span><span class="sxs-lookup"><span data-stu-id="86ae0-210">This collection can contain a maximum of 20 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="86ae0-211">响应</span><span class="sxs-lookup"><span data-stu-id="86ae0-211">Response</span></span>
<span data-ttu-id="86ae0-212">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86ae0-212">If successful, this method returns a `200 OK` response code and an updated [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ae0-213">示例</span><span class="sxs-lookup"><span data-stu-id="86ae0-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="86ae0-214">请求</span><span class="sxs-lookup"><span data-stu-id="86ae0-214">Request</span></span>
<span data-ttu-id="86ae0-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86ae0-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1596

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1,
  "updateScheduleType": "alwaysUpdate",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="86ae0-216">响应</span><span class="sxs-lookup"><span data-stu-id="86ae0-216">Response</span></span>
<span data-ttu-id="86ae0-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86ae0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1768

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
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
  "isEnabled": true,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "desiredOsVersion": "Desired Os Version value",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6,
  "enforcedSoftwareUpdateDelayInDays": 1,
  "updateScheduleType": "alwaysUpdate",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ]
}
```




