---
title: 更新 androidOmaCpConfiguration
description: 更新 androidOmaCpConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8853e1da34d5b7ac789a6dbf1e3a8a115ebaef57
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970042"
---
# <a name="update-androidomacpconfiguration"></a><span data-ttu-id="d1ea4-103">更新 androidOmaCpConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1ea4-103">Update androidOmaCpConfiguration</span></span>

> <span data-ttu-id="d1ea4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1ea4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1ea4-106">更新[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-106">Update the properties of a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1ea4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d1ea4-107">Prerequisites</span></span>
<span data-ttu-id="d1ea4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1ea4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1ea4-110">Permission type</span></span>|<span data-ttu-id="d1ea4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d1ea4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1ea4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1ea4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1ea4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1ea4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1ea4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1ea4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1ea4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-115">Not supported.</span></span>|
|<span data-ttu-id="d1ea4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1ea4-116">Application</span></span>|<span data-ttu-id="d1ea4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1ea4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1ea4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d1ea4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1ea4-119">Request headers</span></span>
|<span data-ttu-id="d1ea4-120">标头</span><span class="sxs-lookup"><span data-stu-id="d1ea4-120">Header</span></span>|<span data-ttu-id="d1ea4-121">值</span><span class="sxs-lookup"><span data-stu-id="d1ea4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1ea4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1ea4-122">Authorization</span></span>|<span data-ttu-id="d1ea4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1ea4-124">接受</span><span class="sxs-lookup"><span data-stu-id="d1ea4-124">Accept</span></span>|<span data-ttu-id="d1ea4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d1ea4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1ea4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1ea4-126">Request body</span></span>
<span data-ttu-id="d1ea4-127">在请求正文中, 提供[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-127">In the request body, supply a JSON representation for the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

<span data-ttu-id="d1ea4-128">下表显示创建[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-128">The following table shows the properties that are required when you create the [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md).</span></span>

|<span data-ttu-id="d1ea4-129">属性</span><span class="sxs-lookup"><span data-stu-id="d1ea4-129">Property</span></span>|<span data-ttu-id="d1ea4-130">类型</span><span class="sxs-lookup"><span data-stu-id="d1ea4-130">Type</span></span>|<span data-ttu-id="d1ea4-131">说明</span><span class="sxs-lookup"><span data-stu-id="d1ea4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1ea4-132">id</span><span class="sxs-lookup"><span data-stu-id="d1ea4-132">id</span></span>|<span data-ttu-id="d1ea4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d1ea4-133">String</span></span>|<span data-ttu-id="d1ea4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-134">Key of the entity.</span></span> <span data-ttu-id="d1ea4-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1ea4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d1ea4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1ea4-137">DateTimeOffset</span></span>|<span data-ttu-id="d1ea4-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d1ea4-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d1ea4-140">roleScopeTagIds</span></span>|<span data-ttu-id="d1ea4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d1ea4-141">String collection</span></span>|<span data-ttu-id="d1ea4-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d1ea4-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d1ea4-144">supportsScopeTags</span></span>|<span data-ttu-id="d1ea4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1ea4-145">Boolean</span></span>|<span data-ttu-id="d1ea4-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d1ea4-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d1ea4-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d1ea4-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-149">This property is read-only.</span></span> <span data-ttu-id="d1ea4-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d1ea4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d1ea4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d1ea4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d1ea4-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d1ea4-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d1ea4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d1ea4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d1ea4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d1ea4-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d1ea4-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d1ea4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d1ea4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d1ea4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d1ea4-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d1ea4-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1ea4-163">createdDateTime</span></span>|<span data-ttu-id="d1ea4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1ea4-164">DateTimeOffset</span></span>|<span data-ttu-id="d1ea4-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-165">DateTime the object was created.</span></span> <span data-ttu-id="d1ea4-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-167">说明</span><span class="sxs-lookup"><span data-stu-id="d1ea4-167">description</span></span>|<span data-ttu-id="d1ea4-168">String</span><span class="sxs-lookup"><span data-stu-id="d1ea4-168">String</span></span>|<span data-ttu-id="d1ea4-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d1ea4-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d1ea4-171">displayName</span></span>|<span data-ttu-id="d1ea4-172">String</span><span class="sxs-lookup"><span data-stu-id="d1ea4-172">String</span></span>|<span data-ttu-id="d1ea4-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d1ea4-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-175">version</span><span class="sxs-lookup"><span data-stu-id="d1ea4-175">version</span></span>|<span data-ttu-id="d1ea4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d1ea4-176">Int32</span></span>|<span data-ttu-id="d1ea4-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-177">Version of the device configuration.</span></span> <span data-ttu-id="d1ea4-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1ea4-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1ea4-179">configurationXml</span><span class="sxs-lookup"><span data-stu-id="d1ea4-179">configurationXml</span></span>|<span data-ttu-id="d1ea4-180">Binary</span><span class="sxs-lookup"><span data-stu-id="d1ea4-180">Binary</span></span>|<span data-ttu-id="d1ea4-181">将应用于设备的配置 XML。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-181">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="d1ea4-182">读取时, 它只提供占位符字符串, 因为原始数据经过加密和存储。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-182">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="d1ea4-183">响应</span><span class="sxs-lookup"><span data-stu-id="d1ea4-183">Response</span></span>
<span data-ttu-id="d1ea4-184">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-184">If successful, this method returns a `200 OK` response code and an updated [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1ea4-185">示例</span><span class="sxs-lookup"><span data-stu-id="d1ea4-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1ea4-186">请求</span><span class="sxs-lookup"><span data-stu-id="d1ea4-186">Request</span></span>
<span data-ttu-id="d1ea4-187">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1079

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
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
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="d1ea4-188">响应</span><span class="sxs-lookup"><span data-stu-id="d1ea4-188">Response</span></span>
<span data-ttu-id="d1ea4-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1ea4-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1251

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
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
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```





