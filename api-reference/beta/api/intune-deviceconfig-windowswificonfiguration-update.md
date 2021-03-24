---
title: 更新 windowsWifiConfiguration
description: 更新 windowsWifiConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adae47a270925418333b2ad30700680fcbaf912e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127184"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="86310-103">更新 windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="86310-103">Update windowsWifiConfiguration</span></span>

<span data-ttu-id="86310-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86310-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86310-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86310-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86310-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86310-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86310-107">更新 [windowsWifiConfiguration 对象](../resources/intune-deviceconfig-windowswificonfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="86310-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86310-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="86310-108">Prerequisites</span></span>
<span data-ttu-id="86310-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86310-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="86310-111">Permission type</span></span>|<span data-ttu-id="86310-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86310-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86310-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86310-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86310-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86310-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86310-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86310-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86310-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86310-116">Not supported.</span></span>|
|<span data-ttu-id="86310-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="86310-117">Application</span></span>|<span data-ttu-id="86310-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86310-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86310-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86310-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="86310-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="86310-120">Request headers</span></span>
|<span data-ttu-id="86310-121">标头</span><span class="sxs-lookup"><span data-stu-id="86310-121">Header</span></span>|<span data-ttu-id="86310-122">值</span><span class="sxs-lookup"><span data-stu-id="86310-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86310-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="86310-123">Authorization</span></span>|<span data-ttu-id="86310-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86310-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86310-125">接受</span><span class="sxs-lookup"><span data-stu-id="86310-125">Accept</span></span>|<span data-ttu-id="86310-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86310-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86310-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86310-127">Request body</span></span>
<span data-ttu-id="86310-128">在请求正文中，提供 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86310-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="86310-129">下表显示创建 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86310-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="86310-130">属性</span><span class="sxs-lookup"><span data-stu-id="86310-130">Property</span></span>|<span data-ttu-id="86310-131">类型</span><span class="sxs-lookup"><span data-stu-id="86310-131">Type</span></span>|<span data-ttu-id="86310-132">说明</span><span class="sxs-lookup"><span data-stu-id="86310-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86310-133">id</span><span class="sxs-lookup"><span data-stu-id="86310-133">id</span></span>|<span data-ttu-id="86310-134">String</span><span class="sxs-lookup"><span data-stu-id="86310-134">String</span></span>|<span data-ttu-id="86310-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86310-135">Key of the entity.</span></span> <span data-ttu-id="86310-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86310-137">lastModifiedDateTime</span></span>|<span data-ttu-id="86310-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86310-138">DateTimeOffset</span></span>|<span data-ttu-id="86310-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86310-139">DateTime the object was last modified.</span></span> <span data-ttu-id="86310-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86310-141">roleScopeTagIds</span></span>|<span data-ttu-id="86310-142">String collection</span><span class="sxs-lookup"><span data-stu-id="86310-142">String collection</span></span>|<span data-ttu-id="86310-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="86310-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86310-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="86310-145">supportsScopeTags</span></span>|<span data-ttu-id="86310-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="86310-146">Boolean</span></span>|<span data-ttu-id="86310-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="86310-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86310-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="86310-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86310-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="86310-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86310-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="86310-150">This property is read-only.</span></span> <span data-ttu-id="86310-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86310-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="86310-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86310-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="86310-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="86310-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="86310-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86310-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="86310-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86310-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="86310-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="86310-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="86310-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86310-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="86310-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86310-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="86310-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="86310-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="86310-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86310-164">createdDateTime</span></span>|<span data-ttu-id="86310-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86310-165">DateTimeOffset</span></span>|<span data-ttu-id="86310-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="86310-166">DateTime the object was created.</span></span> <span data-ttu-id="86310-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-168">说明</span><span class="sxs-lookup"><span data-stu-id="86310-168">description</span></span>|<span data-ttu-id="86310-169">String</span><span class="sxs-lookup"><span data-stu-id="86310-169">String</span></span>|<span data-ttu-id="86310-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="86310-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86310-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-172">displayName</span><span class="sxs-lookup"><span data-stu-id="86310-172">displayName</span></span>|<span data-ttu-id="86310-173">String</span><span class="sxs-lookup"><span data-stu-id="86310-173">String</span></span>|<span data-ttu-id="86310-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="86310-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86310-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-176">version</span><span class="sxs-lookup"><span data-stu-id="86310-176">version</span></span>|<span data-ttu-id="86310-177">Int32</span><span class="sxs-lookup"><span data-stu-id="86310-177">Int32</span></span>|<span data-ttu-id="86310-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="86310-178">Version of the device configuration.</span></span> <span data-ttu-id="86310-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86310-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86310-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="86310-180">preSharedKey</span></span>|<span data-ttu-id="86310-181">String</span><span class="sxs-lookup"><span data-stu-id="86310-181">String</span></span>|<span data-ttu-id="86310-182">这是 WPA 个人共享网络的预共享Wi-Fi密钥。</span><span class="sxs-lookup"><span data-stu-id="86310-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="86310-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="86310-183">wifiSecurityType</span></span>|[<span data-ttu-id="86310-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="86310-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="86310-185">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="86310-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="86310-186">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="86310-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="86310-187">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="86310-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="86310-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="86310-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="86310-189">指定 wifi 连接的按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="86310-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="86310-190">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="86310-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="86310-191">ssid</span><span class="sxs-lookup"><span data-stu-id="86310-191">ssid</span></span>|<span data-ttu-id="86310-192">String</span><span class="sxs-lookup"><span data-stu-id="86310-192">String</span></span>|<span data-ttu-id="86310-193">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="86310-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="86310-194">networkName</span><span class="sxs-lookup"><span data-stu-id="86310-194">networkName</span></span>|<span data-ttu-id="86310-195">String</span><span class="sxs-lookup"><span data-stu-id="86310-195">String</span></span>|<span data-ttu-id="86310-196">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="86310-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="86310-197">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="86310-197">connectAutomatically</span></span>|<span data-ttu-id="86310-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="86310-198">Boolean</span></span>|<span data-ttu-id="86310-199">指定 wifi 连接是否在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="86310-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="86310-200">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="86310-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="86310-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="86310-201">Boolean</span></span>|<span data-ttu-id="86310-202">指定 wifi 连接在已连接到此网络时是否应该连接到更首选的网络。</span><span class="sxs-lookup"><span data-stu-id="86310-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="86310-203">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="86310-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="86310-204">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="86310-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="86310-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="86310-205">Boolean</span></span>|<span data-ttu-id="86310-206">指定即使在 SSID 未广播时 wifi 连接是否应该自动连接。</span><span class="sxs-lookup"><span data-stu-id="86310-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="86310-207">proxySetting</span><span class="sxs-lookup"><span data-stu-id="86310-207">proxySetting</span></span>|[<span data-ttu-id="86310-208">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="86310-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="86310-209">为配置指定Wi-Fi设置。</span><span class="sxs-lookup"><span data-stu-id="86310-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="86310-210">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="86310-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="86310-211">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="86310-211">proxyManualAddress</span></span>|<span data-ttu-id="86310-212">String</span><span class="sxs-lookup"><span data-stu-id="86310-212">String</span></span>|<span data-ttu-id="86310-213">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="86310-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="86310-214">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="86310-214">proxyManualPort</span></span>|<span data-ttu-id="86310-215">Int32</span><span class="sxs-lookup"><span data-stu-id="86310-215">Int32</span></span>|<span data-ttu-id="86310-216">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="86310-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="86310-217">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="86310-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="86310-218">String</span><span class="sxs-lookup"><span data-stu-id="86310-218">String</span></span>|<span data-ttu-id="86310-219">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="86310-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="86310-220">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="86310-220">forceFIPSCompliance</span></span>|<span data-ttu-id="86310-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="86310-221">Boolean</span></span>|<span data-ttu-id="86310-222">指定是否强制 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="86310-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="86310-223">响应</span><span class="sxs-lookup"><span data-stu-id="86310-223">Response</span></span>
<span data-ttu-id="86310-224">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86310-224">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86310-225">示例</span><span class="sxs-lookup"><span data-stu-id="86310-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="86310-226">请求</span><span class="sxs-lookup"><span data-stu-id="86310-226">Request</span></span>
<span data-ttu-id="86310-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86310-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="86310-228">响应</span><span class="sxs-lookup"><span data-stu-id="86310-228">Response</span></span>
<span data-ttu-id="86310-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86310-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1731

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```




