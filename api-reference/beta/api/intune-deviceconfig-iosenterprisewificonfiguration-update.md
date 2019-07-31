---
title: 更新 iosEnterpriseWiFiConfiguration
description: 更新 iosEnterpriseWiFiConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c028f454c9221fa7707d921b16b891d6b9d3ce97
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948248"
---
# <a name="update-iosenterprisewificonfiguration"></a><span data-ttu-id="92f26-103">更新 iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="92f26-103">Update iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="92f26-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92f26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92f26-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92f26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92f26-106">更新[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="92f26-106">Update the properties of a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92f26-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="92f26-107">Prerequisites</span></span>
<span data-ttu-id="92f26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92f26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92f26-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="92f26-110">Permission type</span></span>|<span data-ttu-id="92f26-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="92f26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92f26-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92f26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92f26-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92f26-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92f26-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92f26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92f26-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92f26-115">Not supported.</span></span>|
|<span data-ttu-id="92f26-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="92f26-116">Application</span></span>|<span data-ttu-id="92f26-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="92f26-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92f26-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92f26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="92f26-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="92f26-119">Request headers</span></span>
|<span data-ttu-id="92f26-120">标头</span><span class="sxs-lookup"><span data-stu-id="92f26-120">Header</span></span>|<span data-ttu-id="92f26-121">值</span><span class="sxs-lookup"><span data-stu-id="92f26-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92f26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92f26-122">Authorization</span></span>|<span data-ttu-id="92f26-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92f26-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92f26-124">接受</span><span class="sxs-lookup"><span data-stu-id="92f26-124">Accept</span></span>|<span data-ttu-id="92f26-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92f26-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92f26-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="92f26-126">Request body</span></span>
<span data-ttu-id="92f26-127">在请求正文中, 提供[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92f26-127">In the request body, supply a JSON representation for the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="92f26-128">下表显示创建[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="92f26-128">The following table shows the properties that are required when you create the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="92f26-129">属性</span><span class="sxs-lookup"><span data-stu-id="92f26-129">Property</span></span>|<span data-ttu-id="92f26-130">类型</span><span class="sxs-lookup"><span data-stu-id="92f26-130">Type</span></span>|<span data-ttu-id="92f26-131">说明</span><span class="sxs-lookup"><span data-stu-id="92f26-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92f26-132">id</span><span class="sxs-lookup"><span data-stu-id="92f26-132">id</span></span>|<span data-ttu-id="92f26-133">字符串</span><span class="sxs-lookup"><span data-stu-id="92f26-133">String</span></span>|<span data-ttu-id="92f26-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="92f26-134">Key of the entity.</span></span> <span data-ttu-id="92f26-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92f26-136">lastModifiedDateTime</span></span>|<span data-ttu-id="92f26-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92f26-137">DateTimeOffset</span></span>|<span data-ttu-id="92f26-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="92f26-138">DateTime the object was last modified.</span></span> <span data-ttu-id="92f26-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92f26-140">roleScopeTagIds</span></span>|<span data-ttu-id="92f26-141">String collection</span><span class="sxs-lookup"><span data-stu-id="92f26-141">String collection</span></span>|<span data-ttu-id="92f26-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="92f26-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="92f26-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="92f26-144">supportsScopeTags</span></span>|<span data-ttu-id="92f26-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="92f26-145">Boolean</span></span>|<span data-ttu-id="92f26-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="92f26-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="92f26-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="92f26-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="92f26-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="92f26-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="92f26-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="92f26-149">This property is read-only.</span></span> <span data-ttu-id="92f26-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92f26-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="92f26-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92f26-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="92f26-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="92f26-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="92f26-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92f26-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="92f26-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92f26-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="92f26-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="92f26-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="92f26-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92f26-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="92f26-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92f26-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="92f26-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="92f26-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="92f26-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92f26-163">createdDateTime</span></span>|<span data-ttu-id="92f26-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92f26-164">DateTimeOffset</span></span>|<span data-ttu-id="92f26-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="92f26-165">DateTime the object was created.</span></span> <span data-ttu-id="92f26-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-167">说明</span><span class="sxs-lookup"><span data-stu-id="92f26-167">description</span></span>|<span data-ttu-id="92f26-168">String</span><span class="sxs-lookup"><span data-stu-id="92f26-168">String</span></span>|<span data-ttu-id="92f26-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="92f26-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92f26-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-171">displayName</span><span class="sxs-lookup"><span data-stu-id="92f26-171">displayName</span></span>|<span data-ttu-id="92f26-172">String</span><span class="sxs-lookup"><span data-stu-id="92f26-172">String</span></span>|<span data-ttu-id="92f26-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="92f26-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92f26-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-175">version</span><span class="sxs-lookup"><span data-stu-id="92f26-175">version</span></span>|<span data-ttu-id="92f26-176">Int32</span><span class="sxs-lookup"><span data-stu-id="92f26-176">Int32</span></span>|<span data-ttu-id="92f26-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="92f26-177">Version of the device configuration.</span></span> <span data-ttu-id="92f26-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92f26-179">networkName</span><span class="sxs-lookup"><span data-stu-id="92f26-179">networkName</span></span>|<span data-ttu-id="92f26-180">String</span><span class="sxs-lookup"><span data-stu-id="92f26-180">String</span></span>|<span data-ttu-id="92f26-181">从[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)继承的网络名称</span><span class="sxs-lookup"><span data-stu-id="92f26-181">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f26-182">ssid</span><span class="sxs-lookup"><span data-stu-id="92f26-182">ssid</span></span>|<span data-ttu-id="92f26-183">String</span><span class="sxs-lookup"><span data-stu-id="92f26-183">String</span></span>|<span data-ttu-id="92f26-184">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="92f26-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="92f26-185">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-185">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f26-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="92f26-186">connectAutomatically</span></span>|<span data-ttu-id="92f26-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="92f26-187">Boolean</span></span>|<span data-ttu-id="92f26-188">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="92f26-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="92f26-189">将此设置为 true 将跳过用户提示, 并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="92f26-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="92f26-190">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-190">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f26-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="92f26-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="92f26-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="92f26-192">Boolean</span></span>|<span data-ttu-id="92f26-193">网络未广播其名称 (SSID) 时连接。</span><span class="sxs-lookup"><span data-stu-id="92f26-193">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="92f26-194">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="92f26-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="92f26-195">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-195">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f26-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="92f26-196">wiFiSecurityType</span></span>|[<span data-ttu-id="92f26-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="92f26-197">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="92f26-198">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="92f26-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="92f26-199">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="92f26-199">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="92f26-200">可取值为：`open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="92f26-200">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="92f26-201">proxySettings</span><span class="sxs-lookup"><span data-stu-id="92f26-201">proxySettings</span></span>|[<span data-ttu-id="92f26-202">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="92f26-202">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="92f26-203">从[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)继承的此 wi-fi 连接的代理类型。</span><span class="sxs-lookup"><span data-stu-id="92f26-203">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="92f26-204">可取值为：`none`、`manual`、`automatic`。</span><span class="sxs-lookup"><span data-stu-id="92f26-204">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="92f26-205">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="92f26-205">proxyManualAddress</span></span>|<span data-ttu-id="92f26-206">String</span><span class="sxs-lookup"><span data-stu-id="92f26-206">String</span></span>|<span data-ttu-id="92f26-207">选择手动配置时代理服务器的 IP 地址或 DNS 主机名。</span><span class="sxs-lookup"><span data-stu-id="92f26-207">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="92f26-208">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-208">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f26-209">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="92f26-209">proxyManualPort</span></span>|<span data-ttu-id="92f26-210">Int32</span><span class="sxs-lookup"><span data-stu-id="92f26-210">Int32</span></span>|<span data-ttu-id="92f26-211">选择手动配置时代理服务器的端口。</span><span class="sxs-lookup"><span data-stu-id="92f26-211">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="92f26-212">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-212">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f26-213">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="92f26-213">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="92f26-214">String</span><span class="sxs-lookup"><span data-stu-id="92f26-214">String</span></span>|<span data-ttu-id="92f26-215">选择 "自动配置" 时代理服务器的 "自动配置" 脚本的 URL。</span><span class="sxs-lookup"><span data-stu-id="92f26-215">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="92f26-216">此 URL 通常是 PAC (代理自动配置) 文件的位置。</span><span class="sxs-lookup"><span data-stu-id="92f26-216">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="92f26-217">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-217">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f26-218">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="92f26-218">preSharedKey</span></span>|<span data-ttu-id="92f26-219">String</span><span class="sxs-lookup"><span data-stu-id="92f26-219">String</span></span>|<span data-ttu-id="92f26-220">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="92f26-220">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="92f26-221">继承自[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92f26-221">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="92f26-222">eapType</span><span class="sxs-lookup"><span data-stu-id="92f26-222">eapType</span></span>|[<span data-ttu-id="92f26-223">eapType</span><span class="sxs-lookup"><span data-stu-id="92f26-223">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="92f26-224">可扩展的身份验证协议 (EAP)。</span><span class="sxs-lookup"><span data-stu-id="92f26-224">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="92f26-225">指示 Wi-fi 终结点 (路由器) 上的 EAP 协议集的类型。</span><span class="sxs-lookup"><span data-stu-id="92f26-225">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="92f26-226">可取值为：`eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。</span><span class="sxs-lookup"><span data-stu-id="92f26-226">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="92f26-227">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="92f26-227">eapFastConfiguration</span></span>|[<span data-ttu-id="92f26-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="92f26-228">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="92f26-229">EAP-FAST 配置选项, 当 EAP-FAST 是所选的 EAP 类型时。</span><span class="sxs-lookup"><span data-stu-id="92f26-229">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="92f26-230">可取值为：`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously`。</span><span class="sxs-lookup"><span data-stu-id="92f26-230">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="92f26-231">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="92f26-231">trustedServerCertificateNames</span></span>|<span data-ttu-id="92f26-232">String collection</span><span class="sxs-lookup"><span data-stu-id="92f26-232">String collection</span></span>|<span data-ttu-id="92f26-233">将 EAP 类型配置为 EAP-TLS/TTLS/FAST 或 PEAP 时受信任的服务器证书名称。</span><span class="sxs-lookup"><span data-stu-id="92f26-233">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="92f26-234">这是由受信任的证书颁发机构 (CA) 颁发的证书中使用的公用名称。</span><span class="sxs-lookup"><span data-stu-id="92f26-234">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="92f26-235">如果提供此信息, 则可以绕过在最终用户的设备连接到此 Wi-fi 网络时显示的动态信任对话框。</span><span class="sxs-lookup"><span data-stu-id="92f26-235">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="92f26-236">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="92f26-236">authenticationMethod</span></span>|[<span data-ttu-id="92f26-237">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="92f26-237">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="92f26-238">EAP 类型配置为 PEAP 或 EAP-TTLS 时的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="92f26-238">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="92f26-239">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="92f26-239">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="92f26-240">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="92f26-240">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="92f26-241">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="92f26-241">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="92f26-242">EAP 类型为 EAP 时进行身份验证的非 EAP 方法-TTLS 和 Authenticationmethod 为用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="92f26-242">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="92f26-243">可取值为：`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo`。</span><span class="sxs-lookup"><span data-stu-id="92f26-243">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="92f26-244">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="92f26-244">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="92f26-245">String</span><span class="sxs-lookup"><span data-stu-id="92f26-245">String</span></span>|<span data-ttu-id="92f26-246">将 EAP 类型配置为 EAP-TTLS、EAP-FAST 或 PEAP 时启用标识隐私 (外部标识)。</span><span class="sxs-lookup"><span data-stu-id="92f26-246">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="92f26-247">此属性使用您输入的文本屏蔽用户名。</span><span class="sxs-lookup"><span data-stu-id="92f26-247">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="92f26-248">例如, 如果使用 "匿名", 则使用其真实用户名通过此 Wlan 连接进行身份验证的每个用户都将显示为 "匿名"。</span><span class="sxs-lookup"><span data-stu-id="92f26-248">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="92f26-249">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="92f26-249">usernameFormatString</span></span>|<span data-ttu-id="92f26-250">String</span><span class="sxs-lookup"><span data-stu-id="92f26-250">String</span></span>|<span data-ttu-id="92f26-251">用于生成用户名以连接到 wifi 的用户名格式字符串</span><span class="sxs-lookup"><span data-stu-id="92f26-251">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="92f26-252">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="92f26-252">passwordFormatString</span></span>|<span data-ttu-id="92f26-253">String</span><span class="sxs-lookup"><span data-stu-id="92f26-253">String</span></span>|<span data-ttu-id="92f26-254">用于生成密码以连接到 wifi 的密码格式字符串</span><span class="sxs-lookup"><span data-stu-id="92f26-254">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="92f26-255">响应</span><span class="sxs-lookup"><span data-stu-id="92f26-255">Response</span></span>
<span data-ttu-id="92f26-256">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="92f26-256">If successful, this method returns a `200 OK` response code and an updated [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92f26-257">示例</span><span class="sxs-lookup"><span data-stu-id="92f26-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="92f26-258">请求</span><span class="sxs-lookup"><span data-stu-id="92f26-258">Request</span></span>
<span data-ttu-id="92f26-259">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92f26-259">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="92f26-260">响应</span><span class="sxs-lookup"><span data-stu-id="92f26-260">Response</span></span>
<span data-ttu-id="92f26-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92f26-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





