---
title: 创建 macOSWiFiConfiguration
description: 创建新的 macOSWiFiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c820f18d8e7a487b9368d17ea50a6ce90b46ab6a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287373"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="418b8-103">创建 macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="418b8-103">Create macOSWiFiConfiguration</span></span>

<span data-ttu-id="418b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="418b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="418b8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="418b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="418b8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="418b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="418b8-107">创建新的 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="418b8-107">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="418b8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="418b8-108">Prerequisites</span></span>
<span data-ttu-id="418b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="418b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="418b8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="418b8-111">Permission type</span></span>|<span data-ttu-id="418b8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="418b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="418b8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="418b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="418b8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418b8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="418b8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="418b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="418b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="418b8-116">Not supported.</span></span>|
|<span data-ttu-id="418b8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="418b8-117">Application</span></span>|<span data-ttu-id="418b8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418b8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="418b8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="418b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="418b8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="418b8-120">Request headers</span></span>
|<span data-ttu-id="418b8-121">标头</span><span class="sxs-lookup"><span data-stu-id="418b8-121">Header</span></span>|<span data-ttu-id="418b8-122">值</span><span class="sxs-lookup"><span data-stu-id="418b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="418b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="418b8-123">Authorization</span></span>|<span data-ttu-id="418b8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="418b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="418b8-125">接受</span><span class="sxs-lookup"><span data-stu-id="418b8-125">Accept</span></span>|<span data-ttu-id="418b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="418b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="418b8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="418b8-127">Request body</span></span>
<span data-ttu-id="418b8-128">在请求正文中，提供 macOSWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="418b8-128">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="418b8-129">下表显示创建 macOSWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="418b8-129">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="418b8-130">属性</span><span class="sxs-lookup"><span data-stu-id="418b8-130">Property</span></span>|<span data-ttu-id="418b8-131">类型</span><span class="sxs-lookup"><span data-stu-id="418b8-131">Type</span></span>|<span data-ttu-id="418b8-132">说明</span><span class="sxs-lookup"><span data-stu-id="418b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="418b8-133">id</span><span class="sxs-lookup"><span data-stu-id="418b8-133">id</span></span>|<span data-ttu-id="418b8-134">字符串</span><span class="sxs-lookup"><span data-stu-id="418b8-134">String</span></span>|<span data-ttu-id="418b8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="418b8-135">Key of the entity.</span></span> <span data-ttu-id="418b8-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="418b8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="418b8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="418b8-138">DateTimeOffset</span></span>|<span data-ttu-id="418b8-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="418b8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="418b8-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="418b8-141">roleScopeTagIds</span></span>|<span data-ttu-id="418b8-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="418b8-142">String collection</span></span>|<span data-ttu-id="418b8-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="418b8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="418b8-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="418b8-145">supportsScopeTags</span></span>|<span data-ttu-id="418b8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="418b8-146">Boolean</span></span>|<span data-ttu-id="418b8-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="418b8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="418b8-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="418b8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="418b8-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="418b8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="418b8-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="418b8-150">This property is read-only.</span></span> <span data-ttu-id="418b8-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="418b8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="418b8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="418b8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="418b8-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="418b8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="418b8-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="418b8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="418b8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="418b8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="418b8-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="418b8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="418b8-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="418b8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="418b8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="418b8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="418b8-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="418b8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="418b8-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="418b8-164">createdDateTime</span></span>|<span data-ttu-id="418b8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="418b8-165">DateTimeOffset</span></span>|<span data-ttu-id="418b8-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="418b8-166">DateTime the object was created.</span></span> <span data-ttu-id="418b8-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-168">description</span><span class="sxs-lookup"><span data-stu-id="418b8-168">description</span></span>|<span data-ttu-id="418b8-169">字符串</span><span class="sxs-lookup"><span data-stu-id="418b8-169">String</span></span>|<span data-ttu-id="418b8-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="418b8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="418b8-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="418b8-172">displayName</span></span>|<span data-ttu-id="418b8-173">字符串</span><span class="sxs-lookup"><span data-stu-id="418b8-173">String</span></span>|<span data-ttu-id="418b8-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="418b8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="418b8-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-176">version</span><span class="sxs-lookup"><span data-stu-id="418b8-176">version</span></span>|<span data-ttu-id="418b8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="418b8-177">Int32</span></span>|<span data-ttu-id="418b8-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="418b8-178">Version of the device configuration.</span></span> <span data-ttu-id="418b8-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418b8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418b8-180">networkName</span><span class="sxs-lookup"><span data-stu-id="418b8-180">networkName</span></span>|<span data-ttu-id="418b8-181">字符串</span><span class="sxs-lookup"><span data-stu-id="418b8-181">String</span></span>|<span data-ttu-id="418b8-182">网络名称</span><span class="sxs-lookup"><span data-stu-id="418b8-182">Network Name</span></span>|
|<span data-ttu-id="418b8-183">ssid</span><span class="sxs-lookup"><span data-stu-id="418b8-183">ssid</span></span>|<span data-ttu-id="418b8-184">字符串</span><span class="sxs-lookup"><span data-stu-id="418b8-184">String</span></span>|<span data-ttu-id="418b8-185">这是广播到所有设备的 Wi-Fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="418b8-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="418b8-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="418b8-186">connectAutomatically</span></span>|<span data-ttu-id="418b8-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="418b8-187">Boolean</span></span>|<span data-ttu-id="418b8-188">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="418b8-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="418b8-189">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="418b8-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="418b8-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="418b8-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="418b8-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="418b8-191">Boolean</span></span>|<span data-ttu-id="418b8-192">网络未广播其名称 (SSID) 时连接。</span><span class="sxs-lookup"><span data-stu-id="418b8-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="418b8-193">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="418b8-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="418b8-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="418b8-194">wiFiSecurityType</span></span>|[<span data-ttu-id="418b8-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="418b8-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="418b8-196">指示 Wi-Fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="418b8-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="418b8-197">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="418b8-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="418b8-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="418b8-198">proxySettings</span></span>|[<span data-ttu-id="418b8-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="418b8-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="418b8-200">此 Wi-Fi 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="418b8-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="418b8-201">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="418b8-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="418b8-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="418b8-202">proxyManualAddress</span></span>|<span data-ttu-id="418b8-203">字符串</span><span class="sxs-lookup"><span data-stu-id="418b8-203">String</span></span>|<span data-ttu-id="418b8-204">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="418b8-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="418b8-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="418b8-205">proxyManualPort</span></span>|<span data-ttu-id="418b8-206">Int32</span><span class="sxs-lookup"><span data-stu-id="418b8-206">Int32</span></span>|<span data-ttu-id="418b8-207">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="418b8-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="418b8-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="418b8-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="418b8-209">字符串</span><span class="sxs-lookup"><span data-stu-id="418b8-209">String</span></span>|<span data-ttu-id="418b8-210">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="418b8-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="418b8-211">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="418b8-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="418b8-212">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="418b8-212">preSharedKey</span></span>|<span data-ttu-id="418b8-213">字符串</span><span class="sxs-lookup"><span data-stu-id="418b8-213">String</span></span>|<span data-ttu-id="418b8-214">这是 WPA 个人 Wi-Fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="418b8-214">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="418b8-215">响应</span><span class="sxs-lookup"><span data-stu-id="418b8-215">Response</span></span>
<span data-ttu-id="418b8-216">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="418b8-216">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="418b8-217">示例</span><span class="sxs-lookup"><span data-stu-id="418b8-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="418b8-218">请求</span><span class="sxs-lookup"><span data-stu-id="418b8-218">Request</span></span>
<span data-ttu-id="418b8-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="418b8-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1450

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="418b8-220">响应</span><span class="sxs-lookup"><span data-stu-id="418b8-220">Response</span></span>
<span data-ttu-id="418b8-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="418b8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1622

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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




