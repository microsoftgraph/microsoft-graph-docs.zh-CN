---
title: 创建 iosWiFiConfiguration
description: 创建新的 iosWiFiConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b02a524b6f94731833deef1c1ac69b59e90a208
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977028"
---
# <a name="create-ioswificonfiguration"></a><span data-ttu-id="de09a-103">创建 iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="de09a-103">Create iosWiFiConfiguration</span></span>

> <span data-ttu-id="de09a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="de09a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de09a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="de09a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de09a-106">创建新的[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de09a-106">Create a new [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de09a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="de09a-107">Prerequisites</span></span>
<span data-ttu-id="de09a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de09a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de09a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="de09a-110">Permission type</span></span>|<span data-ttu-id="de09a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de09a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de09a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de09a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de09a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de09a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de09a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de09a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de09a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="de09a-115">Not supported.</span></span>|
|<span data-ttu-id="de09a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="de09a-116">Application</span></span>|<span data-ttu-id="de09a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="de09a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de09a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de09a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="de09a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="de09a-119">Request headers</span></span>
|<span data-ttu-id="de09a-120">标头</span><span class="sxs-lookup"><span data-stu-id="de09a-120">Header</span></span>|<span data-ttu-id="de09a-121">值</span><span class="sxs-lookup"><span data-stu-id="de09a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de09a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="de09a-122">Authorization</span></span>|<span data-ttu-id="de09a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de09a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de09a-124">接受</span><span class="sxs-lookup"><span data-stu-id="de09a-124">Accept</span></span>|<span data-ttu-id="de09a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de09a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de09a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="de09a-126">Request body</span></span>
<span data-ttu-id="de09a-127">在请求正文中, 提供 iosWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de09a-127">In the request body, supply a JSON representation for the iosWiFiConfiguration object.</span></span>

<span data-ttu-id="de09a-128">下表显示创建 iosWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de09a-128">The following table shows the properties that are required when you create the iosWiFiConfiguration.</span></span>

|<span data-ttu-id="de09a-129">属性</span><span class="sxs-lookup"><span data-stu-id="de09a-129">Property</span></span>|<span data-ttu-id="de09a-130">类型</span><span class="sxs-lookup"><span data-stu-id="de09a-130">Type</span></span>|<span data-ttu-id="de09a-131">说明</span><span class="sxs-lookup"><span data-stu-id="de09a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de09a-132">id</span><span class="sxs-lookup"><span data-stu-id="de09a-132">id</span></span>|<span data-ttu-id="de09a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="de09a-133">String</span></span>|<span data-ttu-id="de09a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="de09a-134">Key of the entity.</span></span> <span data-ttu-id="de09a-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de09a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="de09a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de09a-137">DateTimeOffset</span></span>|<span data-ttu-id="de09a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="de09a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="de09a-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de09a-140">roleScopeTagIds</span></span>|<span data-ttu-id="de09a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="de09a-141">String collection</span></span>|<span data-ttu-id="de09a-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="de09a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="de09a-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="de09a-144">supportsScopeTags</span></span>|<span data-ttu-id="de09a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="de09a-145">Boolean</span></span>|<span data-ttu-id="de09a-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="de09a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="de09a-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="de09a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="de09a-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="de09a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="de09a-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="de09a-149">This property is read-only.</span></span> <span data-ttu-id="de09a-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="de09a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="de09a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="de09a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="de09a-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="de09a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="de09a-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="de09a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="de09a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="de09a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="de09a-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="de09a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="de09a-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="de09a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="de09a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="de09a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="de09a-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="de09a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="de09a-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de09a-163">createdDateTime</span></span>|<span data-ttu-id="de09a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de09a-164">DateTimeOffset</span></span>|<span data-ttu-id="de09a-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="de09a-165">DateTime the object was created.</span></span> <span data-ttu-id="de09a-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-167">说明</span><span class="sxs-lookup"><span data-stu-id="de09a-167">description</span></span>|<span data-ttu-id="de09a-168">String</span><span class="sxs-lookup"><span data-stu-id="de09a-168">String</span></span>|<span data-ttu-id="de09a-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="de09a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de09a-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="de09a-171">displayName</span></span>|<span data-ttu-id="de09a-172">String</span><span class="sxs-lookup"><span data-stu-id="de09a-172">String</span></span>|<span data-ttu-id="de09a-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="de09a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de09a-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-175">version</span><span class="sxs-lookup"><span data-stu-id="de09a-175">version</span></span>|<span data-ttu-id="de09a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="de09a-176">Int32</span></span>|<span data-ttu-id="de09a-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="de09a-177">Version of the device configuration.</span></span> <span data-ttu-id="de09a-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de09a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de09a-179">networkName</span><span class="sxs-lookup"><span data-stu-id="de09a-179">networkName</span></span>|<span data-ttu-id="de09a-180">String</span><span class="sxs-lookup"><span data-stu-id="de09a-180">String</span></span>|<span data-ttu-id="de09a-181">网络名称</span><span class="sxs-lookup"><span data-stu-id="de09a-181">Network Name</span></span>|
|<span data-ttu-id="de09a-182">ssid</span><span class="sxs-lookup"><span data-stu-id="de09a-182">ssid</span></span>|<span data-ttu-id="de09a-183">String</span><span class="sxs-lookup"><span data-stu-id="de09a-183">String</span></span>|<span data-ttu-id="de09a-184">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="de09a-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="de09a-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="de09a-185">connectAutomatically</span></span>|<span data-ttu-id="de09a-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="de09a-186">Boolean</span></span>|<span data-ttu-id="de09a-187">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="de09a-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="de09a-188">将此设置为 true 将跳过用户提示, 并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="de09a-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="de09a-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="de09a-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="de09a-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="de09a-190">Boolean</span></span>|<span data-ttu-id="de09a-191">网络未广播其名称 (SSID) 时连接。</span><span class="sxs-lookup"><span data-stu-id="de09a-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="de09a-192">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="de09a-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="de09a-193">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="de09a-193">wiFiSecurityType</span></span>|[<span data-ttu-id="de09a-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="de09a-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="de09a-195">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="de09a-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="de09a-196">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="de09a-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="de09a-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="de09a-197">proxySettings</span></span>|[<span data-ttu-id="de09a-198">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="de09a-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="de09a-199">此 Wlan 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="de09a-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="de09a-200">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="de09a-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="de09a-201">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="de09a-201">proxyManualAddress</span></span>|<span data-ttu-id="de09a-202">String</span><span class="sxs-lookup"><span data-stu-id="de09a-202">String</span></span>|<span data-ttu-id="de09a-203">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="de09a-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="de09a-204">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="de09a-204">proxyManualPort</span></span>|<span data-ttu-id="de09a-205">Int32</span><span class="sxs-lookup"><span data-stu-id="de09a-205">Int32</span></span>|<span data-ttu-id="de09a-206">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="de09a-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="de09a-207">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="de09a-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="de09a-208">String</span><span class="sxs-lookup"><span data-stu-id="de09a-208">String</span></span>|<span data-ttu-id="de09a-209">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="de09a-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="de09a-210">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="de09a-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="de09a-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="de09a-211">preSharedKey</span></span>|<span data-ttu-id="de09a-212">String</span><span class="sxs-lookup"><span data-stu-id="de09a-212">String</span></span>|<span data-ttu-id="de09a-213">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="de09a-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="de09a-214">响应</span><span class="sxs-lookup"><span data-stu-id="de09a-214">Response</span></span>
<span data-ttu-id="de09a-215">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de09a-215">If successful, this method returns a `201 Created` response code and a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de09a-216">示例</span><span class="sxs-lookup"><span data-stu-id="de09a-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="de09a-217">请求</span><span class="sxs-lookup"><span data-stu-id="de09a-217">Request</span></span>
<span data-ttu-id="de09a-218">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de09a-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1448

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
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="de09a-219">响应</span><span class="sxs-lookup"><span data-stu-id="de09a-219">Response</span></span>
<span data-ttu-id="de09a-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de09a-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1620

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
  "preSharedKey": "Pre Shared Key value"
}
```





