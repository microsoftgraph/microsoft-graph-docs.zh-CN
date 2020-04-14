---
title: 创建 androidCustomConfiguration
description: 创建新的 androidCustomConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8ec14e12619afaa43957c341e734d58b67e28a3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43352478"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="f5407-103">创建 androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5407-103">Create androidCustomConfiguration</span></span>

<span data-ttu-id="f5407-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5407-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5407-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5407-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5407-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5407-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5407-107">创建新的 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5407-107">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5407-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5407-108">Prerequisites</span></span>
<span data-ttu-id="f5407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5407-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5407-111">Permission type</span></span>|<span data-ttu-id="f5407-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5407-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5407-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5407-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5407-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5407-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5407-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5407-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5407-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5407-116">Not supported.</span></span>|
|<span data-ttu-id="f5407-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5407-117">Application</span></span>|<span data-ttu-id="f5407-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5407-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5407-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5407-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f5407-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5407-120">Request headers</span></span>
|<span data-ttu-id="f5407-121">标头</span><span class="sxs-lookup"><span data-stu-id="f5407-121">Header</span></span>|<span data-ttu-id="f5407-122">值</span><span class="sxs-lookup"><span data-stu-id="f5407-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5407-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5407-123">Authorization</span></span>|<span data-ttu-id="f5407-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5407-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5407-125">接受</span><span class="sxs-lookup"><span data-stu-id="f5407-125">Accept</span></span>|<span data-ttu-id="f5407-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5407-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5407-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5407-127">Request body</span></span>
<span data-ttu-id="f5407-128">在请求正文中，提供 androidCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5407-128">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="f5407-129">下表显示了创建 androidCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5407-129">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="f5407-130">属性</span><span class="sxs-lookup"><span data-stu-id="f5407-130">Property</span></span>|<span data-ttu-id="f5407-131">类型</span><span class="sxs-lookup"><span data-stu-id="f5407-131">Type</span></span>|<span data-ttu-id="f5407-132">说明</span><span class="sxs-lookup"><span data-stu-id="f5407-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5407-133">id</span><span class="sxs-lookup"><span data-stu-id="f5407-133">id</span></span>|<span data-ttu-id="f5407-134">字符串</span><span class="sxs-lookup"><span data-stu-id="f5407-134">String</span></span>|<span data-ttu-id="f5407-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5407-135">Key of the entity.</span></span> <span data-ttu-id="f5407-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5407-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f5407-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5407-138">DateTimeOffset</span></span>|<span data-ttu-id="f5407-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f5407-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f5407-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f5407-141">roleScopeTagIds</span></span>|<span data-ttu-id="f5407-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="f5407-142">String collection</span></span>|<span data-ttu-id="f5407-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f5407-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f5407-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f5407-145">supportsScopeTags</span></span>|<span data-ttu-id="f5407-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5407-146">Boolean</span></span>|<span data-ttu-id="f5407-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f5407-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f5407-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f5407-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f5407-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f5407-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f5407-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f5407-150">This property is read-only.</span></span> <span data-ttu-id="f5407-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5407-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f5407-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5407-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f5407-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f5407-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f5407-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5407-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f5407-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5407-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f5407-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f5407-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f5407-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f5407-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f5407-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f5407-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f5407-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f5407-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f5407-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5407-164">createdDateTime</span></span>|<span data-ttu-id="f5407-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5407-165">DateTimeOffset</span></span>|<span data-ttu-id="f5407-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f5407-166">DateTime the object was created.</span></span> <span data-ttu-id="f5407-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-168">description</span><span class="sxs-lookup"><span data-stu-id="f5407-168">description</span></span>|<span data-ttu-id="f5407-169">String</span><span class="sxs-lookup"><span data-stu-id="f5407-169">String</span></span>|<span data-ttu-id="f5407-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f5407-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f5407-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f5407-172">displayName</span></span>|<span data-ttu-id="f5407-173">String</span><span class="sxs-lookup"><span data-stu-id="f5407-173">String</span></span>|<span data-ttu-id="f5407-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f5407-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f5407-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-176">version</span><span class="sxs-lookup"><span data-stu-id="f5407-176">version</span></span>|<span data-ttu-id="f5407-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f5407-177">Int32</span></span>|<span data-ttu-id="f5407-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f5407-178">Version of the device configuration.</span></span> <span data-ttu-id="f5407-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5407-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5407-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="f5407-180">omaSettings</span></span>|<span data-ttu-id="f5407-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5407-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="f5407-182">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="f5407-182">OMA settings.</span></span> <span data-ttu-id="f5407-183">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="f5407-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f5407-184">响应</span><span class="sxs-lookup"><span data-stu-id="f5407-184">Response</span></span>
<span data-ttu-id="f5407-185">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5407-185">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5407-186">示例</span><span class="sxs-lookup"><span data-stu-id="f5407-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5407-187">请求</span><span class="sxs-lookup"><span data-stu-id="f5407-187">Request</span></span>
<span data-ttu-id="f5407-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5407-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1294

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="f5407-189">响应</span><span class="sxs-lookup"><span data-stu-id="f5407-189">Response</span></span>
<span data-ttu-id="f5407-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5407-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1466

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



