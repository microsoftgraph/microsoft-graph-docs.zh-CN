---
title: 创建 macOSCustomAppConfiguration
description: 创建新的 macOSCustomAppConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fd6568aa8d2b0869c9b901b89f617231277d875
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948492"
---
# <a name="create-macoscustomappconfiguration"></a><span data-ttu-id="ce7b1-103">创建 macOSCustomAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce7b1-103">Create macOSCustomAppConfiguration</span></span>

> <span data-ttu-id="ce7b1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce7b1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce7b1-106">创建新的[macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-106">Create a new [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce7b1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce7b1-107">Prerequisites</span></span>
<span data-ttu-id="ce7b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce7b1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce7b1-110">Permission type</span></span>|<span data-ttu-id="ce7b1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ce7b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce7b1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce7b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce7b1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce7b1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce7b1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce7b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce7b1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-115">Not supported.</span></span>|
|<span data-ttu-id="ce7b1-116">Application</span><span class="sxs-lookup"><span data-stu-id="ce7b1-116">Application</span></span>|<span data-ttu-id="ce7b1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce7b1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce7b1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce7b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ce7b1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce7b1-119">Request headers</span></span>
|<span data-ttu-id="ce7b1-120">标头</span><span class="sxs-lookup"><span data-stu-id="ce7b1-120">Header</span></span>|<span data-ttu-id="ce7b1-121">值</span><span class="sxs-lookup"><span data-stu-id="ce7b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce7b1-122">授权</span><span class="sxs-lookup"><span data-stu-id="ce7b1-122">Authorization</span></span>|<span data-ttu-id="ce7b1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce7b1-124">接受</span><span class="sxs-lookup"><span data-stu-id="ce7b1-124">Accept</span></span>|<span data-ttu-id="ce7b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce7b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce7b1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce7b1-126">Request body</span></span>
<span data-ttu-id="ce7b1-127">在请求正文中，提供 macOSCustomAppConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-127">In the request body, supply a JSON representation for the macOSCustomAppConfiguration object.</span></span>

<span data-ttu-id="ce7b1-128">下表显示创建 macOSCustomAppConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-128">The following table shows the properties that are required when you create the macOSCustomAppConfiguration.</span></span>

|<span data-ttu-id="ce7b1-129">属性</span><span class="sxs-lookup"><span data-stu-id="ce7b1-129">Property</span></span>|<span data-ttu-id="ce7b1-130">类型</span><span class="sxs-lookup"><span data-stu-id="ce7b1-130">Type</span></span>|<span data-ttu-id="ce7b1-131">说明</span><span class="sxs-lookup"><span data-stu-id="ce7b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce7b1-132">id</span><span class="sxs-lookup"><span data-stu-id="ce7b1-132">id</span></span>|<span data-ttu-id="ce7b1-133">字符串</span><span class="sxs-lookup"><span data-stu-id="ce7b1-133">String</span></span>|<span data-ttu-id="ce7b1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-134">Key of the entity.</span></span> <span data-ttu-id="ce7b1-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce7b1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ce7b1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce7b1-137">DateTimeOffset</span></span>|<span data-ttu-id="ce7b1-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ce7b1-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce7b1-140">roleScopeTagIds</span></span>|<span data-ttu-id="ce7b1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="ce7b1-141">String collection</span></span>|<span data-ttu-id="ce7b1-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce7b1-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ce7b1-144">supportsScopeTags</span></span>|<span data-ttu-id="ce7b1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce7b1-145">Boolean</span></span>|<span data-ttu-id="ce7b1-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce7b1-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce7b1-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce7b1-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-149">This property is read-only.</span></span> <span data-ttu-id="ce7b1-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce7b1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ce7b1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ce7b1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ce7b1-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ce7b1-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce7b1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ce7b1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce7b1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ce7b1-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ce7b1-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce7b1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ce7b1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ce7b1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ce7b1-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ce7b1-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce7b1-163">createdDateTime</span></span>|<span data-ttu-id="ce7b1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce7b1-164">DateTimeOffset</span></span>|<span data-ttu-id="ce7b1-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-165">DateTime the object was created.</span></span> <span data-ttu-id="ce7b1-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-167">说明</span><span class="sxs-lookup"><span data-stu-id="ce7b1-167">description</span></span>|<span data-ttu-id="ce7b1-168">String</span><span class="sxs-lookup"><span data-stu-id="ce7b1-168">String</span></span>|<span data-ttu-id="ce7b1-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce7b1-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ce7b1-171">displayName</span></span>|<span data-ttu-id="ce7b1-172">String</span><span class="sxs-lookup"><span data-stu-id="ce7b1-172">String</span></span>|<span data-ttu-id="ce7b1-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce7b1-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-175">version</span><span class="sxs-lookup"><span data-stu-id="ce7b1-175">version</span></span>|<span data-ttu-id="ce7b1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ce7b1-176">Int32</span></span>|<span data-ttu-id="ce7b1-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-177">Version of the device configuration.</span></span> <span data-ttu-id="ce7b1-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce7b1-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce7b1-179">bundleId</span><span class="sxs-lookup"><span data-stu-id="ce7b1-179">bundleId</span></span>|<span data-ttu-id="ce7b1-180">String</span><span class="sxs-lookup"><span data-stu-id="ce7b1-180">String</span></span>|<span data-ttu-id="ce7b1-181">目标的捆绑包 id。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-181">Bundle id for targeting.</span></span>|
|<span data-ttu-id="ce7b1-182">fileName</span><span class="sxs-lookup"><span data-stu-id="ce7b1-182">fileName</span></span>|<span data-ttu-id="ce7b1-183">字符串</span><span class="sxs-lookup"><span data-stu-id="ce7b1-183">String</span></span>|<span data-ttu-id="ce7b1-184">配置文件名（\* plist</span><span class="sxs-lookup"><span data-stu-id="ce7b1-184">Configuration file name (\*.plist</span></span> | <span data-ttu-id="ce7b1-185">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-185">\*.xml).</span></span>|
|<span data-ttu-id="ce7b1-186">configurationXml</span><span class="sxs-lookup"><span data-stu-id="ce7b1-186">configurationXml</span></span>|<span data-ttu-id="ce7b1-187">Binary</span><span class="sxs-lookup"><span data-stu-id="ce7b1-187">Binary</span></span>|<span data-ttu-id="ce7b1-188">配置 xml。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-188">Configuration xml.</span></span> <span data-ttu-id="ce7b1-189">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="ce7b1-189">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="ce7b1-190">响应</span><span class="sxs-lookup"><span data-stu-id="ce7b1-190">Response</span></span>
<span data-ttu-id="ce7b1-191">如果成功，此方法在响应`201 Created`正文中返回响应代码和[macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-191">If successful, this method returns a `201 Created` response code and a [macOSCustomAppConfiguration](../resources/intune-deviceconfig-macoscustomappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce7b1-192">示例</span><span class="sxs-lookup"><span data-stu-id="ce7b1-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce7b1-193">请求</span><span class="sxs-lookup"><span data-stu-id="ce7b1-193">Request</span></span>
<span data-ttu-id="ce7b1-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ce7b1-195">响应</span><span class="sxs-lookup"><span data-stu-id="ce7b1-195">Response</span></span>
<span data-ttu-id="ce7b1-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce7b1-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





