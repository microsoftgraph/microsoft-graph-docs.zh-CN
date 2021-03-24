---
title: 创建 windows81WifiImportConfiguration
description: 创建新的 windows81WifiImportConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f3d79634df501a9f9976d76c0ecaf6621b3d834
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136970"
---
# <a name="create-windows81wifiimportconfiguration"></a><span data-ttu-id="b5ec6-103">创建 windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5ec6-103">Create windows81WifiImportConfiguration</span></span>

<span data-ttu-id="b5ec6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5ec6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5ec6-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5ec6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5ec6-107">创建新的 [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-107">Create a new [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5ec6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5ec6-108">Prerequisites</span></span>
<span data-ttu-id="b5ec6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5ec6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5ec6-111">Permission type</span></span>|<span data-ttu-id="b5ec6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5ec6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5ec6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5ec6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5ec6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5ec6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5ec6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5ec6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5ec6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-116">Not supported.</span></span>|
|<span data-ttu-id="b5ec6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5ec6-117">Application</span></span>|<span data-ttu-id="b5ec6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5ec6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5ec6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5ec6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b5ec6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5ec6-120">Request headers</span></span>
|<span data-ttu-id="b5ec6-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5ec6-121">Header</span></span>|<span data-ttu-id="b5ec6-122">值</span><span class="sxs-lookup"><span data-stu-id="b5ec6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5ec6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5ec6-123">Authorization</span></span>|<span data-ttu-id="b5ec6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5ec6-125">接受</span><span class="sxs-lookup"><span data-stu-id="b5ec6-125">Accept</span></span>|<span data-ttu-id="b5ec6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5ec6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5ec6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5ec6-127">Request body</span></span>
<span data-ttu-id="b5ec6-128">在请求正文中，提供 windows81WifiImportConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-128">In the request body, supply a JSON representation for the windows81WifiImportConfiguration object.</span></span>

<span data-ttu-id="b5ec6-129">下表显示创建 windows81WifiImportConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-129">The following table shows the properties that are required when you create the windows81WifiImportConfiguration.</span></span>

|<span data-ttu-id="b5ec6-130">属性</span><span class="sxs-lookup"><span data-stu-id="b5ec6-130">Property</span></span>|<span data-ttu-id="b5ec6-131">类型</span><span class="sxs-lookup"><span data-stu-id="b5ec6-131">Type</span></span>|<span data-ttu-id="b5ec6-132">说明</span><span class="sxs-lookup"><span data-stu-id="b5ec6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5ec6-133">id</span><span class="sxs-lookup"><span data-stu-id="b5ec6-133">id</span></span>|<span data-ttu-id="b5ec6-134">String</span><span class="sxs-lookup"><span data-stu-id="b5ec6-134">String</span></span>|<span data-ttu-id="b5ec6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-135">Key of the entity.</span></span> <span data-ttu-id="b5ec6-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5ec6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b5ec6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5ec6-138">DateTimeOffset</span></span>|<span data-ttu-id="b5ec6-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b5ec6-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5ec6-141">roleScopeTagIds</span></span>|<span data-ttu-id="b5ec6-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b5ec6-142">String collection</span></span>|<span data-ttu-id="b5ec6-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5ec6-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b5ec6-145">supportsScopeTags</span></span>|<span data-ttu-id="b5ec6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5ec6-146">Boolean</span></span>|<span data-ttu-id="b5ec6-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b5ec6-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b5ec6-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b5ec6-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-150">This property is read-only.</span></span> <span data-ttu-id="b5ec6-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5ec6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b5ec6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5ec6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b5ec6-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b5ec6-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5ec6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b5ec6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5ec6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b5ec6-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b5ec6-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5ec6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b5ec6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5ec6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b5ec6-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b5ec6-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5ec6-164">createdDateTime</span></span>|<span data-ttu-id="b5ec6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5ec6-165">DateTimeOffset</span></span>|<span data-ttu-id="b5ec6-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-166">DateTime the object was created.</span></span> <span data-ttu-id="b5ec6-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-168">说明</span><span class="sxs-lookup"><span data-stu-id="b5ec6-168">description</span></span>|<span data-ttu-id="b5ec6-169">String</span><span class="sxs-lookup"><span data-stu-id="b5ec6-169">String</span></span>|<span data-ttu-id="b5ec6-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5ec6-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b5ec6-172">displayName</span></span>|<span data-ttu-id="b5ec6-173">String</span><span class="sxs-lookup"><span data-stu-id="b5ec6-173">String</span></span>|<span data-ttu-id="b5ec6-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5ec6-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-176">version</span><span class="sxs-lookup"><span data-stu-id="b5ec6-176">version</span></span>|<span data-ttu-id="b5ec6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b5ec6-177">Int32</span></span>|<span data-ttu-id="b5ec6-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-178">Version of the device configuration.</span></span> <span data-ttu-id="b5ec6-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5ec6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5ec6-180">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="b5ec6-180">payloadFileName</span></span>|<span data-ttu-id="b5ec6-181">String</span><span class="sxs-lookup"><span data-stu-id="b5ec6-181">String</span></span>|<span data-ttu-id="b5ec6-182">有效负载文件名 (\*.xml) 。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-182">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="b5ec6-183">profileName</span><span class="sxs-lookup"><span data-stu-id="b5ec6-183">profileName</span></span>|<span data-ttu-id="b5ec6-184">String</span><span class="sxs-lookup"><span data-stu-id="b5ec6-184">String</span></span>|<span data-ttu-id="b5ec6-185">UI 中显示的配置文件名称。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-185">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="b5ec6-186">payload</span><span class="sxs-lookup"><span data-stu-id="b5ec6-186">payload</span></span>|<span data-ttu-id="b5ec6-187">Binary</span><span class="sxs-lookup"><span data-stu-id="b5ec6-187">Binary</span></span>|<span data-ttu-id="b5ec6-188">有效负载。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-188">Payload.</span></span> <span data-ttu-id="b5ec6-189"> (UTF8 编码的字节数组) 。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-189">(UTF8 encoded byte array).</span></span> <span data-ttu-id="b5ec6-190">这是保存在用于连接到 Wi-Fi 终结点的 XML 文件。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-190">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="b5ec6-191">响应</span><span class="sxs-lookup"><span data-stu-id="b5ec6-191">Response</span></span>
<span data-ttu-id="b5ec6-192">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-192">If successful, this method returns a `201 Created` response code and a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5ec6-193">示例</span><span class="sxs-lookup"><span data-stu-id="b5ec6-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5ec6-194">请求</span><span class="sxs-lookup"><span data-stu-id="b5ec6-194">Request</span></span>
<span data-ttu-id="b5ec6-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1154

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="b5ec6-196">响应</span><span class="sxs-lookup"><span data-stu-id="b5ec6-196">Response</span></span>
<span data-ttu-id="b5ec6-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5ec6-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1326

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
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
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```




