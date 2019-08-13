---
title: 更新 windowsPhone81CustomConfiguration
description: 更新 windowsPhone81CustomConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 771e7472087ad384761833b1d13a4137660f283b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344173"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="0fa55-103">更新 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="0fa55-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="0fa55-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0fa55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fa55-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fa55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fa55-106">更新 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0fa55-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fa55-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0fa55-107">Prerequisites</span></span>
<span data-ttu-id="0fa55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fa55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fa55-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fa55-110">Permission type</span></span>|<span data-ttu-id="0fa55-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0fa55-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fa55-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa55-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fa55-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa55-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fa55-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fa55-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fa55-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fa55-115">Not supported.</span></span>|
|<span data-ttu-id="0fa55-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fa55-116">Application</span></span>|<span data-ttu-id="0fa55-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fa55-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fa55-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fa55-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0fa55-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fa55-119">Request headers</span></span>
|<span data-ttu-id="0fa55-120">标头</span><span class="sxs-lookup"><span data-stu-id="0fa55-120">Header</span></span>|<span data-ttu-id="0fa55-121">值</span><span class="sxs-lookup"><span data-stu-id="0fa55-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fa55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fa55-122">Authorization</span></span>|<span data-ttu-id="0fa55-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0fa55-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fa55-124">接受</span><span class="sxs-lookup"><span data-stu-id="0fa55-124">Accept</span></span>|<span data-ttu-id="0fa55-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0fa55-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fa55-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fa55-126">Request body</span></span>
<span data-ttu-id="0fa55-127">在请求正文中，提供 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fa55-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="0fa55-128">下表显示了创建 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0fa55-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="0fa55-129">属性</span><span class="sxs-lookup"><span data-stu-id="0fa55-129">Property</span></span>|<span data-ttu-id="0fa55-130">类型</span><span class="sxs-lookup"><span data-stu-id="0fa55-130">Type</span></span>|<span data-ttu-id="0fa55-131">说明</span><span class="sxs-lookup"><span data-stu-id="0fa55-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa55-132">id</span><span class="sxs-lookup"><span data-stu-id="0fa55-132">id</span></span>|<span data-ttu-id="0fa55-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0fa55-133">String</span></span>|<span data-ttu-id="0fa55-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0fa55-134">Key of the entity.</span></span> <span data-ttu-id="0fa55-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fa55-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0fa55-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa55-137">DateTimeOffset</span></span>|<span data-ttu-id="0fa55-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0fa55-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0fa55-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0fa55-140">roleScopeTagIds</span></span>|<span data-ttu-id="0fa55-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0fa55-141">String collection</span></span>|<span data-ttu-id="0fa55-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0fa55-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0fa55-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0fa55-144">supportsScopeTags</span></span>|<span data-ttu-id="0fa55-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fa55-145">Boolean</span></span>|<span data-ttu-id="0fa55-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="0fa55-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0fa55-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="0fa55-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0fa55-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="0fa55-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0fa55-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0fa55-149">This property is read-only.</span></span> <span data-ttu-id="0fa55-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0fa55-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0fa55-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0fa55-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0fa55-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="0fa55-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0fa55-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0fa55-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0fa55-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0fa55-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0fa55-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0fa55-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0fa55-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0fa55-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0fa55-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0fa55-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0fa55-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0fa55-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0fa55-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fa55-163">createdDateTime</span></span>|<span data-ttu-id="0fa55-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fa55-164">DateTimeOffset</span></span>|<span data-ttu-id="0fa55-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0fa55-165">DateTime the object was created.</span></span> <span data-ttu-id="0fa55-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-167">说明</span><span class="sxs-lookup"><span data-stu-id="0fa55-167">description</span></span>|<span data-ttu-id="0fa55-168">String</span><span class="sxs-lookup"><span data-stu-id="0fa55-168">String</span></span>|<span data-ttu-id="0fa55-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0fa55-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0fa55-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0fa55-171">displayName</span></span>|<span data-ttu-id="0fa55-172">String</span><span class="sxs-lookup"><span data-stu-id="0fa55-172">String</span></span>|<span data-ttu-id="0fa55-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0fa55-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0fa55-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-175">version</span><span class="sxs-lookup"><span data-stu-id="0fa55-175">version</span></span>|<span data-ttu-id="0fa55-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0fa55-176">Int32</span></span>|<span data-ttu-id="0fa55-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0fa55-177">Version of the device configuration.</span></span> <span data-ttu-id="0fa55-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0fa55-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0fa55-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="0fa55-179">omaSettings</span></span>|<span data-ttu-id="0fa55-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0fa55-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="0fa55-181">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="0fa55-181">OMA settings.</span></span> <span data-ttu-id="0fa55-182">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0fa55-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0fa55-183">响应</span><span class="sxs-lookup"><span data-stu-id="0fa55-183">Response</span></span>
<span data-ttu-id="0fa55-184">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fa55-184">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fa55-185">示例</span><span class="sxs-lookup"><span data-stu-id="0fa55-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fa55-186">请求</span><span class="sxs-lookup"><span data-stu-id="0fa55-186">Request</span></span>
<span data-ttu-id="0fa55-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0fa55-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1301

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
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0fa55-188">响应</span><span class="sxs-lookup"><span data-stu-id="0fa55-188">Response</span></span>
<span data-ttu-id="0fa55-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0fa55-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1473

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
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```






