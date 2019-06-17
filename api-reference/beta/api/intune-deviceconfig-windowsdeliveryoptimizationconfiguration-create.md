---
title: 创建 windowsDeliveryOptimizationConfiguration
description: 创建新的 windowsDeliveryOptimizationConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b504d7a403aec15fad14ae370bf4d76fb7bf7f6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977614"
---
# <a name="create-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="84f0d-103">创建 windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="84f0d-103">Create windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="84f0d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84f0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84f0d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84f0d-106">创建新的[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84f0d-106">Create a new [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84f0d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="84f0d-107">Prerequisites</span></span>
<span data-ttu-id="84f0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84f0d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="84f0d-110">Permission type</span></span>|<span data-ttu-id="84f0d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84f0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84f0d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84f0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84f0d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84f0d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84f0d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84f0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84f0d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84f0d-115">Not supported.</span></span>|
|<span data-ttu-id="84f0d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="84f0d-116">Application</span></span>|<span data-ttu-id="84f0d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="84f0d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84f0d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84f0d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84f0d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="84f0d-119">Request headers</span></span>
|<span data-ttu-id="84f0d-120">标头</span><span class="sxs-lookup"><span data-stu-id="84f0d-120">Header</span></span>|<span data-ttu-id="84f0d-121">值</span><span class="sxs-lookup"><span data-stu-id="84f0d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84f0d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84f0d-122">Authorization</span></span>|<span data-ttu-id="84f0d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84f0d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84f0d-124">接受</span><span class="sxs-lookup"><span data-stu-id="84f0d-124">Accept</span></span>|<span data-ttu-id="84f0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84f0d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84f0d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="84f0d-126">Request body</span></span>
<span data-ttu-id="84f0d-127">在请求正文中, 提供 windowsDeliveryOptimizationConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84f0d-127">In the request body, supply a JSON representation for the windowsDeliveryOptimizationConfiguration object.</span></span>

<span data-ttu-id="84f0d-128">下表显示创建 windowsDeliveryOptimizationConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="84f0d-128">The following table shows the properties that are required when you create the windowsDeliveryOptimizationConfiguration.</span></span>

|<span data-ttu-id="84f0d-129">属性</span><span class="sxs-lookup"><span data-stu-id="84f0d-129">Property</span></span>|<span data-ttu-id="84f0d-130">类型</span><span class="sxs-lookup"><span data-stu-id="84f0d-130">Type</span></span>|<span data-ttu-id="84f0d-131">说明</span><span class="sxs-lookup"><span data-stu-id="84f0d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84f0d-132">id</span><span class="sxs-lookup"><span data-stu-id="84f0d-132">id</span></span>|<span data-ttu-id="84f0d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="84f0d-133">String</span></span>|<span data-ttu-id="84f0d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="84f0d-134">Key of the entity.</span></span> <span data-ttu-id="84f0d-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84f0d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="84f0d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84f0d-137">DateTimeOffset</span></span>|<span data-ttu-id="84f0d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="84f0d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="84f0d-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84f0d-140">roleScopeTagIds</span></span>|<span data-ttu-id="84f0d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="84f0d-141">String collection</span></span>|<span data-ttu-id="84f0d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="84f0d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84f0d-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84f0d-144">supportsScopeTags</span></span>|<span data-ttu-id="84f0d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="84f0d-145">Boolean</span></span>|<span data-ttu-id="84f0d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="84f0d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84f0d-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="84f0d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84f0d-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="84f0d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84f0d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="84f0d-149">This property is read-only.</span></span> <span data-ttu-id="84f0d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="84f0d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="84f0d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="84f0d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="84f0d-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="84f0d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="84f0d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="84f0d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="84f0d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="84f0d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="84f0d-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="84f0d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="84f0d-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="84f0d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="84f0d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="84f0d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="84f0d-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="84f0d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="84f0d-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84f0d-163">createdDateTime</span></span>|<span data-ttu-id="84f0d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84f0d-164">DateTimeOffset</span></span>|<span data-ttu-id="84f0d-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="84f0d-165">DateTime the object was created.</span></span> <span data-ttu-id="84f0d-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-167">说明</span><span class="sxs-lookup"><span data-stu-id="84f0d-167">description</span></span>|<span data-ttu-id="84f0d-168">String</span><span class="sxs-lookup"><span data-stu-id="84f0d-168">String</span></span>|<span data-ttu-id="84f0d-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="84f0d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84f0d-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="84f0d-171">displayName</span></span>|<span data-ttu-id="84f0d-172">String</span><span class="sxs-lookup"><span data-stu-id="84f0d-172">String</span></span>|<span data-ttu-id="84f0d-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="84f0d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84f0d-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-175">version</span><span class="sxs-lookup"><span data-stu-id="84f0d-175">version</span></span>|<span data-ttu-id="84f0d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-176">Int32</span></span>|<span data-ttu-id="84f0d-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="84f0d-177">Version of the device configuration.</span></span> <span data-ttu-id="84f0d-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84f0d-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84f0d-179">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="84f0d-179">deliveryOptimizationMode</span></span>|[<span data-ttu-id="84f0d-180">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="84f0d-180">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="84f0d-181">指定传递优化可用于管理大型内容分布方案的网络带宽消耗的下载方法。</span><span class="sxs-lookup"><span data-stu-id="84f0d-181">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="84f0d-182">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="84f0d-182">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="84f0d-183">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="84f0d-183">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="84f0d-184">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="84f0d-184">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="84f0d-185">指定通过选中的选项来限制对等方选择。</span><span class="sxs-lookup"><span data-stu-id="84f0d-185">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="84f0d-186">选项 1 (子网掩码) 仅适用于传递优化模式: 下载模式 LAN (1) 和组 (2)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-186">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="84f0d-187">可取值为：`notConfigured`、`subnetMask`。</span><span class="sxs-lookup"><span data-stu-id="84f0d-187">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="84f0d-188">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="84f0d-188">groupIdSource</span></span>|[<span data-ttu-id="84f0d-189">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="84f0d-189">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="84f0d-190">指定将对等选择限制为特定源。</span><span class="sxs-lookup"><span data-stu-id="84f0d-190">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="84f0d-191">此策略中设置的选项仅适用于传递优化模式组 (2) 下载模式。</span><span class="sxs-lookup"><span data-stu-id="84f0d-191">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="84f0d-192">如果组 (2) 未设置为下载模式, 此策略将被忽略。</span><span class="sxs-lookup"><span data-stu-id="84f0d-192">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="84f0d-193">对于选项 3-DHCP 选项 ID, 客户端将查询 DHCP 选项 ID 234, 并使用返回的 GUID 值作为组 ID。</span><span class="sxs-lookup"><span data-stu-id="84f0d-193">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="84f0d-194">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="84f0d-194">bandwidthMode</span></span>|[<span data-ttu-id="84f0d-195">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="84f0d-195">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="84f0d-196">指定使用百分比、absolutes 或小时的前景色和背景带宽使用情况。</span><span class="sxs-lookup"><span data-stu-id="84f0d-196">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="84f0d-197">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="84f0d-197">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="84f0d-198">Int64</span><span class="sxs-lookup"><span data-stu-id="84f0d-198">Int64</span></span>|<span data-ttu-id="84f0d-199">指定允许使用对等的后台下载中的 HTTP 源延迟的秒数。</span><span class="sxs-lookup"><span data-stu-id="84f0d-199">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="84f0d-200">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="84f0d-200">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="84f0d-201">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="84f0d-201">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="84f0d-202">Int64</span><span class="sxs-lookup"><span data-stu-id="84f0d-202">Int64</span></span>|<span data-ttu-id="84f0d-203">指定在允许使用对等 (0-86400) 的前台下载中延迟 HTTP 源的秒数。</span><span class="sxs-lookup"><span data-stu-id="84f0d-203">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="84f0d-204">有效值为0至86400</span><span class="sxs-lookup"><span data-stu-id="84f0d-204">Valid values 0 to 86400</span></span>
<span data-ttu-id="84f0d-205">指定0将传递优化设置为使用云服务管理此设置。</span><span class="sxs-lookup"><span data-stu-id="84f0d-205">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="84f0d-206">有效值为0至86400</span><span class="sxs-lookup"><span data-stu-id="84f0d-206">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="84f0d-207">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="84f0d-207">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="84f0d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-208">Int32</span></span>|<span data-ttu-id="84f0d-209">指定使用对等缓存的最小 RAM 大小 (以 GB 为单位) (1-100000)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-209">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="84f0d-210">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="84f0d-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="84f0d-211">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="84f0d-211">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="84f0d-212">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-212">Int32</span></span>|<span data-ttu-id="84f0d-213">指定使用对等缓存的最小磁盘大小 (以 GB 为单位) (1-100000)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-213">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="84f0d-214">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="84f0d-214">Valid values 1 to 100000</span></span>
<span data-ttu-id="84f0d-215">建议值:64 GB 到 256 GB。</span><span class="sxs-lookup"><span data-stu-id="84f0d-215">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="84f0d-216">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="84f0d-216">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="84f0d-217">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="84f0d-217">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="84f0d-218">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-218">Int32</span></span>|<span data-ttu-id="84f0d-219">指定启用以使用对等缓存 (1-100000) 的最小内容文件大小 (以 MB 为单位)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-219">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="84f0d-220">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="84f0d-220">Valid values 1 to 100000</span></span>
<span data-ttu-id="84f0d-221">推荐值: 1 MB 到 100000 MB。</span><span class="sxs-lookup"><span data-stu-id="84f0d-221">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="84f0d-222">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="84f0d-222">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="84f0d-223">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="84f0d-223">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="84f0d-224">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-224">Int32</span></span>|<span data-ttu-id="84f0d-225">指定允许设备上传数据的最小电池百分比 (0-100)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-225">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="84f0d-226">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="84f0d-226">Valid values 0 to 100</span></span>
<span data-ttu-id="84f0d-227">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="84f0d-227">The default value is 0.</span></span> <span data-ttu-id="84f0d-228">值为 0 (零) 表示 "不受限制", 将使用云服务默认值。</span><span class="sxs-lookup"><span data-stu-id="84f0d-228">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="84f0d-229">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="84f0d-229">Valid values 0 to 100</span></span>|
|<span data-ttu-id="84f0d-230">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="84f0d-230">modifyCacheLocation</span></span>|<span data-ttu-id="84f0d-231">String</span><span class="sxs-lookup"><span data-stu-id="84f0d-231">String</span></span>|<span data-ttu-id="84f0d-232">指定传递优化应用于其缓存的驱动器。</span><span class="sxs-lookup"><span data-stu-id="84f0d-232">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="84f0d-233">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="84f0d-233">maximumCacheAgeInDays</span></span>|<span data-ttu-id="84f0d-234">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-234">Int32</span></span>|<span data-ttu-id="84f0d-235">指定在成功下载后, 每个文件保留在传递优化缓存中的最长时间 (以天为单位) (0-3650)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-235">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="84f0d-236">有效值为0至3650</span><span class="sxs-lookup"><span data-stu-id="84f0d-236">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="84f0d-237">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="84f0d-237">maximumCacheSize</span></span>|[<span data-ttu-id="84f0d-238">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="84f0d-238">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="84f0d-239">指定传递优化的最大缓存大小 (以百分比或 GB 为单位)。</span><span class="sxs-lookup"><span data-stu-id="84f0d-239">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="84f0d-240">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="84f0d-240">vpnPeerCaching</span></span>|[<span data-ttu-id="84f0d-241">启用</span><span class="sxs-lookup"><span data-stu-id="84f0d-241">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="84f0d-242">指定是否允许设备在通过 VPN 连接到域网络时参与对等缓存。</span><span class="sxs-lookup"><span data-stu-id="84f0d-242">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="84f0d-243">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="84f0d-243">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="84f0d-244">响应</span><span class="sxs-lookup"><span data-stu-id="84f0d-244">Response</span></span>
<span data-ttu-id="84f0d-245">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84f0d-245">If successful, this method returns a `201 Created` response code and a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84f0d-246">示例</span><span class="sxs-lookup"><span data-stu-id="84f0d-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="84f0d-247">请求</span><span class="sxs-lookup"><span data-stu-id="84f0d-247">Request</span></span>
<span data-ttu-id="84f0d-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84f0d-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1833

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
  "vpnPeerCaching": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="84f0d-249">响应</span><span class="sxs-lookup"><span data-stu-id="84f0d-249">Response</span></span>
<span data-ttu-id="84f0d-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84f0d-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2005

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
  "vpnPeerCaching": "enabled"
}
```





