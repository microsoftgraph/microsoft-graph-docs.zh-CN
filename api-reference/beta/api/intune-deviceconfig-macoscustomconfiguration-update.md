---
title: 更新 macOSCustomConfiguration
description: 更新 macOSCustomConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 73fdf64d35e7ca565124d5075d5feb6290317865
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974637"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="12522-103">更新 macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="12522-103">Update macOSCustomConfiguration</span></span>

<span data-ttu-id="12522-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12522-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12522-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12522-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12522-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12522-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12522-107">更新 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12522-107">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12522-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="12522-108">Prerequisites</span></span>
<span data-ttu-id="12522-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12522-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12522-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12522-111">Permission type</span></span>|<span data-ttu-id="12522-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12522-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12522-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12522-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12522-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12522-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12522-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12522-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12522-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12522-116">Not supported.</span></span>|
|<span data-ttu-id="12522-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12522-117">Application</span></span>|<span data-ttu-id="12522-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12522-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12522-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12522-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="12522-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="12522-120">Request headers</span></span>
|<span data-ttu-id="12522-121">标头</span><span class="sxs-lookup"><span data-stu-id="12522-121">Header</span></span>|<span data-ttu-id="12522-122">值</span><span class="sxs-lookup"><span data-stu-id="12522-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12522-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12522-123">Authorization</span></span>|<span data-ttu-id="12522-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12522-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12522-125">接受</span><span class="sxs-lookup"><span data-stu-id="12522-125">Accept</span></span>|<span data-ttu-id="12522-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12522-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12522-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="12522-127">Request body</span></span>
<span data-ttu-id="12522-128">在请求正文中，提供 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12522-128">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="12522-129">下表显示了创建 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12522-129">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="12522-130">属性</span><span class="sxs-lookup"><span data-stu-id="12522-130">Property</span></span>|<span data-ttu-id="12522-131">类型</span><span class="sxs-lookup"><span data-stu-id="12522-131">Type</span></span>|<span data-ttu-id="12522-132">说明</span><span class="sxs-lookup"><span data-stu-id="12522-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12522-133">id</span><span class="sxs-lookup"><span data-stu-id="12522-133">id</span></span>|<span data-ttu-id="12522-134">String</span><span class="sxs-lookup"><span data-stu-id="12522-134">String</span></span>|<span data-ttu-id="12522-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12522-135">Key of the entity.</span></span> <span data-ttu-id="12522-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12522-137">lastModifiedDateTime</span></span>|<span data-ttu-id="12522-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12522-138">DateTimeOffset</span></span>|<span data-ttu-id="12522-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="12522-139">DateTime the object was last modified.</span></span> <span data-ttu-id="12522-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12522-141">roleScopeTagIds</span></span>|<span data-ttu-id="12522-142">String collection</span><span class="sxs-lookup"><span data-stu-id="12522-142">String collection</span></span>|<span data-ttu-id="12522-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="12522-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="12522-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="12522-145">supportsScopeTags</span></span>|<span data-ttu-id="12522-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="12522-146">Boolean</span></span>|<span data-ttu-id="12522-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="12522-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="12522-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="12522-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="12522-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="12522-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="12522-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="12522-150">This property is read-only.</span></span> <span data-ttu-id="12522-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12522-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="12522-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="12522-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="12522-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="12522-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="12522-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12522-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="12522-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="12522-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="12522-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="12522-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="12522-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12522-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="12522-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="12522-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="12522-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="12522-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="12522-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12522-164">createdDateTime</span></span>|<span data-ttu-id="12522-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12522-165">DateTimeOffset</span></span>|<span data-ttu-id="12522-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="12522-166">DateTime the object was created.</span></span> <span data-ttu-id="12522-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-168">description</span><span class="sxs-lookup"><span data-stu-id="12522-168">description</span></span>|<span data-ttu-id="12522-169">String</span><span class="sxs-lookup"><span data-stu-id="12522-169">String</span></span>|<span data-ttu-id="12522-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="12522-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="12522-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-172">displayName</span><span class="sxs-lookup"><span data-stu-id="12522-172">displayName</span></span>|<span data-ttu-id="12522-173">String</span><span class="sxs-lookup"><span data-stu-id="12522-173">String</span></span>|<span data-ttu-id="12522-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="12522-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="12522-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-176">version</span><span class="sxs-lookup"><span data-stu-id="12522-176">version</span></span>|<span data-ttu-id="12522-177">Int32</span><span class="sxs-lookup"><span data-stu-id="12522-177">Int32</span></span>|<span data-ttu-id="12522-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="12522-178">Version of the device configuration.</span></span> <span data-ttu-id="12522-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12522-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="12522-180">payloadName</span><span class="sxs-lookup"><span data-stu-id="12522-180">payloadName</span></span>|<span data-ttu-id="12522-181">String</span><span class="sxs-lookup"><span data-stu-id="12522-181">String</span></span>|<span data-ttu-id="12522-182">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="12522-182">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="12522-183">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="12522-183">payloadFileName</span></span>|<span data-ttu-id="12522-184">String</span><span class="sxs-lookup"><span data-stu-id="12522-184">String</span></span>|<span data-ttu-id="12522-185">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="12522-185">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="12522-186">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="12522-186">\*.xml).</span></span>|
|<span data-ttu-id="12522-187">payload</span><span class="sxs-lookup"><span data-stu-id="12522-187">payload</span></span>|<span data-ttu-id="12522-188">Binary</span><span class="sxs-lookup"><span data-stu-id="12522-188">Binary</span></span>|<span data-ttu-id="12522-189">有效负载。</span><span class="sxs-lookup"><span data-stu-id="12522-189">Payload.</span></span> <span data-ttu-id="12522-190">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="12522-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="12522-191">响应</span><span class="sxs-lookup"><span data-stu-id="12522-191">Response</span></span>
<span data-ttu-id="12522-192">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="12522-192">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12522-193">示例</span><span class="sxs-lookup"><span data-stu-id="12522-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="12522-194">请求</span><span class="sxs-lookup"><span data-stu-id="12522-194">Request</span></span>
<span data-ttu-id="12522-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12522-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1146

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="12522-196">响应</span><span class="sxs-lookup"><span data-stu-id="12522-196">Response</span></span>
<span data-ttu-id="12522-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12522-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1318

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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






