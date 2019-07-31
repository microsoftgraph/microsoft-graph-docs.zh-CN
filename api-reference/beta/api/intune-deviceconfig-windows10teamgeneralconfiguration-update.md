---
title: 更新 windows10TeamGeneralConfiguration
description: 更新 windows10TeamGeneralConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df6bed0790c9575f818a4ed84f5675de2cfa877f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975184"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="71b23-103">更新 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="71b23-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="71b23-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71b23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71b23-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71b23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71b23-106">更新 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71b23-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71b23-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="71b23-107">Prerequisites</span></span>
<span data-ttu-id="71b23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71b23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71b23-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="71b23-110">Permission type</span></span>|<span data-ttu-id="71b23-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71b23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71b23-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71b23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71b23-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71b23-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71b23-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71b23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71b23-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71b23-115">Not supported.</span></span>|
|<span data-ttu-id="71b23-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="71b23-116">Application</span></span>|<span data-ttu-id="71b23-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="71b23-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71b23-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71b23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="71b23-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="71b23-119">Request headers</span></span>
|<span data-ttu-id="71b23-120">标头</span><span class="sxs-lookup"><span data-stu-id="71b23-120">Header</span></span>|<span data-ttu-id="71b23-121">值</span><span class="sxs-lookup"><span data-stu-id="71b23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71b23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71b23-122">Authorization</span></span>|<span data-ttu-id="71b23-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71b23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71b23-124">接受</span><span class="sxs-lookup"><span data-stu-id="71b23-124">Accept</span></span>|<span data-ttu-id="71b23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71b23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71b23-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="71b23-126">Request body</span></span>
<span data-ttu-id="71b23-127">在请求正文中，提供 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71b23-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="71b23-128">下表显示了创建 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="71b23-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="71b23-129">属性</span><span class="sxs-lookup"><span data-stu-id="71b23-129">Property</span></span>|<span data-ttu-id="71b23-130">类型</span><span class="sxs-lookup"><span data-stu-id="71b23-130">Type</span></span>|<span data-ttu-id="71b23-131">说明</span><span class="sxs-lookup"><span data-stu-id="71b23-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71b23-132">id</span><span class="sxs-lookup"><span data-stu-id="71b23-132">id</span></span>|<span data-ttu-id="71b23-133">字符串</span><span class="sxs-lookup"><span data-stu-id="71b23-133">String</span></span>|<span data-ttu-id="71b23-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="71b23-134">Key of the entity.</span></span> <span data-ttu-id="71b23-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71b23-136">lastModifiedDateTime</span></span>|<span data-ttu-id="71b23-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71b23-137">DateTimeOffset</span></span>|<span data-ttu-id="71b23-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="71b23-138">DateTime the object was last modified.</span></span> <span data-ttu-id="71b23-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71b23-140">roleScopeTagIds</span></span>|<span data-ttu-id="71b23-141">String collection</span><span class="sxs-lookup"><span data-stu-id="71b23-141">String collection</span></span>|<span data-ttu-id="71b23-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="71b23-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71b23-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="71b23-144">supportsScopeTags</span></span>|<span data-ttu-id="71b23-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-145">Boolean</span></span>|<span data-ttu-id="71b23-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="71b23-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71b23-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="71b23-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71b23-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="71b23-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71b23-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="71b23-149">This property is read-only.</span></span> <span data-ttu-id="71b23-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71b23-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="71b23-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71b23-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="71b23-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="71b23-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="71b23-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71b23-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="71b23-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71b23-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="71b23-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="71b23-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="71b23-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71b23-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="71b23-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71b23-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="71b23-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="71b23-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="71b23-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71b23-163">createdDateTime</span></span>|<span data-ttu-id="71b23-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71b23-164">DateTimeOffset</span></span>|<span data-ttu-id="71b23-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="71b23-165">DateTime the object was created.</span></span> <span data-ttu-id="71b23-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-167">说明</span><span class="sxs-lookup"><span data-stu-id="71b23-167">description</span></span>|<span data-ttu-id="71b23-168">String</span><span class="sxs-lookup"><span data-stu-id="71b23-168">String</span></span>|<span data-ttu-id="71b23-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="71b23-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71b23-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-171">displayName</span><span class="sxs-lookup"><span data-stu-id="71b23-171">displayName</span></span>|<span data-ttu-id="71b23-172">字符串</span><span class="sxs-lookup"><span data-stu-id="71b23-172">String</span></span>|<span data-ttu-id="71b23-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="71b23-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71b23-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-175">version</span><span class="sxs-lookup"><span data-stu-id="71b23-175">version</span></span>|<span data-ttu-id="71b23-176">Int32</span><span class="sxs-lookup"><span data-stu-id="71b23-176">Int32</span></span>|<span data-ttu-id="71b23-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="71b23-177">Version of the device configuration.</span></span> <span data-ttu-id="71b23-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71b23-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71b23-179">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="71b23-179">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="71b23-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-180">Boolean</span></span>|<span data-ttu-id="71b23-181">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="71b23-181">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="71b23-182">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="71b23-182">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="71b23-183">String</span><span class="sxs-lookup"><span data-stu-id="71b23-183">String</span></span>|<span data-ttu-id="71b23-184">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="71b23-184">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="71b23-185">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="71b23-185">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="71b23-186">String</span><span class="sxs-lookup"><span data-stu-id="71b23-186">String</span></span>|<span data-ttu-id="71b23-187">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="71b23-187">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="71b23-188">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="71b23-188">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="71b23-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-189">Boolean</span></span>|<span data-ttu-id="71b23-190">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="71b23-190">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="71b23-191">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="71b23-191">maintenanceWindowBlocked</span></span>|<span data-ttu-id="71b23-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-192">Boolean</span></span>|<span data-ttu-id="71b23-193">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="71b23-193">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="71b23-194">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="71b23-194">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="71b23-195">Int32</span><span class="sxs-lookup"><span data-stu-id="71b23-195">Int32</span></span>|<span data-ttu-id="71b23-196">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="71b23-196">Maintenance window duration for device updates.</span></span> <span data-ttu-id="71b23-197">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="71b23-197">Valid values 0 to 5</span></span>|
|<span data-ttu-id="71b23-198">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="71b23-198">maintenanceWindowStartTime</span></span>|<span data-ttu-id="71b23-199">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="71b23-199">TimeOfDay</span></span>|<span data-ttu-id="71b23-200">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="71b23-200">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="71b23-201">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="71b23-201">miracastChannel</span></span>|[<span data-ttu-id="71b23-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="71b23-202">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="71b23-203">频道。</span><span class="sxs-lookup"><span data-stu-id="71b23-203">The channel.</span></span> <span data-ttu-id="71b23-204">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="71b23-204">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="71b23-205">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="71b23-205">miracastBlocked</span></span>|<span data-ttu-id="71b23-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-206">Boolean</span></span>|<span data-ttu-id="71b23-207">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="71b23-207">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="71b23-208">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="71b23-208">miracastRequirePin</span></span>|<span data-ttu-id="71b23-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-209">Boolean</span></span>|<span data-ttu-id="71b23-210">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="71b23-210">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="71b23-211">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="71b23-211">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="71b23-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-212">Boolean</span></span>|<span data-ttu-id="71b23-213">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="71b23-213">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="71b23-214">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="71b23-214">settingsBlockSessionResume</span></span>|<span data-ttu-id="71b23-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-215">Boolean</span></span>|<span data-ttu-id="71b23-216">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="71b23-216">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="71b23-217">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="71b23-217">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="71b23-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-218">Boolean</span></span>|<span data-ttu-id="71b23-219">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="71b23-219">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="71b23-220">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="71b23-220">settingsDefaultVolume</span></span>|<span data-ttu-id="71b23-221">Int32</span><span class="sxs-lookup"><span data-stu-id="71b23-221">Int32</span></span>|<span data-ttu-id="71b23-222">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="71b23-222">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="71b23-223">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="71b23-223">Permitted values are 0-100.</span></span> <span data-ttu-id="71b23-224">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="71b23-224">The default is 45.</span></span> <span data-ttu-id="71b23-225">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="71b23-225">Valid values 0 to 100</span></span>|
|<span data-ttu-id="71b23-226">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="71b23-226">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="71b23-227">Int32</span><span class="sxs-lookup"><span data-stu-id="71b23-227">Int32</span></span>|<span data-ttu-id="71b23-228">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="71b23-228">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="71b23-229">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="71b23-229">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="71b23-230">Int32</span><span class="sxs-lookup"><span data-stu-id="71b23-230">Int32</span></span>|<span data-ttu-id="71b23-231">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="71b23-231">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="71b23-232">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="71b23-232">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="71b23-233">Int32</span><span class="sxs-lookup"><span data-stu-id="71b23-233">Int32</span></span>|<span data-ttu-id="71b23-234">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="71b23-234">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="71b23-235">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="71b23-235">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="71b23-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="71b23-236">Boolean</span></span>|<span data-ttu-id="71b23-237">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="71b23-237">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="71b23-238">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="71b23-238">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="71b23-239">String</span><span class="sxs-lookup"><span data-stu-id="71b23-239">String</span></span>|<span data-ttu-id="71b23-240">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="71b23-240">The welcome screen background image URL.</span></span> <span data-ttu-id="71b23-241">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="71b23-241">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="71b23-242">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="71b23-242">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="71b23-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="71b23-243">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="71b23-244">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="71b23-244">The welcome screen meeting information shown.</span></span> <span data-ttu-id="71b23-245">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="71b23-245">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="71b23-246">响应</span><span class="sxs-lookup"><span data-stu-id="71b23-246">Response</span></span>
<span data-ttu-id="71b23-247">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71b23-247">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71b23-248">示例</span><span class="sxs-lookup"><span data-stu-id="71b23-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="71b23-249">请求</span><span class="sxs-lookup"><span data-stu-id="71b23-249">Request</span></span>
<span data-ttu-id="71b23-250">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71b23-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2015

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="71b23-251">响应</span><span class="sxs-lookup"><span data-stu-id="71b23-251">Response</span></span>
<span data-ttu-id="71b23-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71b23-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2187

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
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
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```





