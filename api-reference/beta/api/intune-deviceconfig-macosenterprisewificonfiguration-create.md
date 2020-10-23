---
title: 创建 macOSEnterpriseWiFiConfiguration
description: 创建新的 macOSEnterpriseWiFiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e393861c9e86bb7e91fb45e35c60034c8ee9188
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732991"
---
# <a name="create-macosenterprisewificonfiguration"></a><span data-ttu-id="9820a-103">创建 macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="9820a-103">Create macOSEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="9820a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9820a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9820a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9820a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9820a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9820a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9820a-107">创建新的 [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9820a-107">Create a new [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9820a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9820a-108">Prerequisites</span></span>
<span data-ttu-id="9820a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9820a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9820a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9820a-111">Permission type</span></span>|<span data-ttu-id="9820a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9820a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9820a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9820a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9820a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9820a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9820a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9820a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9820a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9820a-116">Not supported.</span></span>|
|<span data-ttu-id="9820a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9820a-117">Application</span></span>|<span data-ttu-id="9820a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9820a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9820a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9820a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9820a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9820a-120">Request headers</span></span>
|<span data-ttu-id="9820a-121">标头</span><span class="sxs-lookup"><span data-stu-id="9820a-121">Header</span></span>|<span data-ttu-id="9820a-122">值</span><span class="sxs-lookup"><span data-stu-id="9820a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9820a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9820a-123">Authorization</span></span>|<span data-ttu-id="9820a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9820a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9820a-125">接受</span><span class="sxs-lookup"><span data-stu-id="9820a-125">Accept</span></span>|<span data-ttu-id="9820a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9820a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9820a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9820a-127">Request body</span></span>
<span data-ttu-id="9820a-128">在请求正文中，提供 macOSEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9820a-128">In the request body, supply a JSON representation for the macOSEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="9820a-129">下表显示创建 macOSEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9820a-129">The following table shows the properties that are required when you create the macOSEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="9820a-130">属性</span><span class="sxs-lookup"><span data-stu-id="9820a-130">Property</span></span>|<span data-ttu-id="9820a-131">类型</span><span class="sxs-lookup"><span data-stu-id="9820a-131">Type</span></span>|<span data-ttu-id="9820a-132">说明</span><span class="sxs-lookup"><span data-stu-id="9820a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9820a-133">id</span><span class="sxs-lookup"><span data-stu-id="9820a-133">id</span></span>|<span data-ttu-id="9820a-134">String</span><span class="sxs-lookup"><span data-stu-id="9820a-134">String</span></span>|<span data-ttu-id="9820a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9820a-135">Key of the entity.</span></span> <span data-ttu-id="9820a-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9820a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9820a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9820a-138">DateTimeOffset</span></span>|<span data-ttu-id="9820a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9820a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9820a-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9820a-141">roleScopeTagIds</span></span>|<span data-ttu-id="9820a-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9820a-142">String collection</span></span>|<span data-ttu-id="9820a-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9820a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9820a-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9820a-145">supportsScopeTags</span></span>|<span data-ttu-id="9820a-146">布尔</span><span class="sxs-lookup"><span data-stu-id="9820a-146">Boolean</span></span>|<span data-ttu-id="9820a-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9820a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9820a-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9820a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9820a-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9820a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9820a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9820a-150">This property is read-only.</span></span> <span data-ttu-id="9820a-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9820a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9820a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9820a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9820a-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9820a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9820a-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9820a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9820a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9820a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9820a-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9820a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9820a-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9820a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9820a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9820a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9820a-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9820a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9820a-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9820a-164">createdDateTime</span></span>|<span data-ttu-id="9820a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9820a-165">DateTimeOffset</span></span>|<span data-ttu-id="9820a-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9820a-166">DateTime the object was created.</span></span> <span data-ttu-id="9820a-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-168">说明</span><span class="sxs-lookup"><span data-stu-id="9820a-168">description</span></span>|<span data-ttu-id="9820a-169">String</span><span class="sxs-lookup"><span data-stu-id="9820a-169">String</span></span>|<span data-ttu-id="9820a-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9820a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9820a-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9820a-172">displayName</span></span>|<span data-ttu-id="9820a-173">String</span><span class="sxs-lookup"><span data-stu-id="9820a-173">String</span></span>|<span data-ttu-id="9820a-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9820a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9820a-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-176">version</span><span class="sxs-lookup"><span data-stu-id="9820a-176">version</span></span>|<span data-ttu-id="9820a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9820a-177">Int32</span></span>|<span data-ttu-id="9820a-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9820a-178">Version of the device configuration.</span></span> <span data-ttu-id="9820a-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9820a-180">networkName</span><span class="sxs-lookup"><span data-stu-id="9820a-180">networkName</span></span>|<span data-ttu-id="9820a-181">String</span><span class="sxs-lookup"><span data-stu-id="9820a-181">String</span></span>|<span data-ttu-id="9820a-182">从[MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="9820a-182">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9820a-183">ssid</span><span class="sxs-lookup"><span data-stu-id="9820a-183">ssid</span></span>|<span data-ttu-id="9820a-184">String</span><span class="sxs-lookup"><span data-stu-id="9820a-184">String</span></span>|<span data-ttu-id="9820a-185">这是广播到所有设备的 Wi-Fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="9820a-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="9820a-186">继承自 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-186">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9820a-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="9820a-187">connectAutomatically</span></span>|<span data-ttu-id="9820a-188">布尔</span><span class="sxs-lookup"><span data-stu-id="9820a-188">Boolean</span></span>|<span data-ttu-id="9820a-189">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="9820a-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="9820a-190">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="9820a-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="9820a-191">继承自 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-191">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9820a-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9820a-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9820a-193">布尔</span><span class="sxs-lookup"><span data-stu-id="9820a-193">Boolean</span></span>|<span data-ttu-id="9820a-194">网络未广播其名称 (SSID) 时连接。</span><span class="sxs-lookup"><span data-stu-id="9820a-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="9820a-195">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="9820a-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="9820a-196">继承自 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-196">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9820a-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9820a-197">wiFiSecurityType</span></span>|[<span data-ttu-id="9820a-198">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9820a-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="9820a-199">指示 Wi-Fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="9820a-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="9820a-200">继承自 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="9820a-200">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="9820a-201">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="9820a-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="9820a-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="9820a-202">proxySettings</span></span>|[<span data-ttu-id="9820a-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="9820a-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="9820a-204">此 Wi-Fi 从 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)继承的连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="9820a-204">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="9820a-205">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="9820a-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="9820a-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="9820a-206">proxyManualAddress</span></span>|<span data-ttu-id="9820a-207">String</span><span class="sxs-lookup"><span data-stu-id="9820a-207">String</span></span>|<span data-ttu-id="9820a-208">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="9820a-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="9820a-209">继承自 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-209">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9820a-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="9820a-210">proxyManualPort</span></span>|<span data-ttu-id="9820a-211">Int32</span><span class="sxs-lookup"><span data-stu-id="9820a-211">Int32</span></span>|<span data-ttu-id="9820a-212">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="9820a-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="9820a-213">继承自 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-213">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9820a-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="9820a-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="9820a-215">String</span><span class="sxs-lookup"><span data-stu-id="9820a-215">String</span></span>|<span data-ttu-id="9820a-216">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="9820a-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="9820a-217">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="9820a-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="9820a-218">继承自 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-218">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9820a-219">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="9820a-219">preSharedKey</span></span>|<span data-ttu-id="9820a-220">String</span><span class="sxs-lookup"><span data-stu-id="9820a-220">String</span></span>|<span data-ttu-id="9820a-221">这是 WPA 个人 Wi-Fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="9820a-221">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="9820a-222">继承自 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9820a-222">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9820a-223">eapType</span><span class="sxs-lookup"><span data-stu-id="9820a-223">eapType</span></span>|[<span data-ttu-id="9820a-224">eapType</span><span class="sxs-lookup"><span data-stu-id="9820a-224">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="9820a-225">可扩展的身份验证协议 (EAP) 。</span><span class="sxs-lookup"><span data-stu-id="9820a-225">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="9820a-226">指示 Wi-Fi 终结点 (路由器) 上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="9820a-226">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="9820a-227">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="9820a-227">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="9820a-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="9820a-228">eapFastConfiguration</span></span>|[<span data-ttu-id="9820a-229">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="9820a-229">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="9820a-230">EAP-FAST 配置选项，当 EAP-FAST 是所选的 EAP 类型时。</span><span class="sxs-lookup"><span data-stu-id="9820a-230">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="9820a-231">可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。</span><span class="sxs-lookup"><span data-stu-id="9820a-231">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="9820a-232">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="9820a-232">trustedServerCertificateNames</span></span>|<span data-ttu-id="9820a-233">String collection</span><span class="sxs-lookup"><span data-stu-id="9820a-233">String collection</span></span>|<span data-ttu-id="9820a-234">将 EAP 类型配置为 EAP-TLS/TTLS/FAST 或 PEAP 时受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="9820a-234">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="9820a-235">这是受信任的证书颁发机构 (CA) 颁发的证书中使用的常用名称。</span><span class="sxs-lookup"><span data-stu-id="9820a-235">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="9820a-236">如果提供此信息，则可以在最终用户设备连接到此 Wi-Fi 网络时，绕过显示在最终用户设备上的 "动态信任" 对话框。</span><span class="sxs-lookup"><span data-stu-id="9820a-236">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="9820a-237">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9820a-237">authenticationMethod</span></span>|[<span data-ttu-id="9820a-238">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9820a-238">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="9820a-239">EAP 类型配置为 PEAP 或 EAP-TTLS 时的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="9820a-239">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="9820a-240">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="9820a-240">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="9820a-241">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="9820a-241">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="9820a-242">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="9820a-242">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="9820a-243">在 EAP 类型为 EAP 时，用于身份验证的非 EAP 方法 (内部标识) （eap 类型为 EAP-TTLS，Authenticationmethod 为用户名和密码）。</span><span class="sxs-lookup"><span data-stu-id="9820a-243">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="9820a-244">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="9820a-244">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="9820a-245">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="9820a-245">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="9820a-246">String</span><span class="sxs-lookup"><span data-stu-id="9820a-246">String</span></span>|<span data-ttu-id="9820a-247">将 EAP 类型配置为 EAP-TTLS、EAP-FAST 或 PEAP 时，请启用标识隐私 (外部标识) 。</span><span class="sxs-lookup"><span data-stu-id="9820a-247">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="9820a-248">此属性使用您输入的文本屏蔽用户名。</span><span class="sxs-lookup"><span data-stu-id="9820a-248">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="9820a-249">例如，如果使用 "匿名"，则使用其真实用户名通过此 Wi-Fi 连接进行身份验证的每个用户都显示为 "匿名"。</span><span class="sxs-lookup"><span data-stu-id="9820a-249">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="9820a-250">响应</span><span class="sxs-lookup"><span data-stu-id="9820a-250">Response</span></span>
<span data-ttu-id="9820a-251">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9820a-251">If successful, this method returns a `201 Created` response code and a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9820a-252">示例</span><span class="sxs-lookup"><span data-stu-id="9820a-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="9820a-253">请求</span><span class="sxs-lookup"><span data-stu-id="9820a-253">Request</span></span>
<span data-ttu-id="9820a-254">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9820a-254">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1858

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="9820a-255">响应</span><span class="sxs-lookup"><span data-stu-id="9820a-255">Response</span></span>
<span data-ttu-id="9820a-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9820a-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2030

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





