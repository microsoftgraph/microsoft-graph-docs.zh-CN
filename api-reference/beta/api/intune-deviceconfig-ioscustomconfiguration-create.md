---
title: 创建 iosCustomConfiguration
description: 创建新的 iosCustomConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42f6151a67e7a7cea3bca91d1acfff09b4497d18
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37167940"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="6e274-103">创建 iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e274-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="6e274-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e274-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e274-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e274-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e274-106">创建新的 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e274-106">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e274-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e274-107">Prerequisites</span></span>
<span data-ttu-id="6e274-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e274-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e274-110">Permission type</span></span>|<span data-ttu-id="6e274-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e274-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e274-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e274-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6e274-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e274-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e274-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e274-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e274-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e274-115">Not supported.</span></span>|
|<span data-ttu-id="6e274-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e274-116">Application</span></span>|<span data-ttu-id="6e274-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e274-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e274-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e274-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6e274-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e274-119">Request headers</span></span>
|<span data-ttu-id="6e274-120">标头</span><span class="sxs-lookup"><span data-stu-id="6e274-120">Header</span></span>|<span data-ttu-id="6e274-121">值</span><span class="sxs-lookup"><span data-stu-id="6e274-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e274-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e274-122">Authorization</span></span>|<span data-ttu-id="6e274-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e274-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e274-124">接受</span><span class="sxs-lookup"><span data-stu-id="6e274-124">Accept</span></span>|<span data-ttu-id="6e274-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6e274-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e274-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e274-126">Request body</span></span>
<span data-ttu-id="6e274-127">在请求正文中，提供 iosCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e274-127">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="6e274-128">下表显示创建 iosCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6e274-128">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="6e274-129">属性</span><span class="sxs-lookup"><span data-stu-id="6e274-129">Property</span></span>|<span data-ttu-id="6e274-130">类型</span><span class="sxs-lookup"><span data-stu-id="6e274-130">Type</span></span>|<span data-ttu-id="6e274-131">说明</span><span class="sxs-lookup"><span data-stu-id="6e274-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e274-132">id</span><span class="sxs-lookup"><span data-stu-id="6e274-132">id</span></span>|<span data-ttu-id="6e274-133">字符串</span><span class="sxs-lookup"><span data-stu-id="6e274-133">String</span></span>|<span data-ttu-id="6e274-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6e274-134">Key of the entity.</span></span> <span data-ttu-id="6e274-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e274-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6e274-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e274-137">DateTimeOffset</span></span>|<span data-ttu-id="6e274-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6e274-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6e274-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e274-140">roleScopeTagIds</span></span>|<span data-ttu-id="6e274-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6e274-141">String collection</span></span>|<span data-ttu-id="6e274-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6e274-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e274-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6e274-144">supportsScopeTags</span></span>|<span data-ttu-id="6e274-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e274-145">Boolean</span></span>|<span data-ttu-id="6e274-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6e274-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6e274-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6e274-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6e274-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6e274-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6e274-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6e274-149">This property is read-only.</span></span> <span data-ttu-id="6e274-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6e274-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6e274-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6e274-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6e274-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="6e274-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6e274-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6e274-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6e274-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6e274-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6e274-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6e274-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6e274-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6e274-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6e274-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6e274-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6e274-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="6e274-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6e274-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e274-163">createdDateTime</span></span>|<span data-ttu-id="6e274-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e274-164">DateTimeOffset</span></span>|<span data-ttu-id="6e274-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6e274-165">DateTime the object was created.</span></span> <span data-ttu-id="6e274-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-167">说明</span><span class="sxs-lookup"><span data-stu-id="6e274-167">description</span></span>|<span data-ttu-id="6e274-168">String</span><span class="sxs-lookup"><span data-stu-id="6e274-168">String</span></span>|<span data-ttu-id="6e274-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6e274-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e274-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6e274-171">displayName</span></span>|<span data-ttu-id="6e274-172">字符串</span><span class="sxs-lookup"><span data-stu-id="6e274-172">String</span></span>|<span data-ttu-id="6e274-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6e274-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e274-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-175">version</span><span class="sxs-lookup"><span data-stu-id="6e274-175">version</span></span>|<span data-ttu-id="6e274-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6e274-176">Int32</span></span>|<span data-ttu-id="6e274-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6e274-177">Version of the device configuration.</span></span> <span data-ttu-id="6e274-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e274-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e274-179">payloadName</span><span class="sxs-lookup"><span data-stu-id="6e274-179">payloadName</span></span>|<span data-ttu-id="6e274-180">String</span><span class="sxs-lookup"><span data-stu-id="6e274-180">String</span></span>|<span data-ttu-id="6e274-181">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="6e274-181">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="6e274-182">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6e274-182">payloadFileName</span></span>|<span data-ttu-id="6e274-183">String</span><span class="sxs-lookup"><span data-stu-id="6e274-183">String</span></span>|<span data-ttu-id="6e274-184">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="6e274-184">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="6e274-185">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="6e274-185">\*.xml).</span></span>|
|<span data-ttu-id="6e274-186">payload</span><span class="sxs-lookup"><span data-stu-id="6e274-186">payload</span></span>|<span data-ttu-id="6e274-187">Binary</span><span class="sxs-lookup"><span data-stu-id="6e274-187">Binary</span></span>|<span data-ttu-id="6e274-188">有效负载。</span><span class="sxs-lookup"><span data-stu-id="6e274-188">Payload.</span></span> <span data-ttu-id="6e274-189">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="6e274-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="6e274-190">响应</span><span class="sxs-lookup"><span data-stu-id="6e274-190">Response</span></span>
<span data-ttu-id="6e274-191">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6e274-191">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e274-192">示例</span><span class="sxs-lookup"><span data-stu-id="6e274-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e274-193">请求</span><span class="sxs-lookup"><span data-stu-id="6e274-193">Request</span></span>
<span data-ttu-id="6e274-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e274-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1144

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="6e274-195">响应</span><span class="sxs-lookup"><span data-stu-id="6e274-195">Response</span></span>
<span data-ttu-id="6e274-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e274-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1316

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```




