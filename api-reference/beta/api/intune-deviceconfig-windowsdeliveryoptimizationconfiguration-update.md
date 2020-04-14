---
title: 更新 windowsDeliveryOptimizationConfiguration
description: 更新 windowsDeliveryOptimizationConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6412079701585a157ab760bdc6f78f7175d26b7a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43429669"
---
# <a name="update-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="fad7e-103">更新 windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="fad7e-103">Update windowsDeliveryOptimizationConfiguration</span></span>

<span data-ttu-id="fad7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fad7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fad7e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fad7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fad7e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fad7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fad7e-107">更新[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fad7e-107">Update the properties of a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fad7e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fad7e-108">Prerequisites</span></span>
<span data-ttu-id="fad7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fad7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fad7e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fad7e-111">Permission type</span></span>|<span data-ttu-id="fad7e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fad7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fad7e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fad7e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fad7e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad7e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fad7e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fad7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fad7e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fad7e-116">Not supported.</span></span>|
|<span data-ttu-id="fad7e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fad7e-117">Application</span></span>|<span data-ttu-id="fad7e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad7e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fad7e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fad7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fad7e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fad7e-120">Request headers</span></span>
|<span data-ttu-id="fad7e-121">标头</span><span class="sxs-lookup"><span data-stu-id="fad7e-121">Header</span></span>|<span data-ttu-id="fad7e-122">值</span><span class="sxs-lookup"><span data-stu-id="fad7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fad7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fad7e-123">Authorization</span></span>|<span data-ttu-id="fad7e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fad7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fad7e-125">接受</span><span class="sxs-lookup"><span data-stu-id="fad7e-125">Accept</span></span>|<span data-ttu-id="fad7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fad7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fad7e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fad7e-127">Request body</span></span>
<span data-ttu-id="fad7e-128">在请求正文中，提供[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fad7e-128">In the request body, supply a JSON representation for the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

<span data-ttu-id="fad7e-129">下表显示创建[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fad7e-129">The following table shows the properties that are required when you create the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

|<span data-ttu-id="fad7e-130">属性</span><span class="sxs-lookup"><span data-stu-id="fad7e-130">Property</span></span>|<span data-ttu-id="fad7e-131">类型</span><span class="sxs-lookup"><span data-stu-id="fad7e-131">Type</span></span>|<span data-ttu-id="fad7e-132">说明</span><span class="sxs-lookup"><span data-stu-id="fad7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fad7e-133">id</span><span class="sxs-lookup"><span data-stu-id="fad7e-133">id</span></span>|<span data-ttu-id="fad7e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="fad7e-134">String</span></span>|<span data-ttu-id="fad7e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fad7e-135">Key of the entity.</span></span> <span data-ttu-id="fad7e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fad7e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fad7e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad7e-138">DateTimeOffset</span></span>|<span data-ttu-id="fad7e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fad7e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fad7e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fad7e-141">roleScopeTagIds</span></span>|<span data-ttu-id="fad7e-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="fad7e-142">String collection</span></span>|<span data-ttu-id="fad7e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fad7e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fad7e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fad7e-145">supportsScopeTags</span></span>|<span data-ttu-id="fad7e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fad7e-146">Boolean</span></span>|<span data-ttu-id="fad7e-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="fad7e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fad7e-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="fad7e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fad7e-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="fad7e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fad7e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fad7e-150">This property is read-only.</span></span> <span data-ttu-id="fad7e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fad7e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fad7e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fad7e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fad7e-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="fad7e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fad7e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fad7e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fad7e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fad7e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fad7e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fad7e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fad7e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fad7e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fad7e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fad7e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fad7e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fad7e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fad7e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fad7e-164">createdDateTime</span></span>|<span data-ttu-id="fad7e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fad7e-165">DateTimeOffset</span></span>|<span data-ttu-id="fad7e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fad7e-166">DateTime the object was created.</span></span> <span data-ttu-id="fad7e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-168">description</span><span class="sxs-lookup"><span data-stu-id="fad7e-168">description</span></span>|<span data-ttu-id="fad7e-169">String</span><span class="sxs-lookup"><span data-stu-id="fad7e-169">String</span></span>|<span data-ttu-id="fad7e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fad7e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fad7e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fad7e-172">displayName</span></span>|<span data-ttu-id="fad7e-173">String</span><span class="sxs-lookup"><span data-stu-id="fad7e-173">String</span></span>|<span data-ttu-id="fad7e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fad7e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fad7e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-176">version</span><span class="sxs-lookup"><span data-stu-id="fad7e-176">version</span></span>|<span data-ttu-id="fad7e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fad7e-177">Int32</span></span>|<span data-ttu-id="fad7e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fad7e-178">Version of the device configuration.</span></span> <span data-ttu-id="fad7e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fad7e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fad7e-180">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="fad7e-180">deliveryOptimizationMode</span></span>|[<span data-ttu-id="fad7e-181">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="fad7e-181">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="fad7e-182">指定传递优化可用于管理大型内容分布方案的网络带宽消耗的下载方法。</span><span class="sxs-lookup"><span data-stu-id="fad7e-182">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="fad7e-183">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="fad7e-183">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="fad7e-184">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="fad7e-184">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="fad7e-185">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="fad7e-185">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="fad7e-186">指定通过选中的选项来限制对等方选择。</span><span class="sxs-lookup"><span data-stu-id="fad7e-186">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="fad7e-187">选项1（子网掩码）仅适用于传递优化模式：下载模式 LAN （1）和组（2）。</span><span class="sxs-lookup"><span data-stu-id="fad7e-187">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="fad7e-188">可取值为：`notConfigured`、`subnetMask`。</span><span class="sxs-lookup"><span data-stu-id="fad7e-188">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="fad7e-189">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="fad7e-189">groupIdSource</span></span>|[<span data-ttu-id="fad7e-190">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="fad7e-190">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="fad7e-191">指定将对等选择限制为特定源。</span><span class="sxs-lookup"><span data-stu-id="fad7e-191">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="fad7e-192">此策略中设置的选项仅适用于传递优化模式组（2）下载模式。</span><span class="sxs-lookup"><span data-stu-id="fad7e-192">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="fad7e-193">如果组（2）未设置为下载模式，此策略将被忽略。</span><span class="sxs-lookup"><span data-stu-id="fad7e-193">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="fad7e-194">对于选项 3-DHCP 选项 ID，客户端将查询 DHCP 选项 ID 234，并使用返回的 GUID 值作为组 ID。</span><span class="sxs-lookup"><span data-stu-id="fad7e-194">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="fad7e-195">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="fad7e-195">bandwidthMode</span></span>|[<span data-ttu-id="fad7e-196">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="fad7e-196">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="fad7e-197">指定使用百分比、absolutes 或小时的前景色和背景带宽使用情况。</span><span class="sxs-lookup"><span data-stu-id="fad7e-197">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="fad7e-198">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="fad7e-198">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="fad7e-199">Int64</span><span class="sxs-lookup"><span data-stu-id="fad7e-199">Int64</span></span>|<span data-ttu-id="fad7e-200">指定允许使用对等的后台下载中的 HTTP 源延迟的秒数。</span><span class="sxs-lookup"><span data-stu-id="fad7e-200">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="fad7e-201">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="fad7e-201">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="fad7e-202">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="fad7e-202">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="fad7e-203">Int64</span><span class="sxs-lookup"><span data-stu-id="fad7e-203">Int64</span></span>|<span data-ttu-id="fad7e-204">指定在允许使用对等（0-86400）的前台下载中延迟 HTTP 源的秒数。</span><span class="sxs-lookup"><span data-stu-id="fad7e-204">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="fad7e-205">有效值为0至86400</span><span class="sxs-lookup"><span data-stu-id="fad7e-205">Valid values 0 to 86400</span></span>
<span data-ttu-id="fad7e-206">指定0将传递优化设置为使用云服务管理此设置。</span><span class="sxs-lookup"><span data-stu-id="fad7e-206">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="fad7e-207">有效值为0至86400</span><span class="sxs-lookup"><span data-stu-id="fad7e-207">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="fad7e-208">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="fad7e-208">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="fad7e-209">Int32</span><span class="sxs-lookup"><span data-stu-id="fad7e-209">Int32</span></span>|<span data-ttu-id="fad7e-210">指定使用对等缓存的最小 RAM 大小（以 GB 为单位）（1-100000）。</span><span class="sxs-lookup"><span data-stu-id="fad7e-210">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="fad7e-211">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="fad7e-211">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="fad7e-212">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="fad7e-212">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="fad7e-213">Int32</span><span class="sxs-lookup"><span data-stu-id="fad7e-213">Int32</span></span>|<span data-ttu-id="fad7e-214">指定使用对等缓存的最小磁盘大小（以 GB 为单位）（1-100000）。</span><span class="sxs-lookup"><span data-stu-id="fad7e-214">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="fad7e-215">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="fad7e-215">Valid values 1 to 100000</span></span>
<span data-ttu-id="fad7e-216">建议值： 64 GB 到 256 GB。</span><span class="sxs-lookup"><span data-stu-id="fad7e-216">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="fad7e-217">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="fad7e-217">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="fad7e-218">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="fad7e-218">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="fad7e-219">Int32</span><span class="sxs-lookup"><span data-stu-id="fad7e-219">Int32</span></span>|<span data-ttu-id="fad7e-220">指定启用以使用对等缓存（1-100000）的最小内容文件大小（以 MB 为单位）。</span><span class="sxs-lookup"><span data-stu-id="fad7e-220">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="fad7e-221">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="fad7e-221">Valid values 1 to 100000</span></span>
<span data-ttu-id="fad7e-222">推荐值： 1 MB 到 100000 MB。</span><span class="sxs-lookup"><span data-stu-id="fad7e-222">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="fad7e-223">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="fad7e-223">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="fad7e-224">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="fad7e-224">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="fad7e-225">Int32</span><span class="sxs-lookup"><span data-stu-id="fad7e-225">Int32</span></span>|<span data-ttu-id="fad7e-226">指定允许设备上传数据的最小电池百分比（0-100）。</span><span class="sxs-lookup"><span data-stu-id="fad7e-226">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="fad7e-227">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="fad7e-227">Valid values 0 to 100</span></span>
<span data-ttu-id="fad7e-228">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="fad7e-228">The default value is 0.</span></span> <span data-ttu-id="fad7e-229">值为0（零）表示 "不受限制"，将使用云服务默认值。</span><span class="sxs-lookup"><span data-stu-id="fad7e-229">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="fad7e-230">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="fad7e-230">Valid values 0 to 100</span></span>|
|<span data-ttu-id="fad7e-231">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="fad7e-231">modifyCacheLocation</span></span>|<span data-ttu-id="fad7e-232">String</span><span class="sxs-lookup"><span data-stu-id="fad7e-232">String</span></span>|<span data-ttu-id="fad7e-233">指定传递优化应用于其缓存的驱动器。</span><span class="sxs-lookup"><span data-stu-id="fad7e-233">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="fad7e-234">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="fad7e-234">maximumCacheAgeInDays</span></span>|<span data-ttu-id="fad7e-235">Int32</span><span class="sxs-lookup"><span data-stu-id="fad7e-235">Int32</span></span>|<span data-ttu-id="fad7e-236">指定在成功下载后，每个文件保留在传递优化缓存中的最长时间（以天为单位）（0-3650）。</span><span class="sxs-lookup"><span data-stu-id="fad7e-236">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-3650).</span></span> <span data-ttu-id="fad7e-237">有效值为0至3650</span><span class="sxs-lookup"><span data-stu-id="fad7e-237">Valid values 0 to 3650</span></span>|
|<span data-ttu-id="fad7e-238">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="fad7e-238">maximumCacheSize</span></span>|[<span data-ttu-id="fad7e-239">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="fad7e-239">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="fad7e-240">指定传递优化的最大缓存大小（以百分比或 GB 为单位）。</span><span class="sxs-lookup"><span data-stu-id="fad7e-240">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="fad7e-241">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="fad7e-241">vpnPeerCaching</span></span>|[<span data-ttu-id="fad7e-242">启用</span><span class="sxs-lookup"><span data-stu-id="fad7e-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fad7e-243">指定是否允许设备在通过 VPN 连接到域网络时参与对等缓存。</span><span class="sxs-lookup"><span data-stu-id="fad7e-243">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="fad7e-244">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="fad7e-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fad7e-245">cacheServerHostNames</span><span class="sxs-lookup"><span data-stu-id="fad7e-245">cacheServerHostNames</span></span>|<span data-ttu-id="fad7e-246">String 集合</span><span class="sxs-lookup"><span data-stu-id="fad7e-246">String collection</span></span>|<span data-ttu-id="fad7e-247">指定缓存服务器的主机名。</span><span class="sxs-lookup"><span data-stu-id="fad7e-247">Specifies cache servers host names.</span></span>|
|<span data-ttu-id="fad7e-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="fad7e-248">cacheServerForegroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="fad7e-249">Int32</span><span class="sxs-lookup"><span data-stu-id="fad7e-249">Int32</span></span>|<span data-ttu-id="fad7e-250">指定前台下载延迟从缓存服务器回退到 HTTP 源的秒数。</span><span class="sxs-lookup"><span data-stu-id="fad7e-250">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a foreground download.</span></span> <span data-ttu-id="fad7e-251">有效的值为0到2592000。</span><span class="sxs-lookup"><span data-stu-id="fad7e-251">Valid values 0 to 2592000.</span></span>|
|<span data-ttu-id="fad7e-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="fad7e-252">cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds</span></span>|<span data-ttu-id="fad7e-253">Int32</span><span class="sxs-lookup"><span data-stu-id="fad7e-253">Int32</span></span>|<span data-ttu-id="fad7e-254">指定从缓存服务器回退到用于后台下载的 HTTP 源的秒数。</span><span class="sxs-lookup"><span data-stu-id="fad7e-254">Specifies number of seconds to delay a fall back from cache servers to an HTTP source for a background download.</span></span> <span data-ttu-id="fad7e-255">有效的值为0到2592000。</span><span class="sxs-lookup"><span data-stu-id="fad7e-255">Valid values 0 to 2592000.</span></span>|



## <a name="response"></a><span data-ttu-id="fad7e-256">响应</span><span class="sxs-lookup"><span data-stu-id="fad7e-256">Response</span></span>
<span data-ttu-id="fad7e-257">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fad7e-257">If successful, this method returns a `200 OK` response code and an updated [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fad7e-258">示例</span><span class="sxs-lookup"><span data-stu-id="fad7e-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="fad7e-259">请求</span><span class="sxs-lookup"><span data-stu-id="fad7e-259">Request</span></span>
<span data-ttu-id="fad7e-260">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fad7e-260">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fad7e-261">响应</span><span class="sxs-lookup"><span data-stu-id="fad7e-261">Response</span></span>
<span data-ttu-id="fad7e-p130">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fad7e-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



