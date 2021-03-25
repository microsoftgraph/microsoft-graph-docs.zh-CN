---
title: 更新 windowsDeliveryOptimizationConfiguration
description: 更新 windowsDeliveryOptimizationConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97a9cdb898d60d2945dc71de888ec123f0c2c64b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154922"
---
# <a name="update-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="f7258-103">更新 windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7258-103">Update windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="f7258-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7258-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7258-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7258-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7258-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7258-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7258-107">更新 [windowsDeliveryOptimizationConfiguration 对象](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f7258-107">Update the properties of a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7258-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7258-108">Prerequisites</span></span>
<span data-ttu-id="f7258-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7258-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7258-111">Permission type</span></span>|<span data-ttu-id="f7258-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7258-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7258-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7258-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7258-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7258-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7258-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7258-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7258-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7258-116">Not supported.</span></span>|
|<span data-ttu-id="f7258-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7258-117">Application</span></span>|<span data-ttu-id="f7258-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7258-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7258-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7258-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f7258-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7258-120">Request headers</span></span>
|<span data-ttu-id="f7258-121">标头</span><span class="sxs-lookup"><span data-stu-id="f7258-121">Header</span></span>|<span data-ttu-id="f7258-122">值</span><span class="sxs-lookup"><span data-stu-id="f7258-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7258-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7258-123">Authorization</span></span>|<span data-ttu-id="f7258-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7258-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7258-125">接受</span><span class="sxs-lookup"><span data-stu-id="f7258-125">Accept</span></span>|<span data-ttu-id="f7258-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7258-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7258-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7258-127">Request body</span></span>
<span data-ttu-id="f7258-128">在请求正文中，提供 [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7258-128">In the request body, supply a JSON representation for the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

<span data-ttu-id="f7258-129">下表显示创建 [windowsDeliveryOptimizationConfiguration 时所需的属性](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="f7258-129">The following table shows the properties that are required when you create the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

|<span data-ttu-id="f7258-130">属性</span><span class="sxs-lookup"><span data-stu-id="f7258-130">Property</span></span>|<span data-ttu-id="f7258-131">类型</span><span class="sxs-lookup"><span data-stu-id="f7258-131">Type</span></span>|<span data-ttu-id="f7258-132">说明</span><span class="sxs-lookup"><span data-stu-id="f7258-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7258-133">id</span><span class="sxs-lookup"><span data-stu-id="f7258-133">id</span></span>|<span data-ttu-id="f7258-134">String</span><span class="sxs-lookup"><span data-stu-id="f7258-134">String</span></span>|<span data-ttu-id="f7258-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f7258-135">Key of the entity.</span></span> <span data-ttu-id="f7258-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7258-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f7258-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7258-138">DateTimeOffset</span></span>|<span data-ttu-id="f7258-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f7258-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f7258-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f7258-141">roleScopeTagIds</span></span>|<span data-ttu-id="f7258-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f7258-142">String collection</span></span>|<span data-ttu-id="f7258-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f7258-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f7258-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f7258-145">supportsScopeTags</span></span>|<span data-ttu-id="f7258-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7258-146">Boolean</span></span>|<span data-ttu-id="f7258-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="f7258-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f7258-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="f7258-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f7258-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="f7258-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f7258-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f7258-150">This property is read-only.</span></span> <span data-ttu-id="f7258-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f7258-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f7258-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f7258-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f7258-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="f7258-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f7258-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f7258-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f7258-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f7258-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f7258-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f7258-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f7258-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f7258-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f7258-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f7258-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f7258-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f7258-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f7258-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7258-164">createdDateTime</span></span>|<span data-ttu-id="f7258-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7258-165">DateTimeOffset</span></span>|<span data-ttu-id="f7258-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f7258-166">DateTime the object was created.</span></span> <span data-ttu-id="f7258-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-168">说明</span><span class="sxs-lookup"><span data-stu-id="f7258-168">description</span></span>|<span data-ttu-id="f7258-169">String</span><span class="sxs-lookup"><span data-stu-id="f7258-169">String</span></span>|<span data-ttu-id="f7258-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f7258-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f7258-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f7258-172">displayName</span></span>|<span data-ttu-id="f7258-173">String</span><span class="sxs-lookup"><span data-stu-id="f7258-173">String</span></span>|<span data-ttu-id="f7258-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f7258-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f7258-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-176">version</span><span class="sxs-lookup"><span data-stu-id="f7258-176">version</span></span>|<span data-ttu-id="f7258-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f7258-177">Int32</span></span>|<span data-ttu-id="f7258-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f7258-178">Version of the device configuration.</span></span> <span data-ttu-id="f7258-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7258-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7258-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f7258-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="f7258-181">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f7258-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="f7258-182">指定传递优化可用于管理大型内容分发方案的网络带宽消耗的下载方法。</span><span class="sxs-lookup"><span data-stu-id="f7258-182">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="f7258-183">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="f7258-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="f7258-184">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="f7258-184">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="f7258-185">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="f7258-185">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="f7258-186">指定通过所选选项限制对等选择。</span><span class="sxs-lookup"><span data-stu-id="f7258-186">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="f7258-187">选项 1 (子网掩码) 仅适用于传递优化模式下载模式 LAN (1) 和组 (2) 。</span><span class="sxs-lookup"><span data-stu-id="f7258-187">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="f7258-188">可取值为：`notConfigured`、`subnetMask`。</span><span class="sxs-lookup"><span data-stu-id="f7258-188">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="f7258-189">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="f7258-189">groupIdSource</span></span>|[<span data-ttu-id="f7258-190">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="f7258-190">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="f7258-191">指定将对等选择限制到特定源。</span><span class="sxs-lookup"><span data-stu-id="f7258-191">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="f7258-192">此策略中设置的选项仅适用于"传递优化"模式组 (2) 下载模式。</span><span class="sxs-lookup"><span data-stu-id="f7258-192">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="f7258-193">如果组 (2) 未设置为下载模式，此策略将被忽略。</span><span class="sxs-lookup"><span data-stu-id="f7258-193">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="f7258-194">对于选项 3 - DHCP 选项 ID，客户端将查询 DHCP 选项 ID 234，并使用返回的 GUID 值作为组 ID。</span><span class="sxs-lookup"><span data-stu-id="f7258-194">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="f7258-195">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="f7258-195">bandwidthMode</span></span>|[<span data-ttu-id="f7258-196">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="f7258-196">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="f7258-197">使用百分比、绝对值或小时指定前台和后台带宽使用量。</span><span class="sxs-lookup"><span data-stu-id="f7258-197">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="f7258-198">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="f7258-198">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="f7258-199">Int64</span><span class="sxs-lookup"><span data-stu-id="f7258-199">Int64</span></span>|<span data-ttu-id="f7258-200">指定在后台下载中延迟允许使用对等的 HTTP 源的秒数。</span><span class="sxs-lookup"><span data-stu-id="f7258-200">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="f7258-201">有效值为 0 到 4294967295</span><span class="sxs-lookup"><span data-stu-id="f7258-201">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="f7258-202">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="f7258-202">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="f7258-203">Int64</span><span class="sxs-lookup"><span data-stu-id="f7258-203">Int64</span></span>|<span data-ttu-id="f7258-204">指定延迟前台下载中允许使用对等 (0-86400) 的 HTTP 源的秒数。</span><span class="sxs-lookup"><span data-stu-id="f7258-204">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="f7258-205">有效值为 0 到 86400</span><span class="sxs-lookup"><span data-stu-id="f7258-205">Valid values 0 to 86400</span></span>
<span data-ttu-id="f7258-206">指定 0 将设置传递优化以使用云服务管理此设置。</span><span class="sxs-lookup"><span data-stu-id="f7258-206">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="f7258-207">有效值为 0 到 86400</span><span class="sxs-lookup"><span data-stu-id="f7258-207">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="f7258-208">minimumRamAllowedToPeerInGtesbytes</span><span class="sxs-lookup"><span data-stu-id="f7258-208">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="f7258-209">Int32</span><span class="sxs-lookup"><span data-stu-id="f7258-209">Int32</span></span>|<span data-ttu-id="f7258-210">指定使用 1-100000 和 1-100000 (最小 RAM 大小（) ）。</span><span class="sxs-lookup"><span data-stu-id="f7258-210">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="f7258-211">有效值为 1 到 100000</span><span class="sxs-lookup"><span data-stu-id="f7258-211">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="f7258-212">minimumDiskSizeAllowedToPeerInGtesbytes</span><span class="sxs-lookup"><span data-stu-id="f7258-212">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="f7258-213">Int32</span><span class="sxs-lookup"><span data-stu-id="f7258-213">Int32</span></span>|<span data-ttu-id="f7258-214">指定使用 1-100000 (1-100000 个对等缓存) 。</span><span class="sxs-lookup"><span data-stu-id="f7258-214">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="f7258-215">有效值为 1 到 100000</span><span class="sxs-lookup"><span data-stu-id="f7258-215">Valid values 1 to 100000</span></span>
<span data-ttu-id="f7258-216">建议的值：64 GB 到 256 GB。</span><span class="sxs-lookup"><span data-stu-id="f7258-216">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="f7258-217">有效值为 1 到 100000</span><span class="sxs-lookup"><span data-stu-id="f7258-217">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="f7258-218">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="f7258-218">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="f7258-219">Int32</span><span class="sxs-lookup"><span data-stu-id="f7258-219">Int32</span></span>|<span data-ttu-id="f7258-220">指定启用最小内容文件大小（以 MB 为单位）以使用 1-100000 (1-100000) 。</span><span class="sxs-lookup"><span data-stu-id="f7258-220">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="f7258-221">有效值为 1 到 100000</span><span class="sxs-lookup"><span data-stu-id="f7258-221">Valid values 1 to 100000</span></span>
<span data-ttu-id="f7258-222">建议的值：1 MB 到 100，000 MB。</span><span class="sxs-lookup"><span data-stu-id="f7258-222">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="f7258-223">有效值为 1 到 100000</span><span class="sxs-lookup"><span data-stu-id="f7258-223">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="f7258-224">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="f7258-224">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="f7258-225">Int32</span><span class="sxs-lookup"><span data-stu-id="f7258-225">Int32</span></span>|<span data-ttu-id="f7258-226">指定允许设备将数据上载到 0-100 (的最小电池百) 。</span><span class="sxs-lookup"><span data-stu-id="f7258-226">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="f7258-227">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="f7258-227">Valid values 0 to 100</span></span>
<span data-ttu-id="f7258-228">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="f7258-228">The default value is 0.</span></span> <span data-ttu-id="f7258-229">值 0 (零) 表示"没有限制"，将使用云服务默认值。</span><span class="sxs-lookup"><span data-stu-id="f7258-229">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="f7258-230">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="f7258-230">Valid values 0 to 100</span></span>|
|<span data-ttu-id="f7258-231">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="f7258-231">modifyCacheLocation</span></span>|<span data-ttu-id="f7258-232">String</span><span class="sxs-lookup"><span data-stu-id="f7258-232">String</span></span>|<span data-ttu-id="f7258-233">指定传递优化应该用于其缓存的驱动器。</span><span class="sxs-lookup"><span data-stu-id="f7258-233">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="f7258-234">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="f7258-234">maximumCacheAgeInDays</span></span>|<span data-ttu-id="f7258-235">Int32</span><span class="sxs-lookup"><span data-stu-id="f7258-235">Int32</span></span>|<span data-ttu-id="f7258-236">指定在 0-3650 或 0-3650 (后每个文件在传递优化缓存中保存的最大) 。</span><span class="sxs-lookup"><span data-stu-id="f7258-236">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="f7258-237">有效值为 0 到 3650</span><span class="sxs-lookup"><span data-stu-id="f7258-237">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="f7258-238">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="f7258-238">maximumCacheSize</span></span>|[<span data-ttu-id="f7258-239">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="f7258-239">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="f7258-240">以百分比或 GB 为单位指定传递优化的最大缓存大小。</span><span class="sxs-lookup"><span data-stu-id="f7258-240">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="f7258-241">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="f7258-241">vpnPeerCaching</span></span>|[<span data-ttu-id="f7258-242">enablement</span><span class="sxs-lookup"><span data-stu-id="f7258-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f7258-243">指定是否允许设备在通过 VPN 连接到域网络时参与对等缓存。</span><span class="sxs-lookup"><span data-stu-id="f7258-243">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="f7258-244">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f7258-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f7258-245">cacheServerHostNames</span><span class="sxs-lookup"><span data-stu-id="f7258-245">cacheServerHostNames</span></span>|<span data-ttu-id="f7258-246">String collection</span><span class="sxs-lookup"><span data-stu-id="f7258-246">String collection</span></span>|<span data-ttu-id="f7258-247">指定缓存服务器主机名。</span><span class="sxs-lookup"><span data-stu-id="f7258-247">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="f7258-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="f7258-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="f7258-249">Int32</span><span class="sxs-lookup"><span data-stu-id="f7258-249">Int32</span></span>|<span data-ttu-id="f7258-250">指定延迟从缓存服务器回退到前台下载的 HTTP 源的秒数。</span><span class="sxs-lookup"><span data-stu-id="f7258-250">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="f7258-251">有效值为 0 到 2592000。</span><span class="sxs-lookup"><span data-stu-id="f7258-251">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="f7258-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="f7258-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="f7258-253">Int32</span><span class="sxs-lookup"><span data-stu-id="f7258-253">Int32</span></span>|<span data-ttu-id="f7258-254">指定延迟从缓存服务器回退到 HTTP 源进行后台下载的秒数。</span><span class="sxs-lookup"><span data-stu-id="f7258-254">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="f7258-255">有效值为 0 到 2592000。</span><span class="sxs-lookup"><span data-stu-id="f7258-255">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="f7258-256">响应</span><span class="sxs-lookup"><span data-stu-id="f7258-256">Response</span></span>
<span data-ttu-id="f7258-257">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7258-257">If successful, this method returns a `200 OK` response code and an updated [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7258-258">示例</span><span class="sxs-lookup"><span data-stu-id="f7258-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7258-259">请求</span><span class="sxs-lookup"><span data-stu-id="f7258-259">Request</span></span>
<span data-ttu-id="f7258-260">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7258-260">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2039

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled",
  "cacheServerHostNames": [
    "Cache Server Host Names value"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
}
```

### <a name="response"></a><span data-ttu-id="f7258-261">响应</span><span class="sxs-lookup"><span data-stu-id="f7258-261">Response</span></span>
<span data-ttu-id="f7258-p130">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7258-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2211

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
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
  "restrictPeerSelectionBy": "subnetMask",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 8,
  "foregroundDownloadFromHttpDelayInSeconds": 8,
  "minimumRamAllowedToPeerInGigabytes": 2,
  "minimumDiskSizeAllowedToPeerInGigabytes": 7,
  "minimumFileSizeToCacheInMegabytes": 1,
  "minimumBatteryPercentageAllowedToUpload": 7,
  "modifyCacheLocation": "Modify Cache Location value",
  "maximumCacheAgeInDays": 5,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "enabled",
  "cacheServerHostNames": [
    "Cache Server Host Names value"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 9,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 9
}
```




