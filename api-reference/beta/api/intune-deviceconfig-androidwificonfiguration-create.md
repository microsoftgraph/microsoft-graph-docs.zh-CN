---
title: 创建 androidWiFiConfiguration
description: 创建新的 androidWiFiConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3acaa21e2369c428ccb114e56f0d74df10774f23
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698930"
---
# <a name="create-androidwificonfiguration"></a><span data-ttu-id="5e740-103">创建 androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e740-103">Create androidWiFiConfiguration</span></span>

<span data-ttu-id="5e740-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e740-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e740-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e740-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e740-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e740-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e740-107">创建新的 [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e740-107">Create a new [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e740-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5e740-108">Prerequisites</span></span>
<span data-ttu-id="5e740-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e740-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e740-111">Permission type</span></span>|<span data-ttu-id="5e740-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5e740-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e740-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e740-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e740-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e740-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5e740-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e740-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e740-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e740-116">Not supported.</span></span>|
|<span data-ttu-id="5e740-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e740-117">Application</span></span>|<span data-ttu-id="5e740-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e740-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e740-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e740-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5e740-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e740-120">Request headers</span></span>
|<span data-ttu-id="5e740-121">标头</span><span class="sxs-lookup"><span data-stu-id="5e740-121">Header</span></span>|<span data-ttu-id="5e740-122">值</span><span class="sxs-lookup"><span data-stu-id="5e740-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e740-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e740-123">Authorization</span></span>|<span data-ttu-id="5e740-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5e740-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e740-125">接受</span><span class="sxs-lookup"><span data-stu-id="5e740-125">Accept</span></span>|<span data-ttu-id="5e740-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e740-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e740-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e740-127">Request body</span></span>
<span data-ttu-id="5e740-128">在请求正文中，提供 androidWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e740-128">In the request body, supply a JSON representation for the androidWiFiConfiguration object.</span></span>

<span data-ttu-id="5e740-129">下表显示创建 androidWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5e740-129">The following table shows the properties that are required when you create the androidWiFiConfiguration.</span></span>

|<span data-ttu-id="5e740-130">属性</span><span class="sxs-lookup"><span data-stu-id="5e740-130">Property</span></span>|<span data-ttu-id="5e740-131">类型</span><span class="sxs-lookup"><span data-stu-id="5e740-131">Type</span></span>|<span data-ttu-id="5e740-132">说明</span><span class="sxs-lookup"><span data-stu-id="5e740-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e740-133">id</span><span class="sxs-lookup"><span data-stu-id="5e740-133">id</span></span>|<span data-ttu-id="5e740-134">String</span><span class="sxs-lookup"><span data-stu-id="5e740-134">String</span></span>|<span data-ttu-id="5e740-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5e740-135">Key of the entity.</span></span> <span data-ttu-id="5e740-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e740-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5e740-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e740-138">DateTimeOffset</span></span>|<span data-ttu-id="5e740-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5e740-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5e740-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5e740-141">roleScopeTagIds</span></span>|<span data-ttu-id="5e740-142">String collection</span><span class="sxs-lookup"><span data-stu-id="5e740-142">String collection</span></span>|<span data-ttu-id="5e740-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5e740-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5e740-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5e740-145">supportsScopeTags</span></span>|<span data-ttu-id="5e740-146">布尔</span><span class="sxs-lookup"><span data-stu-id="5e740-146">Boolean</span></span>|<span data-ttu-id="5e740-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5e740-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5e740-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5e740-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5e740-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5e740-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5e740-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5e740-150">This property is read-only.</span></span> <span data-ttu-id="5e740-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5e740-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5e740-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5e740-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5e740-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5e740-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5e740-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5e740-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5e740-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5e740-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5e740-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5e740-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5e740-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5e740-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5e740-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5e740-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5e740-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5e740-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5e740-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e740-164">createdDateTime</span></span>|<span data-ttu-id="5e740-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e740-165">DateTimeOffset</span></span>|<span data-ttu-id="5e740-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5e740-166">DateTime the object was created.</span></span> <span data-ttu-id="5e740-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-168">说明</span><span class="sxs-lookup"><span data-stu-id="5e740-168">description</span></span>|<span data-ttu-id="5e740-169">String</span><span class="sxs-lookup"><span data-stu-id="5e740-169">String</span></span>|<span data-ttu-id="5e740-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5e740-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5e740-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5e740-172">displayName</span></span>|<span data-ttu-id="5e740-173">String</span><span class="sxs-lookup"><span data-stu-id="5e740-173">String</span></span>|<span data-ttu-id="5e740-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5e740-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5e740-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-176">version</span><span class="sxs-lookup"><span data-stu-id="5e740-176">version</span></span>|<span data-ttu-id="5e740-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5e740-177">Int32</span></span>|<span data-ttu-id="5e740-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5e740-178">Version of the device configuration.</span></span> <span data-ttu-id="5e740-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5e740-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5e740-180">networkName</span><span class="sxs-lookup"><span data-stu-id="5e740-180">networkName</span></span>|<span data-ttu-id="5e740-181">String</span><span class="sxs-lookup"><span data-stu-id="5e740-181">String</span></span>|<span data-ttu-id="5e740-182">网络名称</span><span class="sxs-lookup"><span data-stu-id="5e740-182">Network Name</span></span>|
|<span data-ttu-id="5e740-183">ssid</span><span class="sxs-lookup"><span data-stu-id="5e740-183">ssid</span></span>|<span data-ttu-id="5e740-184">String</span><span class="sxs-lookup"><span data-stu-id="5e740-184">String</span></span>|<span data-ttu-id="5e740-185">这是广播到所有设备的 Wi-Fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="5e740-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="5e740-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="5e740-186">connectAutomatically</span></span>|<span data-ttu-id="5e740-187">布尔</span><span class="sxs-lookup"><span data-stu-id="5e740-187">Boolean</span></span>|<span data-ttu-id="5e740-188">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="5e740-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="5e740-189">将此设置为 true 将跳过用户提示，并自动将设备连接到 Wi-Fi 网络。</span><span class="sxs-lookup"><span data-stu-id="5e740-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="5e740-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="5e740-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="5e740-191">布尔</span><span class="sxs-lookup"><span data-stu-id="5e740-191">Boolean</span></span>|<span data-ttu-id="5e740-192">当设置为 true 时，此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="5e740-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="5e740-193">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="5e740-193">wiFiSecurityType</span></span>|[<span data-ttu-id="5e740-194">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="5e740-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="5e740-195">指示 Wi-Fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="5e740-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="5e740-196">可取值为：`open`、`wpaEnterprise`、`wpa2Enterprise`。</span><span class="sxs-lookup"><span data-stu-id="5e740-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="5e740-197">响应</span><span class="sxs-lookup"><span data-stu-id="5e740-197">Response</span></span>
<span data-ttu-id="5e740-198">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e740-198">If successful, this method returns a `201 Created` response code and a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e740-199">示例</span><span class="sxs-lookup"><span data-stu-id="5e740-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e740-200">请求</span><span class="sxs-lookup"><span data-stu-id="5e740-200">Request</span></span>
<span data-ttu-id="5e740-201">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e740-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1208

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="5e740-202">响应</span><span class="sxs-lookup"><span data-stu-id="5e740-202">Response</span></span>
<span data-ttu-id="5e740-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e740-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1380

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
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





