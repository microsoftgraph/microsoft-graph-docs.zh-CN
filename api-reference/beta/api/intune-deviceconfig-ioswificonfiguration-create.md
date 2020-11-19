---
title: 创建 iosWiFiConfiguration
description: 创建新的 iosWiFiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6e9836a50ed08b8a9b365d03146a42a73f5ea6c4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49220229"
---
# <a name="create-ioswificonfiguration"></a><span data-ttu-id="9f474-103">创建 iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f474-103">Create iosWiFiConfiguration</span></span>

<span data-ttu-id="9f474-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f474-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f474-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9f474-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f474-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f474-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f474-107">创建新的 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f474-107">Create a new [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f474-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f474-108">Prerequisites</span></span>
<span data-ttu-id="9f474-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f474-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f474-111">Permission type</span></span>|<span data-ttu-id="9f474-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f474-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f474-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f474-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f474-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f474-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f474-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f474-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f474-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f474-116">Not supported.</span></span>|
|<span data-ttu-id="9f474-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f474-117">Application</span></span>|<span data-ttu-id="9f474-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f474-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f474-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f474-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9f474-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f474-120">Request headers</span></span>
|<span data-ttu-id="9f474-121">标头</span><span class="sxs-lookup"><span data-stu-id="9f474-121">Header</span></span>|<span data-ttu-id="9f474-122">值</span><span class="sxs-lookup"><span data-stu-id="9f474-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f474-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f474-123">Authorization</span></span>|<span data-ttu-id="9f474-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f474-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f474-125">接受</span><span class="sxs-lookup"><span data-stu-id="9f474-125">Accept</span></span>|<span data-ttu-id="9f474-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f474-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f474-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f474-127">Request body</span></span>
<span data-ttu-id="9f474-128">在请求正文中，提供 iosWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f474-128">In the request body, supply a JSON representation for the iosWiFiConfiguration object.</span></span>

<span data-ttu-id="9f474-129">下表显示创建 iosWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f474-129">The following table shows the properties that are required when you create the iosWiFiConfiguration.</span></span>

|<span data-ttu-id="9f474-130">属性</span><span class="sxs-lookup"><span data-stu-id="9f474-130">Property</span></span>|<span data-ttu-id="9f474-131">类型</span><span class="sxs-lookup"><span data-stu-id="9f474-131">Type</span></span>|<span data-ttu-id="9f474-132">说明</span><span class="sxs-lookup"><span data-stu-id="9f474-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f474-133">id</span><span class="sxs-lookup"><span data-stu-id="9f474-133">id</span></span>|<span data-ttu-id="9f474-134">String</span><span class="sxs-lookup"><span data-stu-id="9f474-134">String</span></span>|<span data-ttu-id="9f474-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9f474-135">Key of the entity.</span></span> <span data-ttu-id="9f474-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f474-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9f474-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f474-138">DateTimeOffset</span></span>|<span data-ttu-id="9f474-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9f474-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9f474-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f474-141">roleScopeTagIds</span></span>|<span data-ttu-id="9f474-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="9f474-142">String collection</span></span>|<span data-ttu-id="9f474-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9f474-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9f474-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9f474-145">supportsScopeTags</span></span>|<span data-ttu-id="9f474-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f474-146">Boolean</span></span>|<span data-ttu-id="9f474-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9f474-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9f474-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9f474-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9f474-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9f474-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9f474-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9f474-150">This property is read-only.</span></span> <span data-ttu-id="9f474-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f474-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9f474-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f474-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9f474-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9f474-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9f474-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f474-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9f474-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f474-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9f474-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9f474-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9f474-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f474-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9f474-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f474-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9f474-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9f474-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9f474-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f474-164">createdDateTime</span></span>|<span data-ttu-id="9f474-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f474-165">DateTimeOffset</span></span>|<span data-ttu-id="9f474-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9f474-166">DateTime the object was created.</span></span> <span data-ttu-id="9f474-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-168">description</span><span class="sxs-lookup"><span data-stu-id="9f474-168">description</span></span>|<span data-ttu-id="9f474-169">String</span><span class="sxs-lookup"><span data-stu-id="9f474-169">String</span></span>|<span data-ttu-id="9f474-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9f474-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f474-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9f474-172">displayName</span></span>|<span data-ttu-id="9f474-173">String</span><span class="sxs-lookup"><span data-stu-id="9f474-173">String</span></span>|<span data-ttu-id="9f474-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9f474-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f474-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-176">version</span><span class="sxs-lookup"><span data-stu-id="9f474-176">version</span></span>|<span data-ttu-id="9f474-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9f474-177">Int32</span></span>|<span data-ttu-id="9f474-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9f474-178">Version of the device configuration.</span></span> <span data-ttu-id="9f474-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f474-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f474-180">networkName</span><span class="sxs-lookup"><span data-stu-id="9f474-180">networkName</span></span>|<span data-ttu-id="9f474-181">String</span><span class="sxs-lookup"><span data-stu-id="9f474-181">String</span></span>|<span data-ttu-id="9f474-182">网络名称</span><span class="sxs-lookup"><span data-stu-id="9f474-182">Network Name</span></span>|
|<span data-ttu-id="9f474-183">ssid</span><span class="sxs-lookup"><span data-stu-id="9f474-183">ssid</span></span>|<span data-ttu-id="9f474-184">String</span><span class="sxs-lookup"><span data-stu-id="9f474-184">String</span></span>|<span data-ttu-id="9f474-185">这是广播到所有设备的 Wi-Fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="9f474-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="9f474-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="9f474-186">connectAutomatically</span></span>|<span data-ttu-id="9f474-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f474-187">Boolean</span></span>|<span data-ttu-id="9f474-188">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="9f474-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="9f474-189">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="9f474-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="9f474-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9f474-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9f474-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f474-191">Boolean</span></span>|<span data-ttu-id="9f474-192">网络未广播其名称 (SSID) 时连接。</span><span class="sxs-lookup"><span data-stu-id="9f474-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="9f474-193">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="9f474-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="9f474-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9f474-194">wiFiSecurityType</span></span>|[<span data-ttu-id="9f474-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9f474-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="9f474-196">指示 Wi-Fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="9f474-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="9f474-197">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="9f474-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="9f474-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="9f474-198">proxySettings</span></span>|[<span data-ttu-id="9f474-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="9f474-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="9f474-200">此 Wi-Fi 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="9f474-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="9f474-201">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="9f474-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="9f474-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="9f474-202">proxyManualAddress</span></span>|<span data-ttu-id="9f474-203">String</span><span class="sxs-lookup"><span data-stu-id="9f474-203">String</span></span>|<span data-ttu-id="9f474-204">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="9f474-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="9f474-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="9f474-205">proxyManualPort</span></span>|<span data-ttu-id="9f474-206">Int32</span><span class="sxs-lookup"><span data-stu-id="9f474-206">Int32</span></span>|<span data-ttu-id="9f474-207">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="9f474-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="9f474-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="9f474-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="9f474-209">String</span><span class="sxs-lookup"><span data-stu-id="9f474-209">String</span></span>|<span data-ttu-id="9f474-210">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="9f474-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="9f474-211">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="9f474-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="9f474-212">disableMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="9f474-212">disableMacAddressRandomization</span></span>|<span data-ttu-id="9f474-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f474-213">Boolean</span></span>|<span data-ttu-id="9f474-214">如果设置为 true，则强制设备使用此 Wi-Fi 配置文件进行连接，以提供实际 Wi-Fi MAC 地址，而不是随机 MAC 地址。</span><span class="sxs-lookup"><span data-stu-id="9f474-214">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="9f474-215">适用于 iOS 14 和更高版本。</span><span class="sxs-lookup"><span data-stu-id="9f474-215">Applies to iOS 14 and later.</span></span>|
|<span data-ttu-id="9f474-216">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="9f474-216">preSharedKey</span></span>|<span data-ttu-id="9f474-217">String</span><span class="sxs-lookup"><span data-stu-id="9f474-217">String</span></span>|<span data-ttu-id="9f474-218">这是 WPA 个人 Wi-Fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="9f474-218">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="9f474-219">响应</span><span class="sxs-lookup"><span data-stu-id="9f474-219">Response</span></span>
<span data-ttu-id="9f474-220">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f474-220">If successful, this method returns a `201 Created` response code and a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f474-221">示例</span><span class="sxs-lookup"><span data-stu-id="9f474-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f474-222">请求</span><span class="sxs-lookup"><span data-stu-id="9f474-222">Request</span></span>
<span data-ttu-id="9f474-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f474-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1491

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="9f474-224">响应</span><span class="sxs-lookup"><span data-stu-id="9f474-224">Response</span></span>
<span data-ttu-id="9f474-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f474-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1663

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value"
}
```




