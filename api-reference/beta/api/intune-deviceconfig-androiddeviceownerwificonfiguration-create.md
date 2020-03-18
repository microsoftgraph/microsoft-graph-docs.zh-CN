---
title: 创建 androidDeviceOwnerWiFiConfiguration
description: 创建新的 androidDeviceOwnerWiFiConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4343f5b4d3d82d847f0fa7796eae18b5dd15b153
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759645"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="0601b-103">创建 androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="0601b-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="0601b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0601b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0601b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0601b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0601b-106">创建新的[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0601b-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0601b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0601b-107">Prerequisites</span></span>
<span data-ttu-id="0601b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0601b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0601b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0601b-110">Permission type</span></span>|<span data-ttu-id="0601b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0601b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0601b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0601b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0601b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0601b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0601b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0601b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0601b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0601b-115">Not supported.</span></span>|
|<span data-ttu-id="0601b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0601b-116">Application</span></span>|<span data-ttu-id="0601b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0601b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0601b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0601b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0601b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0601b-119">Request headers</span></span>
|<span data-ttu-id="0601b-120">标头</span><span class="sxs-lookup"><span data-stu-id="0601b-120">Header</span></span>|<span data-ttu-id="0601b-121">值</span><span class="sxs-lookup"><span data-stu-id="0601b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0601b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0601b-122">Authorization</span></span>|<span data-ttu-id="0601b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0601b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0601b-124">接受</span><span class="sxs-lookup"><span data-stu-id="0601b-124">Accept</span></span>|<span data-ttu-id="0601b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0601b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0601b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0601b-126">Request body</span></span>
<span data-ttu-id="0601b-127">在请求正文中，提供 androidDeviceOwnerWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0601b-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="0601b-128">下表显示创建 androidDeviceOwnerWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0601b-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="0601b-129">属性</span><span class="sxs-lookup"><span data-stu-id="0601b-129">Property</span></span>|<span data-ttu-id="0601b-130">类型</span><span class="sxs-lookup"><span data-stu-id="0601b-130">Type</span></span>|<span data-ttu-id="0601b-131">说明</span><span class="sxs-lookup"><span data-stu-id="0601b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0601b-132">id</span><span class="sxs-lookup"><span data-stu-id="0601b-132">id</span></span>|<span data-ttu-id="0601b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0601b-133">String</span></span>|<span data-ttu-id="0601b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0601b-134">Key of the entity.</span></span> <span data-ttu-id="0601b-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0601b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0601b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0601b-137">DateTimeOffset</span></span>|<span data-ttu-id="0601b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0601b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0601b-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0601b-140">roleScopeTagIds</span></span>|<span data-ttu-id="0601b-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0601b-141">String collection</span></span>|<span data-ttu-id="0601b-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0601b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0601b-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0601b-144">supportsScopeTags</span></span>|<span data-ttu-id="0601b-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="0601b-145">Boolean</span></span>|<span data-ttu-id="0601b-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0601b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0601b-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0601b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0601b-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0601b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0601b-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0601b-149">This property is read-only.</span></span> <span data-ttu-id="0601b-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0601b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0601b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0601b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0601b-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0601b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0601b-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0601b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0601b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0601b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0601b-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0601b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0601b-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0601b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0601b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0601b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0601b-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0601b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0601b-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0601b-163">createdDateTime</span></span>|<span data-ttu-id="0601b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0601b-164">DateTimeOffset</span></span>|<span data-ttu-id="0601b-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0601b-165">DateTime the object was created.</span></span> <span data-ttu-id="0601b-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-167">说明</span><span class="sxs-lookup"><span data-stu-id="0601b-167">description</span></span>|<span data-ttu-id="0601b-168">String</span><span class="sxs-lookup"><span data-stu-id="0601b-168">String</span></span>|<span data-ttu-id="0601b-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0601b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0601b-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0601b-171">displayName</span></span>|<span data-ttu-id="0601b-172">String</span><span class="sxs-lookup"><span data-stu-id="0601b-172">String</span></span>|<span data-ttu-id="0601b-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0601b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0601b-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-175">version</span><span class="sxs-lookup"><span data-stu-id="0601b-175">version</span></span>|<span data-ttu-id="0601b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0601b-176">Int32</span></span>|<span data-ttu-id="0601b-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0601b-177">Version of the device configuration.</span></span> <span data-ttu-id="0601b-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0601b-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0601b-179">networkName</span><span class="sxs-lookup"><span data-stu-id="0601b-179">networkName</span></span>|<span data-ttu-id="0601b-180">String</span><span class="sxs-lookup"><span data-stu-id="0601b-180">String</span></span>|<span data-ttu-id="0601b-181">网络名称</span><span class="sxs-lookup"><span data-stu-id="0601b-181">Network Name</span></span>|
|<span data-ttu-id="0601b-182">ssid</span><span class="sxs-lookup"><span data-stu-id="0601b-182">ssid</span></span>|<span data-ttu-id="0601b-183">String</span><span class="sxs-lookup"><span data-stu-id="0601b-183">String</span></span>|<span data-ttu-id="0601b-184">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="0601b-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="0601b-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="0601b-185">connectAutomatically</span></span>|<span data-ttu-id="0601b-186">布尔值</span><span class="sxs-lookup"><span data-stu-id="0601b-186">Boolean</span></span>|<span data-ttu-id="0601b-187">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="0601b-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="0601b-188">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="0601b-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="0601b-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0601b-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0601b-190">布尔值</span><span class="sxs-lookup"><span data-stu-id="0601b-190">Boolean</span></span>|<span data-ttu-id="0601b-191">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="0601b-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="0601b-192">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0601b-192">wiFiSecurityType</span></span>|[<span data-ttu-id="0601b-193">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0601b-193">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="0601b-194">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="0601b-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="0601b-195">可取值为：`open`、`wep`、`wpaPersonal`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="0601b-195">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="0601b-196">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="0601b-196">preSharedKey</span></span>|<span data-ttu-id="0601b-197">String</span><span class="sxs-lookup"><span data-stu-id="0601b-197">String</span></span>|<span data-ttu-id="0601b-198">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="0601b-198">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="0601b-199">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="0601b-199">preSharedKeyIsSet</span></span>|<span data-ttu-id="0601b-200">布尔值</span><span class="sxs-lookup"><span data-stu-id="0601b-200">Boolean</span></span>|<span data-ttu-id="0601b-201">这是 WPA 个人 Wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="0601b-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="0601b-202">响应</span><span class="sxs-lookup"><span data-stu-id="0601b-202">Response</span></span>
<span data-ttu-id="0601b-203">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0601b-203">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0601b-204">示例</span><span class="sxs-lookup"><span data-stu-id="0601b-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="0601b-205">请求</span><span class="sxs-lookup"><span data-stu-id="0601b-205">Request</span></span>
<span data-ttu-id="0601b-206">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0601b-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1282

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="0601b-207">响应</span><span class="sxs-lookup"><span data-stu-id="0601b-207">Response</span></span>
<span data-ttu-id="0601b-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0601b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1454

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```




