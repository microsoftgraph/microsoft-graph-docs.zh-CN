---
title: 更新 windowsDeliveryOptimizationConfiguration
description: 更新 windowsDeliveryOptimizationConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ccd1e01d4574cc45b039f8c0c60bc5aaea67779
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983839"
---
# <a name="update-windowsdeliveryoptimizationconfiguration"></a><span data-ttu-id="0599d-103">更新 windowsDeliveryOptimizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0599d-103">Update windowsDeliveryOptimizationConfiguration</span></span>

> <span data-ttu-id="0599d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0599d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0599d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0599d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0599d-106">更新[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0599d-106">Update the properties of a [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0599d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0599d-107">Prerequisites</span></span>
<span data-ttu-id="0599d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0599d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0599d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0599d-110">Permission type</span></span>|<span data-ttu-id="0599d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0599d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0599d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0599d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0599d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0599d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0599d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0599d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0599d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0599d-115">Not supported.</span></span>|
|<span data-ttu-id="0599d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0599d-116">Application</span></span>|<span data-ttu-id="0599d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0599d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0599d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0599d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0599d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0599d-119">Request headers</span></span>
|<span data-ttu-id="0599d-120">标头</span><span class="sxs-lookup"><span data-stu-id="0599d-120">Header</span></span>|<span data-ttu-id="0599d-121">值</span><span class="sxs-lookup"><span data-stu-id="0599d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0599d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0599d-122">Authorization</span></span>|<span data-ttu-id="0599d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0599d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0599d-124">接受</span><span class="sxs-lookup"><span data-stu-id="0599d-124">Accept</span></span>|<span data-ttu-id="0599d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0599d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0599d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0599d-126">Request body</span></span>
<span data-ttu-id="0599d-127">在请求正文中, 提供[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0599d-127">In the request body, supply a JSON representation for the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object.</span></span>

<span data-ttu-id="0599d-128">下表显示创建[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0599d-128">The following table shows the properties that are required when you create the [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).</span></span>

|<span data-ttu-id="0599d-129">属性</span><span class="sxs-lookup"><span data-stu-id="0599d-129">Property</span></span>|<span data-ttu-id="0599d-130">类型</span><span class="sxs-lookup"><span data-stu-id="0599d-130">Type</span></span>|<span data-ttu-id="0599d-131">说明</span><span class="sxs-lookup"><span data-stu-id="0599d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0599d-132">id</span><span class="sxs-lookup"><span data-stu-id="0599d-132">id</span></span>|<span data-ttu-id="0599d-133">String</span><span class="sxs-lookup"><span data-stu-id="0599d-133">String</span></span>|<span data-ttu-id="0599d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0599d-134">Key of the entity.</span></span> <span data-ttu-id="0599d-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0599d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0599d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0599d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0599d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0599d-137">DateTimeOffset</span></span>|<span data-ttu-id="0599d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0599d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0599d-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0599d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0599d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0599d-140">roleScopeTagIds</span></span>|<span data-ttu-id="0599d-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="0599d-141">String collection</span></span>|<span data-ttu-id="0599d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0599d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0599d-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0599d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0599d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0599d-144">supportsScopeTags</span></span>|<span data-ttu-id="0599d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0599d-145">Boolean</span></span>|<span data-ttu-id="0599d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0599d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0599d-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0599d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0599d-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0599d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0599d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0599d-149">This property is read-only.</span></span> <span data-ttu-id="0599d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0599d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0599d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0599d-151">createdDateTime</span></span>|<span data-ttu-id="0599d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0599d-152">DateTimeOffset</span></span>|<span data-ttu-id="0599d-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0599d-153">DateTime the object was created.</span></span> <span data-ttu-id="0599d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0599d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0599d-155">description</span><span class="sxs-lookup"><span data-stu-id="0599d-155">description</span></span>|<span data-ttu-id="0599d-156">String</span><span class="sxs-lookup"><span data-stu-id="0599d-156">String</span></span>|<span data-ttu-id="0599d-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0599d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0599d-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0599d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0599d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0599d-159">displayName</span></span>|<span data-ttu-id="0599d-160">String</span><span class="sxs-lookup"><span data-stu-id="0599d-160">String</span></span>|<span data-ttu-id="0599d-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0599d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0599d-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0599d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0599d-163">version</span><span class="sxs-lookup"><span data-stu-id="0599d-163">version</span></span>|<span data-ttu-id="0599d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0599d-164">Int32</span></span>|<span data-ttu-id="0599d-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0599d-165">Version of the device configuration.</span></span> <span data-ttu-id="0599d-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0599d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0599d-167">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0599d-167">deliveryOptimizationMode</span></span>|[<span data-ttu-id="0599d-168">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0599d-168">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="0599d-169">指定传递优化可用于管理大型内容分布方案的网络带宽消耗的下载方法。</span><span class="sxs-lookup"><span data-stu-id="0599d-169">Specifies the download method that delivery optimization can use to manage network bandwidth consumption for large content distribution scenarios.</span></span> <span data-ttu-id="0599d-170">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="0599d-170">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="0599d-171">restrictPeerSelectionBy</span><span class="sxs-lookup"><span data-stu-id="0599d-171">restrictPeerSelectionBy</span></span>|[<span data-ttu-id="0599d-172">deliveryOptimizationRestrictPeerSelectionByOptions</span><span class="sxs-lookup"><span data-stu-id="0599d-172">deliveryOptimizationRestrictPeerSelectionByOptions</span></span>](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|<span data-ttu-id="0599d-173">指定通过选中的选项来限制对等方选择。</span><span class="sxs-lookup"><span data-stu-id="0599d-173">Specifies to restrict peer selection via selected option.</span></span>
<span data-ttu-id="0599d-174">选项 1 (子网掩码) 仅适用于传递优化模式: 下载模式 LAN (1) 和组 (2)。</span><span class="sxs-lookup"><span data-stu-id="0599d-174">Option 1 (Subnet mask) only applies to Delivery Optimization modes Download Mode LAN (1) and Group (2).</span></span> <span data-ttu-id="0599d-175">可取值为：`notConfigured`、`subnetMask`。</span><span class="sxs-lookup"><span data-stu-id="0599d-175">Possible values are: `notConfigured`, `subnetMask`.</span></span>|
|<span data-ttu-id="0599d-176">groupIdSource</span><span class="sxs-lookup"><span data-stu-id="0599d-176">groupIdSource</span></span>|[<span data-ttu-id="0599d-177">deliveryOptimizationGroupIdSource</span><span class="sxs-lookup"><span data-stu-id="0599d-177">deliveryOptimizationGroupIdSource</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|<span data-ttu-id="0599d-178">指定将对等选择限制为特定源。</span><span class="sxs-lookup"><span data-stu-id="0599d-178">Specifies to restrict peer selection to a specfic source.</span></span>
<span data-ttu-id="0599d-179">此策略中设置的选项仅适用于传递优化模式组 (2) 下载模式。</span><span class="sxs-lookup"><span data-stu-id="0599d-179">The options set in this policy only apply to Delivery Optimization mode Group (2) download mode.</span></span> <span data-ttu-id="0599d-180">如果组 (2) 未设置为下载模式, 此策略将被忽略。</span><span class="sxs-lookup"><span data-stu-id="0599d-180">If Group (2) isn't set as Download mode, this policy will be ignored.</span></span> <span data-ttu-id="0599d-181">对于选项 3-dhcp 选项 id, 客户端将查询 DHCP 选项 id 234, 并使用返回的 GUID 值作为组 ID。</span><span class="sxs-lookup"><span data-stu-id="0599d-181">For option 3 - DHCP Option ID, the client will query DHCP Option ID 234 and use the returned GUID value as the Group ID.</span></span>|
|<span data-ttu-id="0599d-182">bandwidthMode</span><span class="sxs-lookup"><span data-stu-id="0599d-182">bandwidthMode</span></span>|[<span data-ttu-id="0599d-183">deliveryOptimizationBandwidth</span><span class="sxs-lookup"><span data-stu-id="0599d-183">deliveryOptimizationBandwidth</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|<span data-ttu-id="0599d-184">指定使用百分比、absolutes 或小时的前景色和背景带宽使用情况。</span><span class="sxs-lookup"><span data-stu-id="0599d-184">Specifies foreground and background bandwidth usage using percentages, absolutes, or hours.</span></span>|
|<span data-ttu-id="0599d-185">backgroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="0599d-185">backgroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="0599d-186">Int64</span><span class="sxs-lookup"><span data-stu-id="0599d-186">Int64</span></span>|<span data-ttu-id="0599d-187">指定允许使用对等的后台下载中的 HTTP 源延迟的秒数。</span><span class="sxs-lookup"><span data-stu-id="0599d-187">Specifies number of seconds to delay an HTTP source in a background download that is allowed to use peer-to-peer.</span></span> <span data-ttu-id="0599d-188">有效值为0至4294967295</span><span class="sxs-lookup"><span data-stu-id="0599d-188">Valid values 0 to 4294967295</span></span>|
|<span data-ttu-id="0599d-189">foregroundDownloadFromHttpDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="0599d-189">foregroundDownloadFromHttpDelayInSeconds</span></span>|<span data-ttu-id="0599d-190">Int64</span><span class="sxs-lookup"><span data-stu-id="0599d-190">Int64</span></span>|<span data-ttu-id="0599d-191">指定在允许使用对等 (0-86400) 的前台下载中延迟 HTTP 源的秒数。</span><span class="sxs-lookup"><span data-stu-id="0599d-191">Specifies number of seconds to delay an HTTP source in a foreground download that is allowed to use peer-to-peer (0-86400).</span></span> <span data-ttu-id="0599d-192">有效值为0至86400</span><span class="sxs-lookup"><span data-stu-id="0599d-192">Valid values 0 to 86400</span></span>
<span data-ttu-id="0599d-193">指定0将传递优化设置为使用云服务管理此设置。</span><span class="sxs-lookup"><span data-stu-id="0599d-193">Specifying 0 sets Delivery Optimization to manage this setting using the cloud service.</span></span> <span data-ttu-id="0599d-194">有效值为0至86400</span><span class="sxs-lookup"><span data-stu-id="0599d-194">Valid values 0 to 86400</span></span>|
|<span data-ttu-id="0599d-195">minimumRamAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="0599d-195">minimumRamAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="0599d-196">Int32</span><span class="sxs-lookup"><span data-stu-id="0599d-196">Int32</span></span>|<span data-ttu-id="0599d-197">指定使用对等缓存的最小 RAM 大小 (以 GB 为单位) (1-100000)。</span><span class="sxs-lookup"><span data-stu-id="0599d-197">Specifies the minimum RAM size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="0599d-198">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="0599d-198">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="0599d-199">minimumDiskSizeAllowedToPeerInGigabytes</span><span class="sxs-lookup"><span data-stu-id="0599d-199">minimumDiskSizeAllowedToPeerInGigabytes</span></span>|<span data-ttu-id="0599d-200">Int32</span><span class="sxs-lookup"><span data-stu-id="0599d-200">Int32</span></span>|<span data-ttu-id="0599d-201">指定使用对等缓存的最小磁盘大小 (以 GB 为单位) (1-100000)。</span><span class="sxs-lookup"><span data-stu-id="0599d-201">Specifies the minimum disk size in GB to use Peer Caching (1-100000).</span></span> <span data-ttu-id="0599d-202">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="0599d-202">Valid values 1 to 100000</span></span>
<span data-ttu-id="0599d-203">建议值:64 gb 到 256 gb。</span><span class="sxs-lookup"><span data-stu-id="0599d-203">Recommended values: 64 GB to 256 GB.</span></span> <span data-ttu-id="0599d-204">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="0599d-204">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="0599d-205">minimumFileSizeToCacheInMegabytes</span><span class="sxs-lookup"><span data-stu-id="0599d-205">minimumFileSizeToCacheInMegabytes</span></span>|<span data-ttu-id="0599d-206">Int32</span><span class="sxs-lookup"><span data-stu-id="0599d-206">Int32</span></span>|<span data-ttu-id="0599d-207">指定启用以使用对等缓存 (1-100000) 的最小内容文件大小 (以 MB 为单位)。</span><span class="sxs-lookup"><span data-stu-id="0599d-207">Specifies the minimum content file size in MB enabled to use Peer Caching (1-100000).</span></span> <span data-ttu-id="0599d-208">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="0599d-208">Valid values 1 to 100000</span></span>
<span data-ttu-id="0599d-209">推荐值: 1 mb 到 100000 MB。</span><span class="sxs-lookup"><span data-stu-id="0599d-209">Recommended values: 1 MB to 100,000 MB.</span></span> <span data-ttu-id="0599d-210">有效值为1至100000</span><span class="sxs-lookup"><span data-stu-id="0599d-210">Valid values 1 to 100000</span></span>|
|<span data-ttu-id="0599d-211">minimumBatteryPercentageAllowedToUpload</span><span class="sxs-lookup"><span data-stu-id="0599d-211">minimumBatteryPercentageAllowedToUpload</span></span>|<span data-ttu-id="0599d-212">Int32</span><span class="sxs-lookup"><span data-stu-id="0599d-212">Int32</span></span>|<span data-ttu-id="0599d-213">指定允许设备上传数据的最小电池百分比 (0-100)。</span><span class="sxs-lookup"><span data-stu-id="0599d-213">Specifies the minimum battery percentage to allow the device to upload data (0-100).</span></span> <span data-ttu-id="0599d-214">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="0599d-214">Valid values 0 to 100</span></span>
<span data-ttu-id="0599d-215">默认值为 0。</span><span class="sxs-lookup"><span data-stu-id="0599d-215">The default value is 0.</span></span> <span data-ttu-id="0599d-216">值为 0 (零) 表示 "不受限制", 将使用云服务默认值。</span><span class="sxs-lookup"><span data-stu-id="0599d-216">The value 0 (zero) means "not limited" and the cloud service default value will be used.</span></span> <span data-ttu-id="0599d-217">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="0599d-217">Valid values 0 to 100</span></span>|
|<span data-ttu-id="0599d-218">modifyCacheLocation</span><span class="sxs-lookup"><span data-stu-id="0599d-218">modifyCacheLocation</span></span>|<span data-ttu-id="0599d-219">String</span><span class="sxs-lookup"><span data-stu-id="0599d-219">String</span></span>|<span data-ttu-id="0599d-220">指定传递优化应用于其缓存的驱动器。</span><span class="sxs-lookup"><span data-stu-id="0599d-220">Specifies the drive that Delivery Optimization should use for its cache.</span></span>|
|<span data-ttu-id="0599d-221">maximumCacheAgeInDays</span><span class="sxs-lookup"><span data-stu-id="0599d-221">maximumCacheAgeInDays</span></span>|<span data-ttu-id="0599d-222">Int32</span><span class="sxs-lookup"><span data-stu-id="0599d-222">Int32</span></span>|<span data-ttu-id="0599d-223">指定在成功下载后, 每个文件保留在传递优化缓存中的最长时间 (以天为单位) (0-49710)。</span><span class="sxs-lookup"><span data-stu-id="0599d-223">Specifies the maximum time in days that each file is held in the Delivery Optimization cache after downloading successfully (0-49710).</span></span> <span data-ttu-id="0599d-224">有效值为0至49710</span><span class="sxs-lookup"><span data-stu-id="0599d-224">Valid values 0 to 49710</span></span>|
|<span data-ttu-id="0599d-225">maximumCacheSize</span><span class="sxs-lookup"><span data-stu-id="0599d-225">maximumCacheSize</span></span>|[<span data-ttu-id="0599d-226">deliveryOptimizationMaxCacheSize</span><span class="sxs-lookup"><span data-stu-id="0599d-226">deliveryOptimizationMaxCacheSize</span></span>](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|<span data-ttu-id="0599d-227">指定传递优化的最大缓存大小 (以百分比或 GB 为单位)。</span><span class="sxs-lookup"><span data-stu-id="0599d-227">Specifies the maximum cache size that Delivery Optimization either as a percentage or in GB.</span></span>|
|<span data-ttu-id="0599d-228">vpnPeerCaching</span><span class="sxs-lookup"><span data-stu-id="0599d-228">vpnPeerCaching</span></span>|[<span data-ttu-id="0599d-229">启用</span><span class="sxs-lookup"><span data-stu-id="0599d-229">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0599d-230">指定是否允许设备在通过 VPN 连接到域网络时参与对等缓存。</span><span class="sxs-lookup"><span data-stu-id="0599d-230">Specifies whether the device is allowed to participate in Peer Caching while connected via VPN to the domain network.</span></span> <span data-ttu-id="0599d-231">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="0599d-231">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="0599d-232">响应</span><span class="sxs-lookup"><span data-stu-id="0599d-232">Response</span></span>
<span data-ttu-id="0599d-233">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0599d-233">If successful, this method returns a `200 OK` response code and an updated [windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0599d-234">示例</span><span class="sxs-lookup"><span data-stu-id="0599d-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="0599d-235">请求</span><span class="sxs-lookup"><span data-stu-id="0599d-235">Request</span></span>
<span data-ttu-id="0599d-236">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0599d-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1060

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="0599d-237">响应</span><span class="sxs-lookup"><span data-stu-id="0599d-237">Response</span></span>
<span data-ttu-id="0599d-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0599d-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1232

{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
  "id": "5954ee9b-ee9b-5954-9bee-54599bee5459",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




