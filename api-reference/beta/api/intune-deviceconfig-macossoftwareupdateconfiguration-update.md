---
title: 更新 macOSSoftwareUpdateConfiguration
description: 更新 macOSSoftwareUpdateConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1547500323d3f6c1039206c636e65d3946795d03
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137215"
---
# <a name="update-macossoftwareupdateconfiguration"></a><span data-ttu-id="f1ad9-103">更新 macOSSoftwareUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ad9-103">Update macOSSoftwareUpdateConfiguration</span></span>

<span data-ttu-id="f1ad9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1ad9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1ad9-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1ad9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1ad9-107">更新 [macOSSoftwareUpdateConfiguration 对象](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-107">Update the properties of a [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1ad9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f1ad9-108">Prerequisites</span></span>
<span data-ttu-id="f1ad9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ad9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1ad9-111">Permission type</span></span>|<span data-ttu-id="f1ad9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1ad9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1ad9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1ad9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1ad9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ad9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1ad9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1ad9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1ad9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-116">Not supported.</span></span>|
|<span data-ttu-id="f1ad9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1ad9-117">Application</span></span>|<span data-ttu-id="f1ad9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ad9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1ad9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1ad9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1ad9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1ad9-120">Request headers</span></span>
|<span data-ttu-id="f1ad9-121">标头</span><span class="sxs-lookup"><span data-stu-id="f1ad9-121">Header</span></span>|<span data-ttu-id="f1ad9-122">值</span><span class="sxs-lookup"><span data-stu-id="f1ad9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1ad9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1ad9-123">Authorization</span></span>|<span data-ttu-id="f1ad9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1ad9-125">接受</span><span class="sxs-lookup"><span data-stu-id="f1ad9-125">Accept</span></span>|<span data-ttu-id="f1ad9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1ad9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1ad9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1ad9-127">Request body</span></span>
<span data-ttu-id="f1ad9-128">在请求正文中，提供 [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-128">In the request body, supply a JSON representation for the [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object.</span></span>

<span data-ttu-id="f1ad9-129">下表显示创建 [macOSSoftwareUpdateConfiguration 时所需的属性](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-129">The following table shows the properties that are required when you create the [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md).</span></span>

|<span data-ttu-id="f1ad9-130">属性</span><span class="sxs-lookup"><span data-stu-id="f1ad9-130">Property</span></span>|<span data-ttu-id="f1ad9-131">类型</span><span class="sxs-lookup"><span data-stu-id="f1ad9-131">Type</span></span>|<span data-ttu-id="f1ad9-132">说明</span><span class="sxs-lookup"><span data-stu-id="f1ad9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1ad9-133">id</span><span class="sxs-lookup"><span data-stu-id="f1ad9-133">id</span></span>|<span data-ttu-id="f1ad9-134">String</span><span class="sxs-lookup"><span data-stu-id="f1ad9-134">String</span></span>|<span data-ttu-id="f1ad9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-135">Key of the entity.</span></span> <span data-ttu-id="f1ad9-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1ad9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f1ad9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1ad9-138">DateTimeOffset</span></span>|<span data-ttu-id="f1ad9-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f1ad9-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f1ad9-141">roleScopeTagIds</span></span>|<span data-ttu-id="f1ad9-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f1ad9-142">String collection</span></span>|<span data-ttu-id="f1ad9-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f1ad9-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f1ad9-145">supportsScopeTags</span></span>|<span data-ttu-id="f1ad9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1ad9-146">Boolean</span></span>|<span data-ttu-id="f1ad9-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f1ad9-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f1ad9-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f1ad9-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-150">This property is read-only.</span></span> <span data-ttu-id="f1ad9-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1ad9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f1ad9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f1ad9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f1ad9-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f1ad9-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1ad9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f1ad9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f1ad9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f1ad9-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f1ad9-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f1ad9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f1ad9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f1ad9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f1ad9-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f1ad9-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1ad9-164">createdDateTime</span></span>|<span data-ttu-id="f1ad9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1ad9-165">DateTimeOffset</span></span>|<span data-ttu-id="f1ad9-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-166">DateTime the object was created.</span></span> <span data-ttu-id="f1ad9-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-168">说明</span><span class="sxs-lookup"><span data-stu-id="f1ad9-168">description</span></span>|<span data-ttu-id="f1ad9-169">String</span><span class="sxs-lookup"><span data-stu-id="f1ad9-169">String</span></span>|<span data-ttu-id="f1ad9-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f1ad9-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f1ad9-172">displayName</span></span>|<span data-ttu-id="f1ad9-173">String</span><span class="sxs-lookup"><span data-stu-id="f1ad9-173">String</span></span>|<span data-ttu-id="f1ad9-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f1ad9-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-176">version</span><span class="sxs-lookup"><span data-stu-id="f1ad9-176">version</span></span>|<span data-ttu-id="f1ad9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f1ad9-177">Int32</span></span>|<span data-ttu-id="f1ad9-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-178">Version of the device configuration.</span></span> <span data-ttu-id="f1ad9-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f1ad9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f1ad9-180">criticalUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="f1ad9-180">criticalUpdateBehavior</span></span>|[<span data-ttu-id="f1ad9-181">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="f1ad9-181">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="f1ad9-182">关键更新的更新行为。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-182">Update behavior for critical updates.</span></span> <span data-ttu-id="f1ad9-183">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-183">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="f1ad9-184">configDataUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="f1ad9-184">configDataUpdateBehavior</span></span>|[<span data-ttu-id="f1ad9-185">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="f1ad9-185">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="f1ad9-186">配置文件更新的更新行为。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-186">Update behavior for configuration data file updates.</span></span> <span data-ttu-id="f1ad9-187">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-187">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="f1ad9-188">firmwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="f1ad9-188">firmwareUpdateBehavior</span></span>|[<span data-ttu-id="f1ad9-189">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="f1ad9-189">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="f1ad9-190">固件更新的更新行为。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-190">Update behavior for firmware updates.</span></span> <span data-ttu-id="f1ad9-191">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-191">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="f1ad9-192">allOtherUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="f1ad9-192">allOtherUpdateBehavior</span></span>|[<span data-ttu-id="f1ad9-193">macOSSoftwareUpdateBehavior</span><span class="sxs-lookup"><span data-stu-id="f1ad9-193">macOSSoftwareUpdateBehavior</span></span>](../resources/intune-deviceconfig-macossoftwareupdatebehavior.md)|<span data-ttu-id="f1ad9-194">所有其他更新的更新行为。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-194">Update behavior for all other updates.</span></span> <span data-ttu-id="f1ad9-195">可取值为：`notConfigured`、`default`。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-195">Possible values are: `notConfigured`, `default`.</span></span>|
|<span data-ttu-id="f1ad9-196">updateScheduleType</span><span class="sxs-lookup"><span data-stu-id="f1ad9-196">updateScheduleType</span></span>|[<span data-ttu-id="f1ad9-197">macOSSoftwareUpdateScheduleType</span><span class="sxs-lookup"><span data-stu-id="f1ad9-197">macOSSoftwareUpdateScheduleType</span></span>](../resources/intune-deviceconfig-macossoftwareupdatescheduletype.md)|<span data-ttu-id="f1ad9-198">更新计划类型。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-198">Update schedule type.</span></span> <span data-ttu-id="f1ad9-199">可取值为：`alwaysUpdate`、`updateDuringTimeWindows`、`updateOutsideOfTimeWindows`。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-199">Possible values are: `alwaysUpdate`, `updateDuringTimeWindows`, `updateOutsideOfTimeWindows`.</span></span>|
|<span data-ttu-id="f1ad9-200">customUpdateTimeWindows</span><span class="sxs-lookup"><span data-stu-id="f1ad9-200">customUpdateTimeWindows</span></span>|<span data-ttu-id="f1ad9-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1ad9-201">[customUpdateTimeWindow](../resources/intune-deviceconfig-customupdatetimewindow.md) collection</span></span>|<span data-ttu-id="f1ad9-202">允许或阻止更新的自定义时间窗口。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-202">Custom Time windows when updates will be allowed or blocked.</span></span> <span data-ttu-id="f1ad9-203">此集合最多可包含 20 个元素。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-203">This collection can contain a maximum of 20 elements.</span></span>|
|<span data-ttu-id="f1ad9-204">updateTimeWindowUtcOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="f1ad9-204">updateTimeWindowUtcOffsetInMinutes</span></span>|<span data-ttu-id="f1ad9-205">Int32</span><span class="sxs-lookup"><span data-stu-id="f1ad9-205">Int32</span></span>|<span data-ttu-id="f1ad9-206">指示每个更新时间窗口的 UTC 偏移的分钟数</span><span class="sxs-lookup"><span data-stu-id="f1ad9-206">Minutes indicating UTC offset for each update time window</span></span>|



## <a name="response"></a><span data-ttu-id="f1ad9-207">响应</span><span class="sxs-lookup"><span data-stu-id="f1ad9-207">Response</span></span>
<span data-ttu-id="f1ad9-208">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-208">If successful, this method returns a `200 OK` response code and an updated [macOSSoftwareUpdateConfiguration](../resources/intune-deviceconfig-macossoftwareupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1ad9-209">示例</span><span class="sxs-lookup"><span data-stu-id="f1ad9-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1ad9-210">请求</span><span class="sxs-lookup"><span data-stu-id="f1ad9-210">Request</span></span>
<span data-ttu-id="f1ad9-211">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1542

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```

### <a name="response"></a><span data-ttu-id="f1ad9-212">响应</span><span class="sxs-lookup"><span data-stu-id="f1ad9-212">Response</span></span>
<span data-ttu-id="f1ad9-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f1ad9-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1714

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateConfiguration",
  "id": "b8e467ac-67ac-b8e4-ac67-e4b8ac67e4b8",
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
  "criticalUpdateBehavior": "default",
  "configDataUpdateBehavior": "default",
  "firmwareUpdateBehavior": "default",
  "allOtherUpdateBehavior": "default",
  "updateScheduleType": "updateDuringTimeWindows",
  "customUpdateTimeWindows": [
    {
      "@odata.type": "microsoft.graph.customUpdateTimeWindow",
      "startDay": "monday",
      "endDay": "monday",
      "startTime": "12:03:30.2730000",
      "endTime": "12:03:02.3740000"
    }
  ],
  "updateTimeWindowUtcOffsetInMinutes": 2
}
```




