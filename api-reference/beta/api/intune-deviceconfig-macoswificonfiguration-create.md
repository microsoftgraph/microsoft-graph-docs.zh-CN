---
title: 创建 macOSWiFiConfiguration
description: 创建新的 macOSWiFiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9d552fbc6c4d1d5a96309817482f2fca98ae983
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129669"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="8a59e-103">创建 macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a59e-103">Create macOSWiFiConfiguration</span></span>

<span data-ttu-id="8a59e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a59e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a59e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a59e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a59e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a59e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a59e-107">创建新的 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a59e-107">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a59e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8a59e-108">Prerequisites</span></span>
<span data-ttu-id="8a59e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a59e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a59e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a59e-111">Permission type</span></span>|<span data-ttu-id="8a59e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a59e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a59e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a59e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a59e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a59e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8a59e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a59e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a59e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a59e-116">Not supported.</span></span>|
|<span data-ttu-id="8a59e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a59e-117">Application</span></span>|<span data-ttu-id="8a59e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a59e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a59e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a59e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8a59e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a59e-120">Request headers</span></span>
|<span data-ttu-id="8a59e-121">标头</span><span class="sxs-lookup"><span data-stu-id="8a59e-121">Header</span></span>|<span data-ttu-id="8a59e-122">值</span><span class="sxs-lookup"><span data-stu-id="8a59e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a59e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a59e-123">Authorization</span></span>|<span data-ttu-id="8a59e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8a59e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a59e-125">接受</span><span class="sxs-lookup"><span data-stu-id="8a59e-125">Accept</span></span>|<span data-ttu-id="8a59e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a59e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a59e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a59e-127">Request body</span></span>
<span data-ttu-id="8a59e-128">在请求正文中，提供 macOSWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a59e-128">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="8a59e-129">下表显示创建 macOSWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8a59e-129">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="8a59e-130">属性</span><span class="sxs-lookup"><span data-stu-id="8a59e-130">Property</span></span>|<span data-ttu-id="8a59e-131">类型</span><span class="sxs-lookup"><span data-stu-id="8a59e-131">Type</span></span>|<span data-ttu-id="8a59e-132">说明</span><span class="sxs-lookup"><span data-stu-id="8a59e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a59e-133">id</span><span class="sxs-lookup"><span data-stu-id="8a59e-133">id</span></span>|<span data-ttu-id="8a59e-134">String</span><span class="sxs-lookup"><span data-stu-id="8a59e-134">String</span></span>|<span data-ttu-id="8a59e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8a59e-135">Key of the entity.</span></span> <span data-ttu-id="8a59e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a59e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8a59e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a59e-138">DateTimeOffset</span></span>|<span data-ttu-id="8a59e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a59e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8a59e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8a59e-141">roleScopeTagIds</span></span>|<span data-ttu-id="8a59e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="8a59e-142">String collection</span></span>|<span data-ttu-id="8a59e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8a59e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8a59e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8a59e-145">supportsScopeTags</span></span>|<span data-ttu-id="8a59e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a59e-146">Boolean</span></span>|<span data-ttu-id="8a59e-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="8a59e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8a59e-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="8a59e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8a59e-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="8a59e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8a59e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8a59e-150">This property is read-only.</span></span> <span data-ttu-id="8a59e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8a59e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8a59e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8a59e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8a59e-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="8a59e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8a59e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8a59e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8a59e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8a59e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8a59e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8a59e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8a59e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8a59e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8a59e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8a59e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8a59e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="8a59e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8a59e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a59e-164">createdDateTime</span></span>|<span data-ttu-id="8a59e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a59e-165">DateTimeOffset</span></span>|<span data-ttu-id="8a59e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a59e-166">DateTime the object was created.</span></span> <span data-ttu-id="8a59e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-168">说明</span><span class="sxs-lookup"><span data-stu-id="8a59e-168">description</span></span>|<span data-ttu-id="8a59e-169">String</span><span class="sxs-lookup"><span data-stu-id="8a59e-169">String</span></span>|<span data-ttu-id="8a59e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8a59e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8a59e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8a59e-172">displayName</span></span>|<span data-ttu-id="8a59e-173">String</span><span class="sxs-lookup"><span data-stu-id="8a59e-173">String</span></span>|<span data-ttu-id="8a59e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8a59e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8a59e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-176">version</span><span class="sxs-lookup"><span data-stu-id="8a59e-176">version</span></span>|<span data-ttu-id="8a59e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8a59e-177">Int32</span></span>|<span data-ttu-id="8a59e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8a59e-178">Version of the device configuration.</span></span> <span data-ttu-id="8a59e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a59e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8a59e-180">networkName</span><span class="sxs-lookup"><span data-stu-id="8a59e-180">networkName</span></span>|<span data-ttu-id="8a59e-181">String</span><span class="sxs-lookup"><span data-stu-id="8a59e-181">String</span></span>|<span data-ttu-id="8a59e-182">网络名称</span><span class="sxs-lookup"><span data-stu-id="8a59e-182">Network Name</span></span>|
|<span data-ttu-id="8a59e-183">ssid</span><span class="sxs-lookup"><span data-stu-id="8a59e-183">ssid</span></span>|<span data-ttu-id="8a59e-184">String</span><span class="sxs-lookup"><span data-stu-id="8a59e-184">String</span></span>|<span data-ttu-id="8a59e-185">这是广播到所有Wi-Fi网络的名称。</span><span class="sxs-lookup"><span data-stu-id="8a59e-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="8a59e-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="8a59e-186">connectAutomatically</span></span>|<span data-ttu-id="8a59e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a59e-187">Boolean</span></span>|<span data-ttu-id="8a59e-188">此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="8a59e-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="8a59e-189">如果设置为 true，将跳过用户提示，并自动将设备Wi-Fi网络。</span><span class="sxs-lookup"><span data-stu-id="8a59e-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="8a59e-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="8a59e-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="8a59e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a59e-191">Boolean</span></span>|<span data-ttu-id="8a59e-192">当网络未在 SSID 中广播其名称 (连接) 。</span><span class="sxs-lookup"><span data-stu-id="8a59e-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="8a59e-193">设置为 true 时，此配置文件会强制设备连接到未将其 SSID 广播到所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="8a59e-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="8a59e-194">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8a59e-194">wiFiSecurityType</span></span>|[<span data-ttu-id="8a59e-195">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8a59e-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="8a59e-196">指示Wi-Fi是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="8a59e-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="8a59e-197">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="8a59e-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="8a59e-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="8a59e-198">proxySettings</span></span>|[<span data-ttu-id="8a59e-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="8a59e-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="8a59e-200">此连接代理Wi-Fi类型。</span><span class="sxs-lookup"><span data-stu-id="8a59e-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="8a59e-201">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="8a59e-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="8a59e-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="8a59e-202">proxyManualAddress</span></span>|<span data-ttu-id="8a59e-203">String</span><span class="sxs-lookup"><span data-stu-id="8a59e-203">String</span></span>|<span data-ttu-id="8a59e-204">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="8a59e-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="8a59e-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="8a59e-205">proxyManualPort</span></span>|<span data-ttu-id="8a59e-206">Int32</span><span class="sxs-lookup"><span data-stu-id="8a59e-206">Int32</span></span>|<span data-ttu-id="8a59e-207">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="8a59e-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="8a59e-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="8a59e-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="8a59e-209">String</span><span class="sxs-lookup"><span data-stu-id="8a59e-209">String</span></span>|<span data-ttu-id="8a59e-210">选择自动配置时代理服务器自动配置脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="8a59e-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="8a59e-211">此 URL 通常是 PAC 代理自动配置 (文件) 位置。</span><span class="sxs-lookup"><span data-stu-id="8a59e-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="8a59e-212">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="8a59e-212">preSharedKey</span></span>|<span data-ttu-id="8a59e-213">String</span><span class="sxs-lookup"><span data-stu-id="8a59e-213">String</span></span>|<span data-ttu-id="8a59e-214">这是 WPA 个人共享网络的预共享Wi-Fi密钥。</span><span class="sxs-lookup"><span data-stu-id="8a59e-214">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="8a59e-215">响应</span><span class="sxs-lookup"><span data-stu-id="8a59e-215">Response</span></span>
<span data-ttu-id="8a59e-216">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8a59e-216">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a59e-217">示例</span><span class="sxs-lookup"><span data-stu-id="8a59e-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a59e-218">请求</span><span class="sxs-lookup"><span data-stu-id="8a59e-218">Request</span></span>
<span data-ttu-id="8a59e-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8a59e-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a59e-220">响应</span><span class="sxs-lookup"><span data-stu-id="8a59e-220">Response</span></span>
<span data-ttu-id="8a59e-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a59e-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




