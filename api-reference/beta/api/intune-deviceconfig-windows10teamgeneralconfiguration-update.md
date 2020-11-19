---
title: 更新 windows10TeamGeneralConfiguration
description: 更新 windows10TeamGeneralConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6ac5b6c1d327620297f0cb2f1a1d8d3aefc0eec3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49204731"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="afcbe-103">更新 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="afcbe-103">Update windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="afcbe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afcbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afcbe-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="afcbe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afcbe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afcbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afcbe-107">更新 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="afcbe-107">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afcbe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="afcbe-108">Prerequisites</span></span>
<span data-ttu-id="afcbe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afcbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afcbe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="afcbe-111">Permission type</span></span>|<span data-ttu-id="afcbe-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="afcbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afcbe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afcbe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afcbe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afcbe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afcbe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afcbe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afcbe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="afcbe-116">Not supported.</span></span>|
|<span data-ttu-id="afcbe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="afcbe-117">Application</span></span>|<span data-ttu-id="afcbe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afcbe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afcbe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afcbe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="afcbe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="afcbe-120">Request headers</span></span>
|<span data-ttu-id="afcbe-121">标头</span><span class="sxs-lookup"><span data-stu-id="afcbe-121">Header</span></span>|<span data-ttu-id="afcbe-122">值</span><span class="sxs-lookup"><span data-stu-id="afcbe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afcbe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afcbe-123">Authorization</span></span>|<span data-ttu-id="afcbe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="afcbe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afcbe-125">接受</span><span class="sxs-lookup"><span data-stu-id="afcbe-125">Accept</span></span>|<span data-ttu-id="afcbe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afcbe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afcbe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="afcbe-127">Request body</span></span>
<span data-ttu-id="afcbe-128">在请求正文中，提供 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afcbe-128">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="afcbe-129">下表显示了创建 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="afcbe-129">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="afcbe-130">属性</span><span class="sxs-lookup"><span data-stu-id="afcbe-130">Property</span></span>|<span data-ttu-id="afcbe-131">类型</span><span class="sxs-lookup"><span data-stu-id="afcbe-131">Type</span></span>|<span data-ttu-id="afcbe-132">说明</span><span class="sxs-lookup"><span data-stu-id="afcbe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afcbe-133">id</span><span class="sxs-lookup"><span data-stu-id="afcbe-133">id</span></span>|<span data-ttu-id="afcbe-134">String</span><span class="sxs-lookup"><span data-stu-id="afcbe-134">String</span></span>|<span data-ttu-id="afcbe-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="afcbe-135">Key of the entity.</span></span> <span data-ttu-id="afcbe-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afcbe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="afcbe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afcbe-138">DateTimeOffset</span></span>|<span data-ttu-id="afcbe-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="afcbe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="afcbe-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="afcbe-141">roleScopeTagIds</span></span>|<span data-ttu-id="afcbe-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="afcbe-142">String collection</span></span>|<span data-ttu-id="afcbe-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="afcbe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="afcbe-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="afcbe-145">supportsScopeTags</span></span>|<span data-ttu-id="afcbe-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-146">Boolean</span></span>|<span data-ttu-id="afcbe-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="afcbe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="afcbe-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="afcbe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="afcbe-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="afcbe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="afcbe-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="afcbe-150">This property is read-only.</span></span> <span data-ttu-id="afcbe-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="afcbe-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="afcbe-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="afcbe-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="afcbe-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="afcbe-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="afcbe-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="afcbe-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="afcbe-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="afcbe-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="afcbe-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="afcbe-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="afcbe-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="afcbe-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="afcbe-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="afcbe-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="afcbe-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="afcbe-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="afcbe-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afcbe-164">createdDateTime</span></span>|<span data-ttu-id="afcbe-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afcbe-165">DateTimeOffset</span></span>|<span data-ttu-id="afcbe-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="afcbe-166">DateTime the object was created.</span></span> <span data-ttu-id="afcbe-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-168">description</span><span class="sxs-lookup"><span data-stu-id="afcbe-168">description</span></span>|<span data-ttu-id="afcbe-169">String</span><span class="sxs-lookup"><span data-stu-id="afcbe-169">String</span></span>|<span data-ttu-id="afcbe-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="afcbe-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="afcbe-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-172">displayName</span><span class="sxs-lookup"><span data-stu-id="afcbe-172">displayName</span></span>|<span data-ttu-id="afcbe-173">String</span><span class="sxs-lookup"><span data-stu-id="afcbe-173">String</span></span>|<span data-ttu-id="afcbe-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="afcbe-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="afcbe-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-176">version</span><span class="sxs-lookup"><span data-stu-id="afcbe-176">version</span></span>|<span data-ttu-id="afcbe-177">Int32</span><span class="sxs-lookup"><span data-stu-id="afcbe-177">Int32</span></span>|<span data-ttu-id="afcbe-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="afcbe-178">Version of the device configuration.</span></span> <span data-ttu-id="afcbe-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afcbe-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afcbe-180">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="afcbe-180">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="afcbe-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-181">Boolean</span></span>|<span data-ttu-id="afcbe-182">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="afcbe-182">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="afcbe-183">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="afcbe-183">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="afcbe-184">String</span><span class="sxs-lookup"><span data-stu-id="afcbe-184">String</span></span>|<span data-ttu-id="afcbe-185">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="afcbe-185">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="afcbe-186">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="afcbe-186">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="afcbe-187">String</span><span class="sxs-lookup"><span data-stu-id="afcbe-187">String</span></span>|<span data-ttu-id="afcbe-188">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="afcbe-188">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="afcbe-189">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="afcbe-189">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="afcbe-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-190">Boolean</span></span>|<span data-ttu-id="afcbe-191">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="afcbe-191">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="afcbe-192">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="afcbe-192">maintenanceWindowBlocked</span></span>|<span data-ttu-id="afcbe-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-193">Boolean</span></span>|<span data-ttu-id="afcbe-194">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="afcbe-194">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="afcbe-195">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="afcbe-195">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="afcbe-196">Int32</span><span class="sxs-lookup"><span data-stu-id="afcbe-196">Int32</span></span>|<span data-ttu-id="afcbe-197">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="afcbe-197">Maintenance window duration for device updates.</span></span> <span data-ttu-id="afcbe-198">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="afcbe-198">Valid values 0 to 5</span></span>|
|<span data-ttu-id="afcbe-199">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="afcbe-199">maintenanceWindowStartTime</span></span>|<span data-ttu-id="afcbe-200">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="afcbe-200">TimeOfDay</span></span>|<span data-ttu-id="afcbe-201">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="afcbe-201">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="afcbe-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="afcbe-202">miracastChannel</span></span>|[<span data-ttu-id="afcbe-203">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="afcbe-203">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="afcbe-204">频道。</span><span class="sxs-lookup"><span data-stu-id="afcbe-204">The channel.</span></span> <span data-ttu-id="afcbe-205">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="afcbe-205">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="afcbe-206">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="afcbe-206">miracastBlocked</span></span>|<span data-ttu-id="afcbe-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-207">Boolean</span></span>|<span data-ttu-id="afcbe-208">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="afcbe-208">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="afcbe-209">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="afcbe-209">miracastRequirePin</span></span>|<span data-ttu-id="afcbe-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-210">Boolean</span></span>|<span data-ttu-id="afcbe-211">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="afcbe-211">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="afcbe-212">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="afcbe-212">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="afcbe-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-213">Boolean</span></span>|<span data-ttu-id="afcbe-214">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="afcbe-214">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="afcbe-215">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="afcbe-215">settingsBlockSessionResume</span></span>|<span data-ttu-id="afcbe-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-216">Boolean</span></span>|<span data-ttu-id="afcbe-217">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="afcbe-217">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="afcbe-218">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="afcbe-218">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="afcbe-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-219">Boolean</span></span>|<span data-ttu-id="afcbe-220">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="afcbe-220">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="afcbe-221">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="afcbe-221">settingsDefaultVolume</span></span>|<span data-ttu-id="afcbe-222">Int32</span><span class="sxs-lookup"><span data-stu-id="afcbe-222">Int32</span></span>|<span data-ttu-id="afcbe-223">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="afcbe-223">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="afcbe-224">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="afcbe-224">Permitted values are 0-100.</span></span> <span data-ttu-id="afcbe-225">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="afcbe-225">The default is 45.</span></span> <span data-ttu-id="afcbe-226">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="afcbe-226">Valid values 0 to 100</span></span>|
|<span data-ttu-id="afcbe-227">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="afcbe-227">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="afcbe-228">Int32</span><span class="sxs-lookup"><span data-stu-id="afcbe-228">Int32</span></span>|<span data-ttu-id="afcbe-229">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="afcbe-229">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="afcbe-230">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="afcbe-230">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="afcbe-231">Int32</span><span class="sxs-lookup"><span data-stu-id="afcbe-231">Int32</span></span>|<span data-ttu-id="afcbe-232">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="afcbe-232">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="afcbe-233">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="afcbe-233">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="afcbe-234">Int32</span><span class="sxs-lookup"><span data-stu-id="afcbe-234">Int32</span></span>|<span data-ttu-id="afcbe-235">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="afcbe-235">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="afcbe-236">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="afcbe-236">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="afcbe-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="afcbe-237">Boolean</span></span>|<span data-ttu-id="afcbe-238">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="afcbe-238">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="afcbe-239">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="afcbe-239">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="afcbe-240">String</span><span class="sxs-lookup"><span data-stu-id="afcbe-240">String</span></span>|<span data-ttu-id="afcbe-241">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="afcbe-241">The welcome screen background image URL.</span></span> <span data-ttu-id="afcbe-242">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="afcbe-242">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="afcbe-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="afcbe-243">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="afcbe-244">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="afcbe-244">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="afcbe-245">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="afcbe-245">The welcome screen meeting information shown.</span></span> <span data-ttu-id="afcbe-246">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="afcbe-246">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="afcbe-247">响应</span><span class="sxs-lookup"><span data-stu-id="afcbe-247">Response</span></span>
<span data-ttu-id="afcbe-248">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afcbe-248">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afcbe-249">示例</span><span class="sxs-lookup"><span data-stu-id="afcbe-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="afcbe-250">请求</span><span class="sxs-lookup"><span data-stu-id="afcbe-250">Request</span></span>
<span data-ttu-id="afcbe-251">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afcbe-251">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="afcbe-252">响应</span><span class="sxs-lookup"><span data-stu-id="afcbe-252">Response</span></span>
<span data-ttu-id="afcbe-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afcbe-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




