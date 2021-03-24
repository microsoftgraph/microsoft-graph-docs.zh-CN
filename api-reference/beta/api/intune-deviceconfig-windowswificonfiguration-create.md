---
title: 创建 windowsWifiConfiguration
description: 创建新的 windowsWifiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82b784c82d66c684ac0afac32e9bf490fc26aaaf
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131034"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="bb36e-103">创建 windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb36e-103">Create windowsWifiConfiguration</span></span>

<span data-ttu-id="bb36e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb36e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb36e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb36e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb36e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb36e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb36e-107">创建新的 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb36e-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb36e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb36e-108">Prerequisites</span></span>
<span data-ttu-id="bb36e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb36e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb36e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb36e-111">Permission type</span></span>|<span data-ttu-id="bb36e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb36e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb36e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb36e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb36e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb36e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb36e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb36e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb36e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb36e-116">Not supported.</span></span>|
|<span data-ttu-id="bb36e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb36e-117">Application</span></span>|<span data-ttu-id="bb36e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb36e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb36e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb36e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bb36e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb36e-120">Request headers</span></span>
|<span data-ttu-id="bb36e-121">标头</span><span class="sxs-lookup"><span data-stu-id="bb36e-121">Header</span></span>|<span data-ttu-id="bb36e-122">值</span><span class="sxs-lookup"><span data-stu-id="bb36e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb36e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb36e-123">Authorization</span></span>|<span data-ttu-id="bb36e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb36e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb36e-125">接受</span><span class="sxs-lookup"><span data-stu-id="bb36e-125">Accept</span></span>|<span data-ttu-id="bb36e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb36e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb36e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb36e-127">Request body</span></span>
<span data-ttu-id="bb36e-128">在请求正文中，提供 windowsWifiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb36e-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="bb36e-129">下表显示创建 windowsWifiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bb36e-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="bb36e-130">属性</span><span class="sxs-lookup"><span data-stu-id="bb36e-130">Property</span></span>|<span data-ttu-id="bb36e-131">类型</span><span class="sxs-lookup"><span data-stu-id="bb36e-131">Type</span></span>|<span data-ttu-id="bb36e-132">说明</span><span class="sxs-lookup"><span data-stu-id="bb36e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb36e-133">id</span><span class="sxs-lookup"><span data-stu-id="bb36e-133">id</span></span>|<span data-ttu-id="bb36e-134">String</span><span class="sxs-lookup"><span data-stu-id="bb36e-134">String</span></span>|<span data-ttu-id="bb36e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bb36e-135">Key of the entity.</span></span> <span data-ttu-id="bb36e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb36e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bb36e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb36e-138">DateTimeOffset</span></span>|<span data-ttu-id="bb36e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bb36e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bb36e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb36e-141">roleScopeTagIds</span></span>|<span data-ttu-id="bb36e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="bb36e-142">String collection</span></span>|<span data-ttu-id="bb36e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="bb36e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb36e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bb36e-145">supportsScopeTags</span></span>|<span data-ttu-id="bb36e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb36e-146">Boolean</span></span>|<span data-ttu-id="bb36e-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="bb36e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bb36e-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="bb36e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bb36e-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="bb36e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bb36e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="bb36e-150">This property is read-only.</span></span> <span data-ttu-id="bb36e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb36e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bb36e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb36e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bb36e-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="bb36e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bb36e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb36e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bb36e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb36e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bb36e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bb36e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bb36e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb36e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bb36e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb36e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bb36e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="bb36e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bb36e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb36e-164">createdDateTime</span></span>|<span data-ttu-id="bb36e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb36e-165">DateTimeOffset</span></span>|<span data-ttu-id="bb36e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="bb36e-166">DateTime the object was created.</span></span> <span data-ttu-id="bb36e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-168">说明</span><span class="sxs-lookup"><span data-stu-id="bb36e-168">description</span></span>|<span data-ttu-id="bb36e-169">String</span><span class="sxs-lookup"><span data-stu-id="bb36e-169">String</span></span>|<span data-ttu-id="bb36e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="bb36e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb36e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bb36e-172">displayName</span></span>|<span data-ttu-id="bb36e-173">String</span><span class="sxs-lookup"><span data-stu-id="bb36e-173">String</span></span>|<span data-ttu-id="bb36e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="bb36e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb36e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-176">version</span><span class="sxs-lookup"><span data-stu-id="bb36e-176">version</span></span>|<span data-ttu-id="bb36e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bb36e-177">Int32</span></span>|<span data-ttu-id="bb36e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="bb36e-178">Version of the device configuration.</span></span> <span data-ttu-id="bb36e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb36e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb36e-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="bb36e-180">preSharedKey</span></span>|<span data-ttu-id="bb36e-181">String</span><span class="sxs-lookup"><span data-stu-id="bb36e-181">String</span></span>|<span data-ttu-id="bb36e-182">这是 WPA 个人共享网络的预共享Wi-Fi密钥。</span><span class="sxs-lookup"><span data-stu-id="bb36e-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="bb36e-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="bb36e-183">wifiSecurityType</span></span>|[<span data-ttu-id="bb36e-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="bb36e-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="bb36e-185">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="bb36e-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="bb36e-186">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="bb36e-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="bb36e-187">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="bb36e-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="bb36e-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="bb36e-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="bb36e-189">指定 wifi 连接的按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="bb36e-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="bb36e-190">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="bb36e-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="bb36e-191">ssid</span><span class="sxs-lookup"><span data-stu-id="bb36e-191">ssid</span></span>|<span data-ttu-id="bb36e-192">String</span><span class="sxs-lookup"><span data-stu-id="bb36e-192">String</span></span>|<span data-ttu-id="bb36e-193">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="bb36e-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="bb36e-194">networkName</span><span class="sxs-lookup"><span data-stu-id="bb36e-194">networkName</span></span>|<span data-ttu-id="bb36e-195">String</span><span class="sxs-lookup"><span data-stu-id="bb36e-195">String</span></span>|<span data-ttu-id="bb36e-196">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="bb36e-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="bb36e-197">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="bb36e-197">connectAutomatically</span></span>|<span data-ttu-id="bb36e-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb36e-198">Boolean</span></span>|<span data-ttu-id="bb36e-199">指定 wifi 连接是否在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="bb36e-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="bb36e-200">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="bb36e-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="bb36e-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb36e-201">Boolean</span></span>|<span data-ttu-id="bb36e-202">指定 wifi 连接在已连接到此网络时是否应该连接到更首选的网络。</span><span class="sxs-lookup"><span data-stu-id="bb36e-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="bb36e-203">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="bb36e-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="bb36e-204">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="bb36e-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="bb36e-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb36e-205">Boolean</span></span>|<span data-ttu-id="bb36e-206">指定即使在 SSID 未广播时 wifi 连接是否应该自动连接。</span><span class="sxs-lookup"><span data-stu-id="bb36e-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="bb36e-207">proxySetting</span><span class="sxs-lookup"><span data-stu-id="bb36e-207">proxySetting</span></span>|[<span data-ttu-id="bb36e-208">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="bb36e-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="bb36e-209">为配置指定Wi-Fi设置。</span><span class="sxs-lookup"><span data-stu-id="bb36e-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="bb36e-210">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="bb36e-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="bb36e-211">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="bb36e-211">proxyManualAddress</span></span>|<span data-ttu-id="bb36e-212">String</span><span class="sxs-lookup"><span data-stu-id="bb36e-212">String</span></span>|<span data-ttu-id="bb36e-213">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="bb36e-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="bb36e-214">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="bb36e-214">proxyManualPort</span></span>|<span data-ttu-id="bb36e-215">Int32</span><span class="sxs-lookup"><span data-stu-id="bb36e-215">Int32</span></span>|<span data-ttu-id="bb36e-216">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="bb36e-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="bb36e-217">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="bb36e-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="bb36e-218">String</span><span class="sxs-lookup"><span data-stu-id="bb36e-218">String</span></span>|<span data-ttu-id="bb36e-219">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="bb36e-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="bb36e-220">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="bb36e-220">forceFIPSCompliance</span></span>|<span data-ttu-id="bb36e-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb36e-221">Boolean</span></span>|<span data-ttu-id="bb36e-222">指定是否强制 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="bb36e-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="bb36e-223">响应</span><span class="sxs-lookup"><span data-stu-id="bb36e-223">Response</span></span>
<span data-ttu-id="bb36e-224">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb36e-224">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb36e-225">示例</span><span class="sxs-lookup"><span data-stu-id="bb36e-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb36e-226">请求</span><span class="sxs-lookup"><span data-stu-id="bb36e-226">Request</span></span>
<span data-ttu-id="bb36e-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb36e-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="bb36e-228">响应</span><span class="sxs-lookup"><span data-stu-id="bb36e-228">Response</span></span>
<span data-ttu-id="bb36e-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb36e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




