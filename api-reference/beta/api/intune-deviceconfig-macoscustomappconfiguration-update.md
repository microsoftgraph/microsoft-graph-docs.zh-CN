---
title: 更新 macOSCustomAppConfiguration
description: 更新 macOSCustomAppConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3290a4761de3bf47e16f99f3605c67bee5e57114
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994797"
---
# <a name="update-macoscustomappconfiguration"></a><span data-ttu-id="858b8-103">更新 macOSCustomAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="858b8-103">Update macOSCustomAppConfiguration</span></span>

<span data-ttu-id="858b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="858b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="858b8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="858b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="858b8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="858b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="858b8-107">更新 [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="858b8-107">Update the properties of a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="858b8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="858b8-108">Prerequisites</span></span>
<span data-ttu-id="858b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="858b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="858b8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="858b8-111">Permission type</span></span>|<span data-ttu-id="858b8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="858b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="858b8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="858b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="858b8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="858b8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="858b8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="858b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="858b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="858b8-116">Not supported.</span></span>|
|<span data-ttu-id="858b8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="858b8-117">Application</span></span>|<span data-ttu-id="858b8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="858b8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="858b8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="858b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="858b8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="858b8-120">Request headers</span></span>
|<span data-ttu-id="858b8-121">标头</span><span class="sxs-lookup"><span data-stu-id="858b8-121">Header</span></span>|<span data-ttu-id="858b8-122">值</span><span class="sxs-lookup"><span data-stu-id="858b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="858b8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="858b8-123">Authorization</span></span>|<span data-ttu-id="858b8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="858b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="858b8-125">接受</span><span class="sxs-lookup"><span data-stu-id="858b8-125">Accept</span></span>|<span data-ttu-id="858b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="858b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="858b8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="858b8-127">Request body</span></span>
<span data-ttu-id="858b8-128">在请求正文中，提供 [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="858b8-128">In the request body, supply a JSON representation for the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

<span data-ttu-id="858b8-129">下表显示创建 [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="858b8-129">The following table shows the properties that are required when you create the [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md).</span></span>

|<span data-ttu-id="858b8-130">属性</span><span class="sxs-lookup"><span data-stu-id="858b8-130">Property</span></span>|<span data-ttu-id="858b8-131">类型</span><span class="sxs-lookup"><span data-stu-id="858b8-131">Type</span></span>|<span data-ttu-id="858b8-132">说明</span><span class="sxs-lookup"><span data-stu-id="858b8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="858b8-133">id</span><span class="sxs-lookup"><span data-stu-id="858b8-133">id</span></span>|<span data-ttu-id="858b8-134">String</span><span class="sxs-lookup"><span data-stu-id="858b8-134">String</span></span>|<span data-ttu-id="858b8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="858b8-135">Key of the entity.</span></span> <span data-ttu-id="858b8-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="858b8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="858b8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="858b8-138">DateTimeOffset</span></span>|<span data-ttu-id="858b8-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="858b8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="858b8-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="858b8-141">roleScopeTagIds</span></span>|<span data-ttu-id="858b8-142">String collection</span><span class="sxs-lookup"><span data-stu-id="858b8-142">String collection</span></span>|<span data-ttu-id="858b8-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="858b8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="858b8-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="858b8-145">supportsScopeTags</span></span>|<span data-ttu-id="858b8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="858b8-146">Boolean</span></span>|<span data-ttu-id="858b8-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="858b8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="858b8-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="858b8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="858b8-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="858b8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="858b8-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="858b8-150">This property is read-only.</span></span> <span data-ttu-id="858b8-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="858b8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="858b8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="858b8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="858b8-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="858b8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="858b8-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="858b8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="858b8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="858b8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="858b8-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="858b8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="858b8-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="858b8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="858b8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="858b8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="858b8-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="858b8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="858b8-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="858b8-164">createdDateTime</span></span>|<span data-ttu-id="858b8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="858b8-165">DateTimeOffset</span></span>|<span data-ttu-id="858b8-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="858b8-166">DateTime the object was created.</span></span> <span data-ttu-id="858b8-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-168">description</span><span class="sxs-lookup"><span data-stu-id="858b8-168">description</span></span>|<span data-ttu-id="858b8-169">String</span><span class="sxs-lookup"><span data-stu-id="858b8-169">String</span></span>|<span data-ttu-id="858b8-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="858b8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="858b8-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="858b8-172">displayName</span></span>|<span data-ttu-id="858b8-173">String</span><span class="sxs-lookup"><span data-stu-id="858b8-173">String</span></span>|<span data-ttu-id="858b8-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="858b8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="858b8-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-176">version</span><span class="sxs-lookup"><span data-stu-id="858b8-176">version</span></span>|<span data-ttu-id="858b8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="858b8-177">Int32</span></span>|<span data-ttu-id="858b8-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="858b8-178">Version of the device configuration.</span></span> <span data-ttu-id="858b8-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="858b8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="858b8-180">bundleId</span><span class="sxs-lookup"><span data-stu-id="858b8-180">bundleId</span></span>|<span data-ttu-id="858b8-181">String</span><span class="sxs-lookup"><span data-stu-id="858b8-181">String</span></span>|<span data-ttu-id="858b8-182">目标的捆绑包 id。</span><span class="sxs-lookup"><span data-stu-id="858b8-182">Bundle id for targeting.</span></span>|
|<span data-ttu-id="858b8-183">fileName</span><span class="sxs-lookup"><span data-stu-id="858b8-183">fileName</span></span>|<span data-ttu-id="858b8-184">String</span><span class="sxs-lookup"><span data-stu-id="858b8-184">String</span></span>|<span data-ttu-id="858b8-185">配置文件名 ( \* plist</span><span class="sxs-lookup"><span data-stu-id="858b8-185">Configuration file name (\*.plist</span></span> | <span data-ttu-id="858b8-186">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="858b8-186">\*.xml).</span></span>|
|<span data-ttu-id="858b8-187">configurationXml</span><span class="sxs-lookup"><span data-stu-id="858b8-187">configurationXml</span></span>|<span data-ttu-id="858b8-188">Binary</span><span class="sxs-lookup"><span data-stu-id="858b8-188">Binary</span></span>|<span data-ttu-id="858b8-189">配置 xml。</span><span class="sxs-lookup"><span data-stu-id="858b8-189">Configuration xml.</span></span> <span data-ttu-id="858b8-190">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="858b8-190">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="858b8-191">响应</span><span class="sxs-lookup"><span data-stu-id="858b8-191">Response</span></span>
<span data-ttu-id="858b8-192">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="858b8-192">If successful, this method returns a `200 OK` response code and an updated [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="858b8-193">示例</span><span class="sxs-lookup"><span data-stu-id="858b8-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="858b8-194">请求</span><span class="sxs-lookup"><span data-stu-id="858b8-194">Request</span></span>
<span data-ttu-id="858b8-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="858b8-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="858b8-196">响应</span><span class="sxs-lookup"><span data-stu-id="858b8-196">Response</span></span>
<span data-ttu-id="858b8-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="858b8-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






