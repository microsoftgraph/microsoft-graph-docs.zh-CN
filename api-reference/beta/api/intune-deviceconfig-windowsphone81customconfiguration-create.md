---
title: 创建 windowsPhone81CustomConfiguration
description: 创建新的 windowsPhone81CustomConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f0884f45199d2e6c480d9492589b2a5853c3e7dc
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178981"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="35f0e-103">创建 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="35f0e-103">Create windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="35f0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35f0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35f0e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35f0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35f0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35f0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35f0e-107">创建新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35f0e-107">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35f0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="35f0e-108">Prerequisites</span></span>
<span data-ttu-id="35f0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35f0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35f0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="35f0e-111">Permission type</span></span>|<span data-ttu-id="35f0e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35f0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35f0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35f0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35f0e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f0e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35f0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35f0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35f0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="35f0e-116">Not supported.</span></span>|
|<span data-ttu-id="35f0e-117">Application</span><span class="sxs-lookup"><span data-stu-id="35f0e-117">Application</span></span>|<span data-ttu-id="35f0e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f0e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35f0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35f0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="35f0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="35f0e-120">Request headers</span></span>
|<span data-ttu-id="35f0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="35f0e-121">Header</span></span>|<span data-ttu-id="35f0e-122">值</span><span class="sxs-lookup"><span data-stu-id="35f0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35f0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35f0e-123">Authorization</span></span>|<span data-ttu-id="35f0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35f0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35f0e-125">接受</span><span class="sxs-lookup"><span data-stu-id="35f0e-125">Accept</span></span>|<span data-ttu-id="35f0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35f0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="35f0e-127">Request body</span></span>
<span data-ttu-id="35f0e-128">在请求正文中，提供 windowsPhone81CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35f0e-128">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="35f0e-129">下表显示了创建 windowsPhone81CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="35f0e-129">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="35f0e-130">属性</span><span class="sxs-lookup"><span data-stu-id="35f0e-130">Property</span></span>|<span data-ttu-id="35f0e-131">类型</span><span class="sxs-lookup"><span data-stu-id="35f0e-131">Type</span></span>|<span data-ttu-id="35f0e-132">说明</span><span class="sxs-lookup"><span data-stu-id="35f0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35f0e-133">id</span><span class="sxs-lookup"><span data-stu-id="35f0e-133">id</span></span>|<span data-ttu-id="35f0e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="35f0e-134">String</span></span>|<span data-ttu-id="35f0e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="35f0e-135">Key of the entity.</span></span> <span data-ttu-id="35f0e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35f0e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="35f0e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f0e-138">DateTimeOffset</span></span>|<span data-ttu-id="35f0e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="35f0e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="35f0e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35f0e-141">roleScopeTagIds</span></span>|<span data-ttu-id="35f0e-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="35f0e-142">String collection</span></span>|<span data-ttu-id="35f0e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="35f0e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35f0e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="35f0e-145">supportsScopeTags</span></span>|<span data-ttu-id="35f0e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f0e-146">Boolean</span></span>|<span data-ttu-id="35f0e-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="35f0e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="35f0e-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="35f0e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="35f0e-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="35f0e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="35f0e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="35f0e-150">This property is read-only.</span></span> <span data-ttu-id="35f0e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="35f0e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="35f0e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="35f0e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="35f0e-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="35f0e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="35f0e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="35f0e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="35f0e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="35f0e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="35f0e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="35f0e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="35f0e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="35f0e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="35f0e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="35f0e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="35f0e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="35f0e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="35f0e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35f0e-164">createdDateTime</span></span>|<span data-ttu-id="35f0e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f0e-165">DateTimeOffset</span></span>|<span data-ttu-id="35f0e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="35f0e-166">DateTime the object was created.</span></span> <span data-ttu-id="35f0e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-168">说明</span><span class="sxs-lookup"><span data-stu-id="35f0e-168">description</span></span>|<span data-ttu-id="35f0e-169">String</span><span class="sxs-lookup"><span data-stu-id="35f0e-169">String</span></span>|<span data-ttu-id="35f0e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="35f0e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35f0e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="35f0e-172">displayName</span></span>|<span data-ttu-id="35f0e-173">String</span><span class="sxs-lookup"><span data-stu-id="35f0e-173">String</span></span>|<span data-ttu-id="35f0e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="35f0e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35f0e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-176">version</span><span class="sxs-lookup"><span data-stu-id="35f0e-176">version</span></span>|<span data-ttu-id="35f0e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="35f0e-177">Int32</span></span>|<span data-ttu-id="35f0e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="35f0e-178">Version of the device configuration.</span></span> <span data-ttu-id="35f0e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35f0e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35f0e-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="35f0e-180">omaSettings</span></span>|<span data-ttu-id="35f0e-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="35f0e-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="35f0e-182">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="35f0e-182">OMA settings.</span></span> <span data-ttu-id="35f0e-183">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="35f0e-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="35f0e-184">响应</span><span class="sxs-lookup"><span data-stu-id="35f0e-184">Response</span></span>
<span data-ttu-id="35f0e-185">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35f0e-185">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f0e-186">示例</span><span class="sxs-lookup"><span data-stu-id="35f0e-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="35f0e-187">请求</span><span class="sxs-lookup"><span data-stu-id="35f0e-187">Request</span></span>
<span data-ttu-id="35f0e-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35f0e-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1248

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="35f0e-189">响应</span><span class="sxs-lookup"><span data-stu-id="35f0e-189">Response</span></span>
<span data-ttu-id="35f0e-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35f0e-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1420

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```



