---
title: 更新 windows10NetworkBoundaryConfiguration
description: 更新 windows10NetworkBoundaryConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 789c366ee219104e9f0e17080771c580725f8981
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127611"
---
# <a name="update-windows10networkboundaryconfiguration"></a><span data-ttu-id="ca117-103">更新 windows10NetworkBoundaryConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca117-103">Update windows10NetworkBoundaryConfiguration</span></span>

<span data-ttu-id="ca117-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca117-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca117-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca117-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca117-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca117-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca117-107">更新 [windows10NetworkBoundaryConfiguration 对象](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="ca117-107">Update the properties of a [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca117-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca117-108">Prerequisites</span></span>
<span data-ttu-id="ca117-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca117-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca117-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca117-111">Permission type</span></span>|<span data-ttu-id="ca117-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca117-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca117-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca117-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca117-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca117-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca117-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca117-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca117-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca117-116">Not supported.</span></span>|
|<span data-ttu-id="ca117-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca117-117">Application</span></span>|<span data-ttu-id="ca117-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca117-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca117-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca117-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ca117-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca117-120">Request headers</span></span>
|<span data-ttu-id="ca117-121">标头</span><span class="sxs-lookup"><span data-stu-id="ca117-121">Header</span></span>|<span data-ttu-id="ca117-122">值</span><span class="sxs-lookup"><span data-stu-id="ca117-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca117-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca117-123">Authorization</span></span>|<span data-ttu-id="ca117-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca117-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca117-125">接受</span><span class="sxs-lookup"><span data-stu-id="ca117-125">Accept</span></span>|<span data-ttu-id="ca117-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca117-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca117-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca117-127">Request body</span></span>
<span data-ttu-id="ca117-128">在请求正文中，提供 [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca117-128">In the request body, supply a JSON representation for the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object.</span></span>

<span data-ttu-id="ca117-129">下表显示创建 [windows10NetworkBoundaryConfiguration 时所需的属性](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ca117-129">The following table shows the properties that are required when you create the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md).</span></span>

|<span data-ttu-id="ca117-130">属性</span><span class="sxs-lookup"><span data-stu-id="ca117-130">Property</span></span>|<span data-ttu-id="ca117-131">类型</span><span class="sxs-lookup"><span data-stu-id="ca117-131">Type</span></span>|<span data-ttu-id="ca117-132">说明</span><span class="sxs-lookup"><span data-stu-id="ca117-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca117-133">id</span><span class="sxs-lookup"><span data-stu-id="ca117-133">id</span></span>|<span data-ttu-id="ca117-134">String</span><span class="sxs-lookup"><span data-stu-id="ca117-134">String</span></span>|<span data-ttu-id="ca117-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ca117-135">Key of the entity.</span></span> <span data-ttu-id="ca117-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca117-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ca117-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca117-138">DateTimeOffset</span></span>|<span data-ttu-id="ca117-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ca117-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ca117-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca117-141">roleScopeTagIds</span></span>|<span data-ttu-id="ca117-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ca117-142">String collection</span></span>|<span data-ttu-id="ca117-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ca117-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca117-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ca117-145">supportsScopeTags</span></span>|<span data-ttu-id="ca117-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca117-146">Boolean</span></span>|<span data-ttu-id="ca117-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="ca117-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ca117-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="ca117-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ca117-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="ca117-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ca117-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ca117-150">This property is read-only.</span></span> <span data-ttu-id="ca117-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ca117-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ca117-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ca117-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ca117-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="ca117-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ca117-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ca117-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ca117-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ca117-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ca117-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ca117-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ca117-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ca117-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ca117-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ca117-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ca117-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ca117-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ca117-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca117-164">createdDateTime</span></span>|<span data-ttu-id="ca117-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca117-165">DateTimeOffset</span></span>|<span data-ttu-id="ca117-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ca117-166">DateTime the object was created.</span></span> <span data-ttu-id="ca117-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-168">说明</span><span class="sxs-lookup"><span data-stu-id="ca117-168">description</span></span>|<span data-ttu-id="ca117-169">String</span><span class="sxs-lookup"><span data-stu-id="ca117-169">String</span></span>|<span data-ttu-id="ca117-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ca117-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca117-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ca117-172">displayName</span></span>|<span data-ttu-id="ca117-173">String</span><span class="sxs-lookup"><span data-stu-id="ca117-173">String</span></span>|<span data-ttu-id="ca117-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ca117-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca117-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-176">version</span><span class="sxs-lookup"><span data-stu-id="ca117-176">version</span></span>|<span data-ttu-id="ca117-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ca117-177">Int32</span></span>|<span data-ttu-id="ca117-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ca117-178">Version of the device configuration.</span></span> <span data-ttu-id="ca117-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca117-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca117-180">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="ca117-180">windowsNetworkIsolationPolicy</span></span>|[<span data-ttu-id="ca117-181">windowsNetworkIsolationPolicy</span><span class="sxs-lookup"><span data-stu-id="ca117-181">windowsNetworkIsolationPolicy</span></span>](../resources/intune-deviceconfig-windowsnetworkisolationpolicy.md)|<span data-ttu-id="ca117-182">Windows 网络隔离策略</span><span class="sxs-lookup"><span data-stu-id="ca117-182">Windows Network Isolation Policy</span></span>|



## <a name="response"></a><span data-ttu-id="ca117-183">响应</span><span class="sxs-lookup"><span data-stu-id="ca117-183">Response</span></span>
<span data-ttu-id="ca117-184">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca117-184">If successful, this method returns a `200 OK` response code and an updated [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca117-185">示例</span><span class="sxs-lookup"><span data-stu-id="ca117-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca117-186">请求</span><span class="sxs-lookup"><span data-stu-id="ca117-186">Request</span></span>
<span data-ttu-id="ca117-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca117-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1919

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
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
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.ipRange"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="ca117-188">响应</span><span class="sxs-lookup"><span data-stu-id="ca117-188">Response</span></span>
<span data-ttu-id="ca117-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca117-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2091

{
  "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
  "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
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
  "windowsNetworkIsolationPolicy": {
    "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
    "enterpriseNetworkDomainNames": [
      "Enterprise Network Domain Names value"
    ],
    "enterpriseCloudResources": [
      {
        "@odata.type": "microsoft.graph.proxiedDomain",
        "ipAddressOrFQDN": "Ip Address Or FQDN value",
        "proxy": "Proxy value"
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.ipRange"
      }
    ],
    "enterpriseInternalProxyServers": [
      "Enterprise Internal Proxy Servers value"
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      "Enterprise Proxy Servers value"
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      "Neutral Domain Resources value"
    ]
  }
}
```




