---
title: 创建 windows10TeamGeneralConfiguration
description: 创建新的 windows10TeamGeneralConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f1250a152435ff48bf84f34c953f78abb8b9f8c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42477887"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="c5a48-103">创建 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5a48-103">Create windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="c5a48-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c5a48-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5a48-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5a48-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5a48-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5a48-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a48-107">创建新的 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5a48-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5a48-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c5a48-108">Prerequisites</span></span>
<span data-ttu-id="c5a48-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a48-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5a48-111">Permission type</span></span>|<span data-ttu-id="c5a48-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c5a48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a48-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5a48-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a48-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c5a48-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5a48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a48-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5a48-116">Not supported.</span></span>|
|<span data-ttu-id="c5a48-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5a48-117">Application</span></span>|<span data-ttu-id="c5a48-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a48-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a48-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5a48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c5a48-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5a48-120">Request headers</span></span>
|<span data-ttu-id="c5a48-121">标头</span><span class="sxs-lookup"><span data-stu-id="c5a48-121">Header</span></span>|<span data-ttu-id="c5a48-122">值</span><span class="sxs-lookup"><span data-stu-id="c5a48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5a48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5a48-123">Authorization</span></span>|<span data-ttu-id="c5a48-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c5a48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5a48-125">接受</span><span class="sxs-lookup"><span data-stu-id="c5a48-125">Accept</span></span>|<span data-ttu-id="c5a48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a48-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5a48-127">Request body</span></span>
<span data-ttu-id="c5a48-128">在请求正文中，提供 windows10TeamGeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5a48-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="c5a48-129">下表显示了创建 windows10TeamGeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c5a48-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="c5a48-130">属性</span><span class="sxs-lookup"><span data-stu-id="c5a48-130">Property</span></span>|<span data-ttu-id="c5a48-131">类型</span><span class="sxs-lookup"><span data-stu-id="c5a48-131">Type</span></span>|<span data-ttu-id="c5a48-132">说明</span><span class="sxs-lookup"><span data-stu-id="c5a48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a48-133">id</span><span class="sxs-lookup"><span data-stu-id="c5a48-133">id</span></span>|<span data-ttu-id="c5a48-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c5a48-134">String</span></span>|<span data-ttu-id="c5a48-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c5a48-135">Key of the entity.</span></span> <span data-ttu-id="c5a48-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a48-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c5a48-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a48-138">DateTimeOffset</span></span>|<span data-ttu-id="c5a48-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5a48-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c5a48-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c5a48-141">roleScopeTagIds</span></span>|<span data-ttu-id="c5a48-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="c5a48-142">String collection</span></span>|<span data-ttu-id="c5a48-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c5a48-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c5a48-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c5a48-145">supportsScopeTags</span></span>|<span data-ttu-id="c5a48-146">布尔</span><span class="sxs-lookup"><span data-stu-id="c5a48-146">Boolean</span></span>|<span data-ttu-id="c5a48-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c5a48-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c5a48-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c5a48-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c5a48-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c5a48-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c5a48-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c5a48-150">This property is read-only.</span></span> <span data-ttu-id="c5a48-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c5a48-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c5a48-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c5a48-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c5a48-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="c5a48-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c5a48-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c5a48-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c5a48-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c5a48-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c5a48-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c5a48-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c5a48-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c5a48-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c5a48-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c5a48-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c5a48-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="c5a48-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c5a48-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a48-164">createdDateTime</span></span>|<span data-ttu-id="c5a48-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a48-165">DateTimeOffset</span></span>|<span data-ttu-id="c5a48-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c5a48-166">DateTime the object was created.</span></span> <span data-ttu-id="c5a48-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-168">说明</span><span class="sxs-lookup"><span data-stu-id="c5a48-168">description</span></span>|<span data-ttu-id="c5a48-169">String</span><span class="sxs-lookup"><span data-stu-id="c5a48-169">String</span></span>|<span data-ttu-id="c5a48-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c5a48-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c5a48-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c5a48-172">displayName</span></span>|<span data-ttu-id="c5a48-173">字符串</span><span class="sxs-lookup"><span data-stu-id="c5a48-173">String</span></span>|<span data-ttu-id="c5a48-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c5a48-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c5a48-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-176">version</span><span class="sxs-lookup"><span data-stu-id="c5a48-176">version</span></span>|<span data-ttu-id="c5a48-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a48-177">Int32</span></span>|<span data-ttu-id="c5a48-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c5a48-178">Version of the device configuration.</span></span> <span data-ttu-id="c5a48-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c5a48-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c5a48-180">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="c5a48-180">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="c5a48-181">布尔</span><span class="sxs-lookup"><span data-stu-id="c5a48-181">Boolean</span></span>|<span data-ttu-id="c5a48-182">指示是否阻止 Azure 操作见解。</span><span class="sxs-lookup"><span data-stu-id="c5a48-182">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="c5a48-183">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="c5a48-183">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="c5a48-184">String</span><span class="sxs-lookup"><span data-stu-id="c5a48-184">String</span></span>|<span data-ttu-id="c5a48-185">Azure 操作见解工作区 ID。</span><span class="sxs-lookup"><span data-stu-id="c5a48-185">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="c5a48-186">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="c5a48-186">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="c5a48-187">String</span><span class="sxs-lookup"><span data-stu-id="c5a48-187">String</span></span>|<span data-ttu-id="c5a48-188">Azure 操作见解工作区键。</span><span class="sxs-lookup"><span data-stu-id="c5a48-188">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="c5a48-189">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="c5a48-189">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="c5a48-190">布尔</span><span class="sxs-lookup"><span data-stu-id="c5a48-190">Boolean</span></span>|<span data-ttu-id="c5a48-191">指定是否在启动投影时自动启动 Connect 应用。</span><span class="sxs-lookup"><span data-stu-id="c5a48-191">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="c5a48-192">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="c5a48-192">maintenanceWindowBlocked</span></span>|<span data-ttu-id="c5a48-193">布尔</span><span class="sxs-lookup"><span data-stu-id="c5a48-193">Boolean</span></span>|<span data-ttu-id="c5a48-194">指示是否阻止设置设备更新的维护时段。</span><span class="sxs-lookup"><span data-stu-id="c5a48-194">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="c5a48-195">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="c5a48-195">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="c5a48-196">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a48-196">Int32</span></span>|<span data-ttu-id="c5a48-197">设备更新的维护时段持续时间。</span><span class="sxs-lookup"><span data-stu-id="c5a48-197">Maintenance window duration for device updates.</span></span> <span data-ttu-id="c5a48-198">有效值为 0 至 5</span><span class="sxs-lookup"><span data-stu-id="c5a48-198">Valid values 0 to 5</span></span>|
|<span data-ttu-id="c5a48-199">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="c5a48-199">maintenanceWindowStartTime</span></span>|<span data-ttu-id="c5a48-200">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c5a48-200">TimeOfDay</span></span>|<span data-ttu-id="c5a48-201">设备更新的维护时段开始时间。</span><span class="sxs-lookup"><span data-stu-id="c5a48-201">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="c5a48-202">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="c5a48-202">miracastChannel</span></span>|[<span data-ttu-id="c5a48-203">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="c5a48-203">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="c5a48-204">频道。</span><span class="sxs-lookup"><span data-stu-id="c5a48-204">The channel.</span></span> <span data-ttu-id="c5a48-205">可取值为：`userDefined`、`one`、`two`、`three`、`four`、`five`、`six`、`seven`、`eight`、`nine`、`ten`、`eleven`、`thirtySix`、`forty`、`fortyFour`、`fortyEight`、`oneHundredFortyNine`、`oneHundredFiftyThree`、`oneHundredFiftySeven`、`oneHundredSixtyOne`、`oneHundredSixtyFive`。</span><span class="sxs-lookup"><span data-stu-id="c5a48-205">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="c5a48-206">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="c5a48-206">miracastBlocked</span></span>|<span data-ttu-id="c5a48-207">布尔</span><span class="sxs-lookup"><span data-stu-id="c5a48-207">Boolean</span></span>|<span data-ttu-id="c5a48-208">指示是否阻止无线投影。</span><span class="sxs-lookup"><span data-stu-id="c5a48-208">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="c5a48-209">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="c5a48-209">miracastRequirePin</span></span>|<span data-ttu-id="c5a48-210">布尔</span><span class="sxs-lookup"><span data-stu-id="c5a48-210">Boolean</span></span>|<span data-ttu-id="c5a48-211">指示是否需要 PIN 才能进行无线投影。</span><span class="sxs-lookup"><span data-stu-id="c5a48-211">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="c5a48-212">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="c5a48-212">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="c5a48-213">布尔</span><span class="sxs-lookup"><span data-stu-id="c5a48-213">Boolean</span></span>|<span data-ttu-id="c5a48-214">指定是否禁用“开始”菜单中的“我的会议和文件”功能，该功能显示来自 Office 365 的已登录用户的会议和文件。</span><span class="sxs-lookup"><span data-stu-id="c5a48-214">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="c5a48-215">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="c5a48-215">settingsBlockSessionResume</span></span>|<span data-ttu-id="c5a48-216">布尔</span><span class="sxs-lookup"><span data-stu-id="c5a48-216">Boolean</span></span>|<span data-ttu-id="c5a48-217">指定是否允许在会话超时时恢复会话。</span><span class="sxs-lookup"><span data-stu-id="c5a48-217">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="c5a48-218">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="c5a48-218">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="c5a48-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a48-219">Boolean</span></span>|<span data-ttu-id="c5a48-220">指定是否禁用计划会议的被邀请者自动填充登录对话框。</span><span class="sxs-lookup"><span data-stu-id="c5a48-220">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="c5a48-221">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="c5a48-221">settingsDefaultVolume</span></span>|<span data-ttu-id="c5a48-222">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a48-222">Int32</span></span>|<span data-ttu-id="c5a48-223">指定新会话的默认音量值。</span><span class="sxs-lookup"><span data-stu-id="c5a48-223">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="c5a48-224">允许的值为 0-100。</span><span class="sxs-lookup"><span data-stu-id="c5a48-224">Permitted values are 0-100.</span></span> <span data-ttu-id="c5a48-225">默认值为 45。</span><span class="sxs-lookup"><span data-stu-id="c5a48-225">The default is 45.</span></span> <span data-ttu-id="c5a48-226">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="c5a48-226">Valid values 0 to 100</span></span>|
|<span data-ttu-id="c5a48-227">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c5a48-227">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="c5a48-228">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a48-228">Int32</span></span>|<span data-ttu-id="c5a48-229">指定 Hub 屏幕关闭前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c5a48-229">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="c5a48-230">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c5a48-230">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="c5a48-231">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a48-231">Int32</span></span>|<span data-ttu-id="c5a48-232">指定会话超时前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c5a48-232">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="c5a48-233">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c5a48-233">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="c5a48-234">Int32</span><span class="sxs-lookup"><span data-stu-id="c5a48-234">Int32</span></span>|<span data-ttu-id="c5a48-235">指定 Hub 进入睡眠模式前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c5a48-235">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="c5a48-236">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="c5a48-236">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="c5a48-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5a48-237">Boolean</span></span>|<span data-ttu-id="c5a48-238">指示当某人进入会议室时是否阻止欢迎屏幕自动唤醒。</span><span class="sxs-lookup"><span data-stu-id="c5a48-238">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="c5a48-239">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="c5a48-239">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="c5a48-240">String</span><span class="sxs-lookup"><span data-stu-id="c5a48-240">String</span></span>|<span data-ttu-id="c5a48-241">欢迎屏幕背景图像 URL。</span><span class="sxs-lookup"><span data-stu-id="c5a48-241">The welcome screen background image URL.</span></span> <span data-ttu-id="c5a48-242">URL 必须使用 HTTPS 协议并返回 PNG 图像。</span><span class="sxs-lookup"><span data-stu-id="c5a48-242">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="c5a48-243">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="c5a48-243">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="c5a48-244">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="c5a48-244">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="c5a48-245">显示的欢迎屏幕会议信息。</span><span class="sxs-lookup"><span data-stu-id="c5a48-245">The welcome screen meeting information shown.</span></span> <span data-ttu-id="c5a48-246">可取值为：`userDefined`、`showOrganizerAndTimeOnly`、`showOrganizerAndTimeAndSubject`。</span><span class="sxs-lookup"><span data-stu-id="c5a48-246">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="c5a48-247">响应</span><span class="sxs-lookup"><span data-stu-id="c5a48-247">Response</span></span>
<span data-ttu-id="c5a48-248">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5a48-248">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5a48-249">示例</span><span class="sxs-lookup"><span data-stu-id="c5a48-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5a48-250">请求</span><span class="sxs-lookup"><span data-stu-id="c5a48-250">Request</span></span>
<span data-ttu-id="c5a48-251">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5a48-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c5a48-252">响应</span><span class="sxs-lookup"><span data-stu-id="c5a48-252">Response</span></span>
<span data-ttu-id="c5a48-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5a48-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





