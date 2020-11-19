---
title: 创建 iosExpeditedCheckinConfiguration
description: 创建新的 iosExpeditedCheckinConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff4bb3feddc490e3d682a2ff8f89f9eec907a010
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49264777"
---
# <a name="create-iosexpeditedcheckinconfiguration"></a><span data-ttu-id="5ff03-103">创建 iosExpeditedCheckinConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ff03-103">Create iosExpeditedCheckinConfiguration</span></span>

<span data-ttu-id="5ff03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ff03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ff03-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ff03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ff03-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ff03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ff03-107">创建新的 [iosExpeditedCheckinConfiguration](../resources/intune-deviceconfig-iosexpeditedcheckinconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ff03-107">Create a new [iosExpeditedCheckinConfiguration](../resources/intune-deviceconfig-iosexpeditedcheckinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ff03-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5ff03-108">Prerequisites</span></span>
<span data-ttu-id="5ff03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ff03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ff03-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ff03-111">Permission type</span></span>|<span data-ttu-id="5ff03-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5ff03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ff03-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ff03-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ff03-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff03-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ff03-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ff03-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ff03-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ff03-116">Not supported.</span></span>|
|<span data-ttu-id="5ff03-117">Application</span><span class="sxs-lookup"><span data-stu-id="5ff03-117">Application</span></span>|<span data-ttu-id="5ff03-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff03-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ff03-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ff03-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5ff03-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ff03-120">Request headers</span></span>
|<span data-ttu-id="5ff03-121">标头</span><span class="sxs-lookup"><span data-stu-id="5ff03-121">Header</span></span>|<span data-ttu-id="5ff03-122">值</span><span class="sxs-lookup"><span data-stu-id="5ff03-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ff03-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ff03-123">Authorization</span></span>|<span data-ttu-id="5ff03-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5ff03-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ff03-125">接受</span><span class="sxs-lookup"><span data-stu-id="5ff03-125">Accept</span></span>|<span data-ttu-id="5ff03-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ff03-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ff03-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ff03-127">Request body</span></span>
<span data-ttu-id="5ff03-128">在请求正文中，提供 iosExpeditedCheckinConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ff03-128">In the request body, supply a JSON representation for the iosExpeditedCheckinConfiguration object.</span></span>

<span data-ttu-id="5ff03-129">下表显示创建 iosExpeditedCheckinConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5ff03-129">The following table shows the properties that are required when you create the iosExpeditedCheckinConfiguration.</span></span>

|<span data-ttu-id="5ff03-130">属性</span><span class="sxs-lookup"><span data-stu-id="5ff03-130">Property</span></span>|<span data-ttu-id="5ff03-131">类型</span><span class="sxs-lookup"><span data-stu-id="5ff03-131">Type</span></span>|<span data-ttu-id="5ff03-132">说明</span><span class="sxs-lookup"><span data-stu-id="5ff03-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ff03-133">id</span><span class="sxs-lookup"><span data-stu-id="5ff03-133">id</span></span>|<span data-ttu-id="5ff03-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5ff03-134">String</span></span>|<span data-ttu-id="5ff03-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5ff03-135">Key of the entity.</span></span> <span data-ttu-id="5ff03-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ff03-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5ff03-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ff03-138">DateTimeOffset</span></span>|<span data-ttu-id="5ff03-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5ff03-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5ff03-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ff03-141">roleScopeTagIds</span></span>|<span data-ttu-id="5ff03-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="5ff03-142">String collection</span></span>|<span data-ttu-id="5ff03-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="5ff03-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ff03-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5ff03-145">supportsScopeTags</span></span>|<span data-ttu-id="5ff03-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ff03-146">Boolean</span></span>|<span data-ttu-id="5ff03-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="5ff03-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5ff03-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="5ff03-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5ff03-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="5ff03-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5ff03-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5ff03-150">This property is read-only.</span></span> <span data-ttu-id="5ff03-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5ff03-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5ff03-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5ff03-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5ff03-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="5ff03-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5ff03-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5ff03-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5ff03-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5ff03-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5ff03-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5ff03-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5ff03-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5ff03-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5ff03-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5ff03-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5ff03-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="5ff03-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5ff03-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ff03-164">createdDateTime</span></span>|<span data-ttu-id="5ff03-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ff03-165">DateTimeOffset</span></span>|<span data-ttu-id="5ff03-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5ff03-166">DateTime the object was created.</span></span> <span data-ttu-id="5ff03-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-168">description</span><span class="sxs-lookup"><span data-stu-id="5ff03-168">description</span></span>|<span data-ttu-id="5ff03-169">字符串</span><span class="sxs-lookup"><span data-stu-id="5ff03-169">String</span></span>|<span data-ttu-id="5ff03-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5ff03-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ff03-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-172">displayName</span><span class="sxs-lookup"><span data-stu-id="5ff03-172">displayName</span></span>|<span data-ttu-id="5ff03-173">字符串</span><span class="sxs-lookup"><span data-stu-id="5ff03-173">String</span></span>|<span data-ttu-id="5ff03-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5ff03-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ff03-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-176">version</span><span class="sxs-lookup"><span data-stu-id="5ff03-176">version</span></span>|<span data-ttu-id="5ff03-177">Int32</span><span class="sxs-lookup"><span data-stu-id="5ff03-177">Int32</span></span>|<span data-ttu-id="5ff03-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5ff03-178">Version of the device configuration.</span></span> <span data-ttu-id="5ff03-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ff03-180">enableExpeditedCheckin</span><span class="sxs-lookup"><span data-stu-id="5ff03-180">enableExpeditedCheckin</span></span>|<span data-ttu-id="5ff03-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ff03-181">Boolean</span></span>|<span data-ttu-id="5ff03-182">获取或设置是否启用加速设备签入。继承自 [appleExpeditedCheckinConfigurationBase](../resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="5ff03-182">Gets or sets whether to enable expedited device check-ins. Inherited from [appleExpeditedCheckinConfigurationBase](../resources/intune-deviceconfig-appleexpeditedcheckinconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5ff03-183">响应</span><span class="sxs-lookup"><span data-stu-id="5ff03-183">Response</span></span>
<span data-ttu-id="5ff03-184">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosExpeditedCheckinConfiguration](../resources/intune-deviceconfig-iosexpeditedcheckinconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ff03-184">If successful, this method returns a `201 Created` response code and a [iosExpeditedCheckinConfiguration](../resources/intune-deviceconfig-iosexpeditedcheckinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ff03-185">示例</span><span class="sxs-lookup"><span data-stu-id="5ff03-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ff03-186">请求</span><span class="sxs-lookup"><span data-stu-id="5ff03-186">Request</span></span>
<span data-ttu-id="5ff03-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ff03-187">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1070

{
  "@odata.type": "#microsoft.graph.iosExpeditedCheckinConfiguration",
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
  "enableExpeditedCheckin": true
}
```

### <a name="response"></a><span data-ttu-id="5ff03-188">响应</span><span class="sxs-lookup"><span data-stu-id="5ff03-188">Response</span></span>
<span data-ttu-id="5ff03-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ff03-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1242

{
  "@odata.type": "#microsoft.graph.iosExpeditedCheckinConfiguration",
  "id": "f833f985-f985-f833-85f9-33f885f933f8",
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
  "enableExpeditedCheckin": true
}
```




