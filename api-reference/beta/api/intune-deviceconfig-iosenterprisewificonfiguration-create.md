---
title: 创建 iosEnterpriseWiFiConfiguration
description: 创建新的 iosEnterpriseWiFiConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa3efe22a5879a3207f013337432b0d09176f83f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948926"
---
# <a name="create-iosenterprisewificonfiguration"></a><span data-ttu-id="d1f82-103">创建 iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1f82-103">Create iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="d1f82-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1f82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1f82-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1f82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1f82-106">创建新的[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d1f82-106">Create a new [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1f82-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1f82-107">Prerequisites</span></span>
<span data-ttu-id="d1f82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1f82-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1f82-110">Permission type</span></span>|<span data-ttu-id="d1f82-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d1f82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1f82-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1f82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1f82-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f82-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1f82-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1f82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1f82-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1f82-115">Not supported.</span></span>|
|<span data-ttu-id="d1f82-116">Application</span><span class="sxs-lookup"><span data-stu-id="d1f82-116">Application</span></span>|<span data-ttu-id="d1f82-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1f82-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1f82-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1f82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d1f82-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1f82-119">Request headers</span></span>
|<span data-ttu-id="d1f82-120">标头</span><span class="sxs-lookup"><span data-stu-id="d1f82-120">Header</span></span>|<span data-ttu-id="d1f82-121">值</span><span class="sxs-lookup"><span data-stu-id="d1f82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1f82-122">授权</span><span class="sxs-lookup"><span data-stu-id="d1f82-122">Authorization</span></span>|<span data-ttu-id="d1f82-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1f82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1f82-124">接受</span><span class="sxs-lookup"><span data-stu-id="d1f82-124">Accept</span></span>|<span data-ttu-id="d1f82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1f82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1f82-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1f82-126">Request body</span></span>
<span data-ttu-id="d1f82-127">在请求正文中，提供 iosEnterpriseWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1f82-127">In the request body, supply a JSON representation for the iosEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="d1f82-128">下表显示创建 iosEnterpriseWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d1f82-128">The following table shows the properties that are required when you create the iosEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="d1f82-129">属性</span><span class="sxs-lookup"><span data-stu-id="d1f82-129">Property</span></span>|<span data-ttu-id="d1f82-130">类型</span><span class="sxs-lookup"><span data-stu-id="d1f82-130">Type</span></span>|<span data-ttu-id="d1f82-131">说明</span><span class="sxs-lookup"><span data-stu-id="d1f82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1f82-132">id</span><span class="sxs-lookup"><span data-stu-id="d1f82-132">id</span></span>|<span data-ttu-id="d1f82-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-133">String</span></span>|<span data-ttu-id="d1f82-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d1f82-134">Key of the entity.</span></span> <span data-ttu-id="d1f82-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1f82-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d1f82-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1f82-137">DateTimeOffset</span></span>|<span data-ttu-id="d1f82-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d1f82-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d1f82-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d1f82-140">roleScopeTagIds</span></span>|<span data-ttu-id="d1f82-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d1f82-141">String collection</span></span>|<span data-ttu-id="d1f82-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d1f82-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d1f82-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d1f82-144">supportsScopeTags</span></span>|<span data-ttu-id="d1f82-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f82-145">Boolean</span></span>|<span data-ttu-id="d1f82-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d1f82-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d1f82-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d1f82-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d1f82-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d1f82-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d1f82-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d1f82-149">This property is read-only.</span></span> <span data-ttu-id="d1f82-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d1f82-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d1f82-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d1f82-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d1f82-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="d1f82-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d1f82-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d1f82-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d1f82-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d1f82-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d1f82-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d1f82-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d1f82-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d1f82-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d1f82-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d1f82-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d1f82-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d1f82-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d1f82-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1f82-163">createdDateTime</span></span>|<span data-ttu-id="d1f82-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1f82-164">DateTimeOffset</span></span>|<span data-ttu-id="d1f82-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d1f82-165">DateTime the object was created.</span></span> <span data-ttu-id="d1f82-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-167">说明</span><span class="sxs-lookup"><span data-stu-id="d1f82-167">description</span></span>|<span data-ttu-id="d1f82-168">String</span><span class="sxs-lookup"><span data-stu-id="d1f82-168">String</span></span>|<span data-ttu-id="d1f82-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d1f82-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d1f82-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d1f82-171">displayName</span></span>|<span data-ttu-id="d1f82-172">String</span><span class="sxs-lookup"><span data-stu-id="d1f82-172">String</span></span>|<span data-ttu-id="d1f82-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d1f82-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d1f82-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-175">version</span><span class="sxs-lookup"><span data-stu-id="d1f82-175">version</span></span>|<span data-ttu-id="d1f82-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f82-176">Int32</span></span>|<span data-ttu-id="d1f82-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d1f82-177">Version of the device configuration.</span></span> <span data-ttu-id="d1f82-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-179">networkName</span><span class="sxs-lookup"><span data-stu-id="d1f82-179">networkName</span></span>|<span data-ttu-id="d1f82-180">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-180">String</span></span>|<span data-ttu-id="d1f82-181">从[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="d1f82-181">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-182">ssid</span><span class="sxs-lookup"><span data-stu-id="d1f82-182">ssid</span></span>|<span data-ttu-id="d1f82-183">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-183">String</span></span>|<span data-ttu-id="d1f82-184">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="d1f82-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="d1f82-185">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-185">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="d1f82-186">connectAutomatically</span></span>|<span data-ttu-id="d1f82-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f82-187">Boolean</span></span>|<span data-ttu-id="d1f82-188">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="d1f82-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="d1f82-189">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="d1f82-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="d1f82-190">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-190">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="d1f82-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="d1f82-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1f82-192">Boolean</span></span>|<span data-ttu-id="d1f82-193">网络未广播其名称（SSID）时连接。</span><span class="sxs-lookup"><span data-stu-id="d1f82-193">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="d1f82-194">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="d1f82-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="d1f82-195">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-195">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d1f82-196">wiFiSecurityType</span></span>|[<span data-ttu-id="d1f82-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d1f82-197">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="d1f82-198">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="d1f82-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="d1f82-199">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="d1f82-199">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="d1f82-200">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="d1f82-200">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="d1f82-201">proxySettings</span><span class="sxs-lookup"><span data-stu-id="d1f82-201">proxySettings</span></span>|[<span data-ttu-id="d1f82-202">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="d1f82-202">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="d1f82-203">从[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)继承的此 wi-fi 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="d1f82-203">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="d1f82-204">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="d1f82-204">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="d1f82-205">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="d1f82-205">proxyManualAddress</span></span>|<span data-ttu-id="d1f82-206">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-206">String</span></span>|<span data-ttu-id="d1f82-207">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="d1f82-207">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="d1f82-208">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-208">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-209">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="d1f82-209">proxyManualPort</span></span>|<span data-ttu-id="d1f82-210">Int32</span><span class="sxs-lookup"><span data-stu-id="d1f82-210">Int32</span></span>|<span data-ttu-id="d1f82-211">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="d1f82-211">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="d1f82-212">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-212">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-213">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="d1f82-213">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="d1f82-214">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-214">String</span></span>|<span data-ttu-id="d1f82-215">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="d1f82-215">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="d1f82-216">此 URL 通常是 PAC （代理自动配置）文件的位置。</span><span class="sxs-lookup"><span data-stu-id="d1f82-216">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="d1f82-217">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-217">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-218">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="d1f82-218">preSharedKey</span></span>|<span data-ttu-id="d1f82-219">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-219">String</span></span>|<span data-ttu-id="d1f82-220">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="d1f82-220">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="d1f82-221">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1f82-221">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="d1f82-222">eapType</span><span class="sxs-lookup"><span data-stu-id="d1f82-222">eapType</span></span>|[<span data-ttu-id="d1f82-223">eapType</span><span class="sxs-lookup"><span data-stu-id="d1f82-223">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="d1f82-224">可扩展的身份验证协议（EAP）。</span><span class="sxs-lookup"><span data-stu-id="d1f82-224">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="d1f82-225">指示 Wi-fi 终结点（路由器）上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="d1f82-225">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="d1f82-226">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="d1f82-226">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="d1f82-227">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1f82-227">eapFastConfiguration</span></span>|[<span data-ttu-id="d1f82-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1f82-228">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="d1f82-229">EAP-FAST 配置选项，当 EAP-FAST 是所选的 EAP 类型时。</span><span class="sxs-lookup"><span data-stu-id="d1f82-229">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="d1f82-230">可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。</span><span class="sxs-lookup"><span data-stu-id="d1f82-230">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="d1f82-231">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="d1f82-231">trustedServerCertificateNames</span></span>|<span data-ttu-id="d1f82-232">String collection</span><span class="sxs-lookup"><span data-stu-id="d1f82-232">String collection</span></span>|<span data-ttu-id="d1f82-233">将 EAP 类型配置为 EAP-TLS/TTLS/FAST 或 PEAP 时受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="d1f82-233">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="d1f82-234">这是由受信任的证书颁发机构（CA）颁发的证书中使用的公用名称。</span><span class="sxs-lookup"><span data-stu-id="d1f82-234">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="d1f82-235">如果提供此信息，则可以绕过在最终用户的设备连接到此 Wi-fi 网络时显示的动态信任对话框。</span><span class="sxs-lookup"><span data-stu-id="d1f82-235">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="d1f82-236">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d1f82-236">authenticationMethod</span></span>|[<span data-ttu-id="d1f82-237">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d1f82-237">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="d1f82-238">EAP 类型配置为 PEAP 或 EAP-TTLS 时的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="d1f82-238">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="d1f82-239">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="d1f82-239">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d1f82-240">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="d1f82-240">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="d1f82-241">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="d1f82-241">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="d1f82-242">EAP 类型为 EAP 时进行身份验证的非 EAP 方法-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="d1f82-242">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="d1f82-243">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="d1f82-243">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="d1f82-244">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="d1f82-244">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="d1f82-245">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-245">String</span></span>|<span data-ttu-id="d1f82-246">将 EAP 类型配置为 EAP-TTLS、EAP-FAST 或 PEAP 时启用标识隐私（外部标识）。</span><span class="sxs-lookup"><span data-stu-id="d1f82-246">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="d1f82-247">此属性使用您输入的文本屏蔽用户名。</span><span class="sxs-lookup"><span data-stu-id="d1f82-247">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="d1f82-248">例如，如果使用 "匿名"，则使用其真实用户名通过此 Wlan 连接进行身份验证的每个用户都将显示为 "匿名"。</span><span class="sxs-lookup"><span data-stu-id="d1f82-248">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="d1f82-249">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="d1f82-249">usernameFormatString</span></span>|<span data-ttu-id="d1f82-250">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-250">String</span></span>|<span data-ttu-id="d1f82-251">用于生成用户名以连接到 wifi 的用户名格式字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-251">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="d1f82-252">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="d1f82-252">passwordFormatString</span></span>|<span data-ttu-id="d1f82-253">字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-253">String</span></span>|<span data-ttu-id="d1f82-254">用于生成密码以连接到 wifi 的密码格式字符串</span><span class="sxs-lookup"><span data-stu-id="d1f82-254">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="d1f82-255">响应</span><span class="sxs-lookup"><span data-stu-id="d1f82-255">Response</span></span>
<span data-ttu-id="d1f82-256">如果成功，此方法在响应`201 Created`正文中返回响应代码和[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d1f82-256">If successful, this method returns a `201 Created` response code and a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1f82-257">示例</span><span class="sxs-lookup"><span data-stu-id="d1f82-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1f82-258">请求</span><span class="sxs-lookup"><span data-stu-id="d1f82-258">Request</span></span>
<span data-ttu-id="d1f82-259">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1f82-259">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1974

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```

### <a name="response"></a><span data-ttu-id="d1f82-260">响应</span><span class="sxs-lookup"><span data-stu-id="d1f82-260">Response</span></span>
<span data-ttu-id="d1f82-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1f82-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2146

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```





