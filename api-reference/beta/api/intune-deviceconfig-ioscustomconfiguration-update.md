---
title: 更新 iosCustomConfiguration
description: 更新 iosCustomConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ea8e04d07e833fb382184b6cf9d239b16c9f626b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474860"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="0aa98-103">更新 iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="0aa98-103">Update iosCustomConfiguration</span></span>

<span data-ttu-id="0aa98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aa98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0aa98-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0aa98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0aa98-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0aa98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aa98-107">更新 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0aa98-107">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0aa98-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0aa98-108">Prerequisites</span></span>
<span data-ttu-id="0aa98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0aa98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aa98-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0aa98-111">Permission type</span></span>|<span data-ttu-id="0aa98-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0aa98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0aa98-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0aa98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0aa98-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aa98-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0aa98-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0aa98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0aa98-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0aa98-116">Not supported.</span></span>|
|<span data-ttu-id="0aa98-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0aa98-117">Application</span></span>|<span data-ttu-id="0aa98-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0aa98-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0aa98-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0aa98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0aa98-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0aa98-120">Request headers</span></span>
|<span data-ttu-id="0aa98-121">标头</span><span class="sxs-lookup"><span data-stu-id="0aa98-121">Header</span></span>|<span data-ttu-id="0aa98-122">值</span><span class="sxs-lookup"><span data-stu-id="0aa98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0aa98-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aa98-123">Authorization</span></span>|<span data-ttu-id="0aa98-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0aa98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0aa98-125">接受</span><span class="sxs-lookup"><span data-stu-id="0aa98-125">Accept</span></span>|<span data-ttu-id="0aa98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0aa98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aa98-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0aa98-127">Request body</span></span>
<span data-ttu-id="0aa98-128">在请求正文中，提供 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0aa98-128">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="0aa98-129">下表显示创建 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0aa98-129">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="0aa98-130">属性</span><span class="sxs-lookup"><span data-stu-id="0aa98-130">Property</span></span>|<span data-ttu-id="0aa98-131">类型</span><span class="sxs-lookup"><span data-stu-id="0aa98-131">Type</span></span>|<span data-ttu-id="0aa98-132">说明</span><span class="sxs-lookup"><span data-stu-id="0aa98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aa98-133">id</span><span class="sxs-lookup"><span data-stu-id="0aa98-133">id</span></span>|<span data-ttu-id="0aa98-134">String</span><span class="sxs-lookup"><span data-stu-id="0aa98-134">String</span></span>|<span data-ttu-id="0aa98-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0aa98-135">Key of the entity.</span></span> <span data-ttu-id="0aa98-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0aa98-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0aa98-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aa98-138">DateTimeOffset</span></span>|<span data-ttu-id="0aa98-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0aa98-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0aa98-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0aa98-141">roleScopeTagIds</span></span>|<span data-ttu-id="0aa98-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0aa98-142">String collection</span></span>|<span data-ttu-id="0aa98-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0aa98-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0aa98-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0aa98-145">supportsScopeTags</span></span>|<span data-ttu-id="0aa98-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0aa98-146">Boolean</span></span>|<span data-ttu-id="0aa98-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="0aa98-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0aa98-148">当此值为 false 且实体对范围用户不可见时，不允许向 ScopeTags 属性赋值。</span><span class="sxs-lookup"><span data-stu-id="0aa98-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0aa98-149">这适用于在 Silverlight 中创建的旧策略，可通过在 Azure 门户中删除和重新创建策略来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="0aa98-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0aa98-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0aa98-150">This property is read-only.</span></span> <span data-ttu-id="0aa98-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0aa98-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0aa98-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0aa98-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0aa98-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="0aa98-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0aa98-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0aa98-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0aa98-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0aa98-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0aa98-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0aa98-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0aa98-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0aa98-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0aa98-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0aa98-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0aa98-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="0aa98-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0aa98-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0aa98-164">createdDateTime</span></span>|<span data-ttu-id="0aa98-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0aa98-165">DateTimeOffset</span></span>|<span data-ttu-id="0aa98-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0aa98-166">DateTime the object was created.</span></span> <span data-ttu-id="0aa98-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-168">说明</span><span class="sxs-lookup"><span data-stu-id="0aa98-168">description</span></span>|<span data-ttu-id="0aa98-169">String</span><span class="sxs-lookup"><span data-stu-id="0aa98-169">String</span></span>|<span data-ttu-id="0aa98-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0aa98-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0aa98-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0aa98-172">displayName</span></span>|<span data-ttu-id="0aa98-173">String</span><span class="sxs-lookup"><span data-stu-id="0aa98-173">String</span></span>|<span data-ttu-id="0aa98-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0aa98-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0aa98-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-176">version</span><span class="sxs-lookup"><span data-stu-id="0aa98-176">version</span></span>|<span data-ttu-id="0aa98-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0aa98-177">Int32</span></span>|<span data-ttu-id="0aa98-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0aa98-178">Version of the device configuration.</span></span> <span data-ttu-id="0aa98-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0aa98-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0aa98-180">payloadName</span><span class="sxs-lookup"><span data-stu-id="0aa98-180">payloadName</span></span>|<span data-ttu-id="0aa98-181">String</span><span class="sxs-lookup"><span data-stu-id="0aa98-181">String</span></span>|<span data-ttu-id="0aa98-182">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="0aa98-182">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="0aa98-183">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="0aa98-183">payloadFileName</span></span>|<span data-ttu-id="0aa98-184">String</span><span class="sxs-lookup"><span data-stu-id="0aa98-184">String</span></span>|<span data-ttu-id="0aa98-185">有效负载文件名 (\*.mobileconfig \| \*.xml) 。</span><span class="sxs-lookup"><span data-stu-id="0aa98-185">Payload file name (\*.mobileconfig \| \*.xml).</span></span>|
|<span data-ttu-id="0aa98-186">payload</span><span class="sxs-lookup"><span data-stu-id="0aa98-186">payload</span></span>|<span data-ttu-id="0aa98-187">Binary</span><span class="sxs-lookup"><span data-stu-id="0aa98-187">Binary</span></span>|<span data-ttu-id="0aa98-188">有效负载。</span><span class="sxs-lookup"><span data-stu-id="0aa98-188">Payload.</span></span> <span data-ttu-id="0aa98-189">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="0aa98-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="0aa98-190">响应</span><span class="sxs-lookup"><span data-stu-id="0aa98-190">Response</span></span>
<span data-ttu-id="0aa98-191">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0aa98-191">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aa98-192">示例</span><span class="sxs-lookup"><span data-stu-id="0aa98-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="0aa98-193">请求</span><span class="sxs-lookup"><span data-stu-id="0aa98-193">Request</span></span>
<span data-ttu-id="0aa98-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0aa98-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="0aa98-195">响应</span><span class="sxs-lookup"><span data-stu-id="0aa98-195">Response</span></span>
<span data-ttu-id="0aa98-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0aa98-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




