---
title: 创建 windowsWifiConfiguration
description: 创建新的 windowsWifiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6c945a6e8b88e482311d49a231c6888fcc5204ce
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43332753"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="18d07-103">创建 windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="18d07-103">Create windowsWifiConfiguration</span></span>

<span data-ttu-id="18d07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18d07-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18d07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18d07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18d07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d07-107">创建新的[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="18d07-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18d07-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="18d07-108">Prerequisites</span></span>
<span data-ttu-id="18d07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18d07-111">Permission type</span></span>|<span data-ttu-id="18d07-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18d07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18d07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18d07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18d07-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d07-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18d07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18d07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18d07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18d07-116">Not supported.</span></span>|
|<span data-ttu-id="18d07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18d07-117">Application</span></span>|<span data-ttu-id="18d07-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d07-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18d07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18d07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18d07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18d07-120">Request headers</span></span>
|<span data-ttu-id="18d07-121">标头</span><span class="sxs-lookup"><span data-stu-id="18d07-121">Header</span></span>|<span data-ttu-id="18d07-122">值</span><span class="sxs-lookup"><span data-stu-id="18d07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18d07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18d07-123">Authorization</span></span>|<span data-ttu-id="18d07-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18d07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18d07-125">接受</span><span class="sxs-lookup"><span data-stu-id="18d07-125">Accept</span></span>|<span data-ttu-id="18d07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18d07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18d07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18d07-127">Request body</span></span>
<span data-ttu-id="18d07-128">在请求正文中，提供 windowsWifiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18d07-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="18d07-129">下表显示创建 windowsWifiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="18d07-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="18d07-130">属性</span><span class="sxs-lookup"><span data-stu-id="18d07-130">Property</span></span>|<span data-ttu-id="18d07-131">类型</span><span class="sxs-lookup"><span data-stu-id="18d07-131">Type</span></span>|<span data-ttu-id="18d07-132">说明</span><span class="sxs-lookup"><span data-stu-id="18d07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d07-133">id</span><span class="sxs-lookup"><span data-stu-id="18d07-133">id</span></span>|<span data-ttu-id="18d07-134">字符串</span><span class="sxs-lookup"><span data-stu-id="18d07-134">String</span></span>|<span data-ttu-id="18d07-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="18d07-135">Key of the entity.</span></span> <span data-ttu-id="18d07-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18d07-137">lastModifiedDateTime</span></span>|<span data-ttu-id="18d07-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d07-138">DateTimeOffset</span></span>|<span data-ttu-id="18d07-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="18d07-139">DateTime the object was last modified.</span></span> <span data-ttu-id="18d07-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18d07-141">roleScopeTagIds</span></span>|<span data-ttu-id="18d07-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="18d07-142">String collection</span></span>|<span data-ttu-id="18d07-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="18d07-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18d07-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="18d07-145">supportsScopeTags</span></span>|<span data-ttu-id="18d07-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="18d07-146">Boolean</span></span>|<span data-ttu-id="18d07-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="18d07-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="18d07-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="18d07-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="18d07-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="18d07-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="18d07-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="18d07-150">This property is read-only.</span></span> <span data-ttu-id="18d07-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18d07-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="18d07-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18d07-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="18d07-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="18d07-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="18d07-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18d07-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="18d07-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18d07-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="18d07-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="18d07-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="18d07-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18d07-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="18d07-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18d07-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="18d07-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="18d07-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="18d07-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18d07-164">createdDateTime</span></span>|<span data-ttu-id="18d07-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18d07-165">DateTimeOffset</span></span>|<span data-ttu-id="18d07-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="18d07-166">DateTime the object was created.</span></span> <span data-ttu-id="18d07-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-168">description</span><span class="sxs-lookup"><span data-stu-id="18d07-168">description</span></span>|<span data-ttu-id="18d07-169">String</span><span class="sxs-lookup"><span data-stu-id="18d07-169">String</span></span>|<span data-ttu-id="18d07-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="18d07-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18d07-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-172">displayName</span><span class="sxs-lookup"><span data-stu-id="18d07-172">displayName</span></span>|<span data-ttu-id="18d07-173">String</span><span class="sxs-lookup"><span data-stu-id="18d07-173">String</span></span>|<span data-ttu-id="18d07-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="18d07-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18d07-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-176">version</span><span class="sxs-lookup"><span data-stu-id="18d07-176">version</span></span>|<span data-ttu-id="18d07-177">Int32</span><span class="sxs-lookup"><span data-stu-id="18d07-177">Int32</span></span>|<span data-ttu-id="18d07-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="18d07-178">Version of the device configuration.</span></span> <span data-ttu-id="18d07-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18d07-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18d07-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="18d07-180">preSharedKey</span></span>|<span data-ttu-id="18d07-181">字符串</span><span class="sxs-lookup"><span data-stu-id="18d07-181">String</span></span>|<span data-ttu-id="18d07-182">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="18d07-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="18d07-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="18d07-183">wifiSecurityType</span></span>|[<span data-ttu-id="18d07-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="18d07-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="18d07-185">指定 Wifi 安全类型。</span><span class="sxs-lookup"><span data-stu-id="18d07-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="18d07-186">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="18d07-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="18d07-187">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="18d07-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="18d07-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="18d07-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="18d07-189">为 wifi 连接指定按流量计费的连接限制类型。</span><span class="sxs-lookup"><span data-stu-id="18d07-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="18d07-190">可取值为：`unrestricted`、`fixed`、`variable`。</span><span class="sxs-lookup"><span data-stu-id="18d07-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="18d07-191">ssid</span><span class="sxs-lookup"><span data-stu-id="18d07-191">ssid</span></span>|<span data-ttu-id="18d07-192">字符串</span><span class="sxs-lookup"><span data-stu-id="18d07-192">String</span></span>|<span data-ttu-id="18d07-193">指定 wifi 连接的 SSID。</span><span class="sxs-lookup"><span data-stu-id="18d07-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="18d07-194">networkName</span><span class="sxs-lookup"><span data-stu-id="18d07-194">networkName</span></span>|<span data-ttu-id="18d07-195">字符串</span><span class="sxs-lookup"><span data-stu-id="18d07-195">String</span></span>|<span data-ttu-id="18d07-196">指定网络配置名称。</span><span class="sxs-lookup"><span data-stu-id="18d07-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="18d07-197">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="18d07-197">connectAutomatically</span></span>|<span data-ttu-id="18d07-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="18d07-198">Boolean</span></span>|<span data-ttu-id="18d07-199">指定是否在范围内自动连接 wifi 连接。</span><span class="sxs-lookup"><span data-stu-id="18d07-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="18d07-200">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="18d07-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="18d07-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="18d07-201">Boolean</span></span>|<span data-ttu-id="18d07-202">指定 wifi 连接是否应连接到更多的首选网络（如果已连接到此连接的话）。</span><span class="sxs-lookup"><span data-stu-id="18d07-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="18d07-203">要求 ConnectAutomatically 为 true。</span><span class="sxs-lookup"><span data-stu-id="18d07-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="18d07-204">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="18d07-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="18d07-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="18d07-205">Boolean</span></span>|<span data-ttu-id="18d07-206">指定是否应自动连接 wifi 连接，即使 SSID 未进行广播也是如此。</span><span class="sxs-lookup"><span data-stu-id="18d07-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="18d07-207">proxySetting</span><span class="sxs-lookup"><span data-stu-id="18d07-207">proxySetting</span></span>|[<span data-ttu-id="18d07-208">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="18d07-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="18d07-209">指定 Wlan 配置的代理设置。</span><span class="sxs-lookup"><span data-stu-id="18d07-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="18d07-210">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="18d07-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="18d07-211">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="18d07-211">proxyManualAddress</span></span>|<span data-ttu-id="18d07-212">字符串</span><span class="sxs-lookup"><span data-stu-id="18d07-212">String</span></span>|<span data-ttu-id="18d07-213">指定代理服务器的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="18d07-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="18d07-214">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="18d07-214">proxyManualPort</span></span>|<span data-ttu-id="18d07-215">Int32</span><span class="sxs-lookup"><span data-stu-id="18d07-215">Int32</span></span>|<span data-ttu-id="18d07-216">指定代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="18d07-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="18d07-217">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="18d07-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="18d07-218">字符串</span><span class="sxs-lookup"><span data-stu-id="18d07-218">String</span></span>|<span data-ttu-id="18d07-219">指定代理服务器配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="18d07-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="18d07-220">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="18d07-220">forceFIPSCompliance</span></span>|<span data-ttu-id="18d07-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="18d07-221">Boolean</span></span>|<span data-ttu-id="18d07-222">指定是否强制进行 FIPS 合规性。</span><span class="sxs-lookup"><span data-stu-id="18d07-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="18d07-223">响应</span><span class="sxs-lookup"><span data-stu-id="18d07-223">Response</span></span>
<span data-ttu-id="18d07-224">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="18d07-224">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18d07-225">示例</span><span class="sxs-lookup"><span data-stu-id="18d07-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="18d07-226">请求</span><span class="sxs-lookup"><span data-stu-id="18d07-226">Request</span></span>
<span data-ttu-id="18d07-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18d07-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18d07-228">响应</span><span class="sxs-lookup"><span data-stu-id="18d07-228">Response</span></span>
<span data-ttu-id="18d07-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18d07-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



