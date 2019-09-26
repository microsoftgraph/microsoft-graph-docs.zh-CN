---
title: 更新 androidForWorkWiFiConfiguration
description: 更新 androidForWorkWiFiConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 53a0b512dc3ba47a2f84059b85b0bdf831873498
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37169214"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="dd41d-103">更新 androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="dd41d-103">Update androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="dd41d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd41d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd41d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd41d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd41d-106">更新[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dd41d-106">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd41d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd41d-107">Prerequisites</span></span>
<span data-ttu-id="dd41d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd41d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd41d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd41d-110">Permission type</span></span>|<span data-ttu-id="dd41d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dd41d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd41d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd41d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd41d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd41d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd41d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd41d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd41d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd41d-115">Not supported.</span></span>|
|<span data-ttu-id="dd41d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd41d-116">Application</span></span>|<span data-ttu-id="dd41d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd41d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd41d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd41d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dd41d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd41d-119">Request headers</span></span>
|<span data-ttu-id="dd41d-120">标头</span><span class="sxs-lookup"><span data-stu-id="dd41d-120">Header</span></span>|<span data-ttu-id="dd41d-121">值</span><span class="sxs-lookup"><span data-stu-id="dd41d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd41d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd41d-122">Authorization</span></span>|<span data-ttu-id="dd41d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd41d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd41d-124">接受</span><span class="sxs-lookup"><span data-stu-id="dd41d-124">Accept</span></span>|<span data-ttu-id="dd41d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd41d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd41d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd41d-126">Request body</span></span>
<span data-ttu-id="dd41d-127">在请求正文中，提供[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd41d-127">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="dd41d-128">下表显示创建[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dd41d-128">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="dd41d-129">属性</span><span class="sxs-lookup"><span data-stu-id="dd41d-129">Property</span></span>|<span data-ttu-id="dd41d-130">类型</span><span class="sxs-lookup"><span data-stu-id="dd41d-130">Type</span></span>|<span data-ttu-id="dd41d-131">说明</span><span class="sxs-lookup"><span data-stu-id="dd41d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd41d-132">id</span><span class="sxs-lookup"><span data-stu-id="dd41d-132">id</span></span>|<span data-ttu-id="dd41d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="dd41d-133">String</span></span>|<span data-ttu-id="dd41d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dd41d-134">Key of the entity.</span></span> <span data-ttu-id="dd41d-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd41d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dd41d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd41d-137">DateTimeOffset</span></span>|<span data-ttu-id="dd41d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dd41d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dd41d-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd41d-140">roleScopeTagIds</span></span>|<span data-ttu-id="dd41d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="dd41d-141">String collection</span></span>|<span data-ttu-id="dd41d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="dd41d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dd41d-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dd41d-144">supportsScopeTags</span></span>|<span data-ttu-id="dd41d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd41d-145">Boolean</span></span>|<span data-ttu-id="dd41d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="dd41d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dd41d-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="dd41d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dd41d-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="dd41d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dd41d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dd41d-149">This property is read-only.</span></span> <span data-ttu-id="dd41d-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dd41d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="dd41d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dd41d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="dd41d-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="dd41d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="dd41d-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dd41d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="dd41d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dd41d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="dd41d-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="dd41d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="dd41d-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dd41d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="dd41d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dd41d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="dd41d-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="dd41d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="dd41d-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd41d-163">createdDateTime</span></span>|<span data-ttu-id="dd41d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd41d-164">DateTimeOffset</span></span>|<span data-ttu-id="dd41d-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dd41d-165">DateTime the object was created.</span></span> <span data-ttu-id="dd41d-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-167">说明</span><span class="sxs-lookup"><span data-stu-id="dd41d-167">description</span></span>|<span data-ttu-id="dd41d-168">String</span><span class="sxs-lookup"><span data-stu-id="dd41d-168">String</span></span>|<span data-ttu-id="dd41d-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="dd41d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dd41d-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="dd41d-171">displayName</span></span>|<span data-ttu-id="dd41d-172">String</span><span class="sxs-lookup"><span data-stu-id="dd41d-172">String</span></span>|<span data-ttu-id="dd41d-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="dd41d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dd41d-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-175">version</span><span class="sxs-lookup"><span data-stu-id="dd41d-175">version</span></span>|<span data-ttu-id="dd41d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="dd41d-176">Int32</span></span>|<span data-ttu-id="dd41d-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="dd41d-177">Version of the device configuration.</span></span> <span data-ttu-id="dd41d-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dd41d-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dd41d-179">networkName</span><span class="sxs-lookup"><span data-stu-id="dd41d-179">networkName</span></span>|<span data-ttu-id="dd41d-180">String</span><span class="sxs-lookup"><span data-stu-id="dd41d-180">String</span></span>|<span data-ttu-id="dd41d-181">网络名称</span><span class="sxs-lookup"><span data-stu-id="dd41d-181">Network Name</span></span>|
|<span data-ttu-id="dd41d-182">ssid</span><span class="sxs-lookup"><span data-stu-id="dd41d-182">ssid</span></span>|<span data-ttu-id="dd41d-183">String</span><span class="sxs-lookup"><span data-stu-id="dd41d-183">String</span></span>|<span data-ttu-id="dd41d-184">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="dd41d-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="dd41d-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="dd41d-185">connectAutomatically</span></span>|<span data-ttu-id="dd41d-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd41d-186">Boolean</span></span>|<span data-ttu-id="dd41d-187">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="dd41d-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="dd41d-188">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="dd41d-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="dd41d-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="dd41d-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="dd41d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd41d-190">Boolean</span></span>|<span data-ttu-id="dd41d-191">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="dd41d-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="dd41d-192">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="dd41d-192">wiFiSecurityType</span></span>|[<span data-ttu-id="dd41d-193">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="dd41d-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="dd41d-194">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="dd41d-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="dd41d-195">可取值为：`open`、`wpaEnterprise`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="dd41d-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="dd41d-196">响应</span><span class="sxs-lookup"><span data-stu-id="dd41d-196">Response</span></span>
<span data-ttu-id="dd41d-197">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dd41d-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd41d-198">示例</span><span class="sxs-lookup"><span data-stu-id="dd41d-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd41d-199">请求</span><span class="sxs-lookup"><span data-stu-id="dd41d-199">Request</span></span>
<span data-ttu-id="dd41d-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd41d-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1215

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="dd41d-201">响应</span><span class="sxs-lookup"><span data-stu-id="dd41d-201">Response</span></span>
<span data-ttu-id="dd41d-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd41d-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1387

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```




