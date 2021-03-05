---
title: 更新 macOSCustomAppConfiguration
description: 更新 macOSCustomAppConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7579806180874a9dd8dfda38bf4ba70663c41b8e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473580"
---
# <a name="update-macoscustomappconfiguration"></a><span data-ttu-id="fe08e-103">更新 macOSCustomAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe08e-103">Update macOSCustomAppConfiguration</span></span>

<span data-ttu-id="fe08e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe08e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe08e-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe08e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe08e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe08e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe08e-107">更新 [macOSCustomAppConfiguration 对象](../resources/intune-deviceconfig-macoscustomappconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="fe08e-107">Update the properties of a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe08e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe08e-108">Prerequisites</span></span>
<span data-ttu-id="fe08e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe08e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe08e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe08e-111">Permission type</span></span>|<span data-ttu-id="fe08e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fe08e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe08e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe08e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe08e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe08e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe08e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe08e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe08e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe08e-116">Not supported.</span></span>|
|<span data-ttu-id="fe08e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe08e-117">Application</span></span>|<span data-ttu-id="fe08e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe08e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe08e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe08e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fe08e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe08e-120">Request headers</span></span>
|<span data-ttu-id="fe08e-121">标头</span><span class="sxs-lookup"><span data-stu-id="fe08e-121">Header</span></span>|<span data-ttu-id="fe08e-122">值</span><span class="sxs-lookup"><span data-stu-id="fe08e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe08e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe08e-123">Authorization</span></span>|<span data-ttu-id="fe08e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe08e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe08e-125">接受</span><span class="sxs-lookup"><span data-stu-id="fe08e-125">Accept</span></span>|<span data-ttu-id="fe08e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe08e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe08e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe08e-127">Request body</span></span>
<span data-ttu-id="fe08e-128">在请求正文中，提供 [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe08e-128">In the request body, supply a JSON representation for the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

<span data-ttu-id="fe08e-129">下表显示创建 [macOSCustomAppConfiguration 时所需的属性](../resources/intune-deviceconfig-macoscustomappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="fe08e-129">The following table shows the properties that are required when you create the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span></span>

|<span data-ttu-id="fe08e-130">属性</span><span class="sxs-lookup"><span data-stu-id="fe08e-130">Property</span></span>|<span data-ttu-id="fe08e-131">类型</span><span class="sxs-lookup"><span data-stu-id="fe08e-131">Type</span></span>|<span data-ttu-id="fe08e-132">说明</span><span class="sxs-lookup"><span data-stu-id="fe08e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe08e-133">id</span><span class="sxs-lookup"><span data-stu-id="fe08e-133">id</span></span>|<span data-ttu-id="fe08e-134">String</span><span class="sxs-lookup"><span data-stu-id="fe08e-134">String</span></span>|<span data-ttu-id="fe08e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fe08e-135">Key of the entity.</span></span> <span data-ttu-id="fe08e-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe08e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fe08e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe08e-138">DateTimeOffset</span></span>|<span data-ttu-id="fe08e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fe08e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fe08e-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe08e-141">roleScopeTagIds</span></span>|<span data-ttu-id="fe08e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="fe08e-142">String collection</span></span>|<span data-ttu-id="fe08e-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="fe08e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fe08e-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fe08e-145">supportsScopeTags</span></span>|<span data-ttu-id="fe08e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe08e-146">Boolean</span></span>|<span data-ttu-id="fe08e-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="fe08e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fe08e-148">当此值为 false 且实体对范围用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="fe08e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fe08e-149">对于在 Silverlight 中创建的旧策略，会发生此情况，可通过在 Azure 门户中删除和重新创建策略来解决此问题。</span><span class="sxs-lookup"><span data-stu-id="fe08e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fe08e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="fe08e-150">This property is read-only.</span></span> <span data-ttu-id="fe08e-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fe08e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fe08e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fe08e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fe08e-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="fe08e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fe08e-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fe08e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fe08e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fe08e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fe08e-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fe08e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fe08e-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fe08e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fe08e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fe08e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fe08e-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="fe08e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fe08e-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe08e-164">createdDateTime</span></span>|<span data-ttu-id="fe08e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe08e-165">DateTimeOffset</span></span>|<span data-ttu-id="fe08e-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="fe08e-166">DateTime the object was created.</span></span> <span data-ttu-id="fe08e-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-168">说明</span><span class="sxs-lookup"><span data-stu-id="fe08e-168">description</span></span>|<span data-ttu-id="fe08e-169">String</span><span class="sxs-lookup"><span data-stu-id="fe08e-169">String</span></span>|<span data-ttu-id="fe08e-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="fe08e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe08e-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fe08e-172">displayName</span></span>|<span data-ttu-id="fe08e-173">String</span><span class="sxs-lookup"><span data-stu-id="fe08e-173">String</span></span>|<span data-ttu-id="fe08e-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="fe08e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe08e-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-176">version</span><span class="sxs-lookup"><span data-stu-id="fe08e-176">version</span></span>|<span data-ttu-id="fe08e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fe08e-177">Int32</span></span>|<span data-ttu-id="fe08e-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="fe08e-178">Version of the device configuration.</span></span> <span data-ttu-id="fe08e-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe08e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe08e-180">bundleId</span><span class="sxs-lookup"><span data-stu-id="fe08e-180">bundleId</span></span>|<span data-ttu-id="fe08e-181">String</span><span class="sxs-lookup"><span data-stu-id="fe08e-181">String</span></span>|<span data-ttu-id="fe08e-182">用于定位的捆绑包 ID。</span><span class="sxs-lookup"><span data-stu-id="fe08e-182">Bundle id for targeting.</span></span>|
|<span data-ttu-id="fe08e-183">fileName</span><span class="sxs-lookup"><span data-stu-id="fe08e-183">fileName</span></span>|<span data-ttu-id="fe08e-184">String</span><span class="sxs-lookup"><span data-stu-id="fe08e-184">String</span></span>|<span data-ttu-id="fe08e-185">配置文件名称 (\*.plist \| \*.xml) 。</span><span class="sxs-lookup"><span data-stu-id="fe08e-185">Configuration file name (\*.plist \| \*.xml).</span></span>|
|<span data-ttu-id="fe08e-186">configurationXml</span><span class="sxs-lookup"><span data-stu-id="fe08e-186">configurationXml</span></span>|<span data-ttu-id="fe08e-187">Binary</span><span class="sxs-lookup"><span data-stu-id="fe08e-187">Binary</span></span>|<span data-ttu-id="fe08e-188">Configuration xml。</span><span class="sxs-lookup"><span data-stu-id="fe08e-188">Configuration xml.</span></span> <span data-ttu-id="fe08e-189">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="fe08e-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="fe08e-190">响应</span><span class="sxs-lookup"><span data-stu-id="fe08e-190">Response</span></span>
<span data-ttu-id="fe08e-191">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe08e-191">If successful, this method returns a `200 OK` response code and an updated [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe08e-192">示例</span><span class="sxs-lookup"><span data-stu-id="fe08e-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe08e-193">请求</span><span class="sxs-lookup"><span data-stu-id="fe08e-193">Request</span></span>
<span data-ttu-id="fe08e-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe08e-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1149

{
  "@odata.type": "#microsoft.graph.macOSCustomAppConfiguration",
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
  "bundleId": "Bundle Id value",
  "fileName": "File Name value",
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="fe08e-195">响应</span><span class="sxs-lookup"><span data-stu-id="fe08e-195">Response</span></span>
<span data-ttu-id="fe08e-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe08e-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1321

{
  "@odata.type": "#microsoft.graph.macOSCustomAppConfiguration",
  "id": "1b8a4e02-4e02-1b8a-024e-8a1b024e8a1b",
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
  "bundleId": "Bundle Id value",
  "fileName": "File Name value",
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```




