---
title: 创建 iosEducationDeviceConfiguration
description: 创建新的 iosEducationDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 186eb819c790e9baa63b3cc0dc027bcbf142e245
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439322"
---
# <a name="create-ioseducationdeviceconfiguration"></a><span data-ttu-id="b8974-103">创建 iosEducationDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8974-103">Create iosEducationDeviceConfiguration</span></span>

<span data-ttu-id="b8974-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8974-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8974-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8974-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8974-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8974-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8974-107">创建新的[iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8974-107">Create a new [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8974-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8974-108">Prerequisites</span></span>
<span data-ttu-id="b8974-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8974-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8974-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8974-111">Permission type</span></span>|<span data-ttu-id="b8974-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8974-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8974-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8974-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8974-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8974-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8974-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8974-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8974-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8974-116">Not supported.</span></span>|
|<span data-ttu-id="b8974-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8974-117">Application</span></span>|<span data-ttu-id="b8974-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8974-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8974-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8974-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8974-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8974-120">Request headers</span></span>
|<span data-ttu-id="b8974-121">标头</span><span class="sxs-lookup"><span data-stu-id="b8974-121">Header</span></span>|<span data-ttu-id="b8974-122">值</span><span class="sxs-lookup"><span data-stu-id="b8974-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8974-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8974-123">Authorization</span></span>|<span data-ttu-id="b8974-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8974-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8974-125">接受</span><span class="sxs-lookup"><span data-stu-id="b8974-125">Accept</span></span>|<span data-ttu-id="b8974-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8974-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8974-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8974-127">Request body</span></span>
<span data-ttu-id="b8974-128">在请求正文中，提供 iosEducationDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8974-128">In the request body, supply a JSON representation for the iosEducationDeviceConfiguration object.</span></span>

<span data-ttu-id="b8974-129">下表显示创建 iosEducationDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b8974-129">The following table shows the properties that are required when you create the iosEducationDeviceConfiguration.</span></span>

|<span data-ttu-id="b8974-130">属性</span><span class="sxs-lookup"><span data-stu-id="b8974-130">Property</span></span>|<span data-ttu-id="b8974-131">类型</span><span class="sxs-lookup"><span data-stu-id="b8974-131">Type</span></span>|<span data-ttu-id="b8974-132">说明</span><span class="sxs-lookup"><span data-stu-id="b8974-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8974-133">id</span><span class="sxs-lookup"><span data-stu-id="b8974-133">id</span></span>|<span data-ttu-id="b8974-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b8974-134">String</span></span>|<span data-ttu-id="b8974-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8974-135">Key of the entity.</span></span> <span data-ttu-id="b8974-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8974-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b8974-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8974-138">DateTimeOffset</span></span>|<span data-ttu-id="b8974-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b8974-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b8974-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8974-141">roleScopeTagIds</span></span>|<span data-ttu-id="b8974-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b8974-142">String collection</span></span>|<span data-ttu-id="b8974-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b8974-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b8974-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b8974-145">supportsScopeTags</span></span>|<span data-ttu-id="b8974-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8974-146">Boolean</span></span>|<span data-ttu-id="b8974-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b8974-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b8974-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b8974-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b8974-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b8974-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b8974-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b8974-150">This property is read-only.</span></span> <span data-ttu-id="b8974-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b8974-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b8974-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b8974-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b8974-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b8974-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b8974-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b8974-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b8974-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b8974-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b8974-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b8974-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b8974-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b8974-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b8974-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b8974-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b8974-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b8974-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b8974-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8974-164">createdDateTime</span></span>|<span data-ttu-id="b8974-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8974-165">DateTimeOffset</span></span>|<span data-ttu-id="b8974-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b8974-166">DateTime the object was created.</span></span> <span data-ttu-id="b8974-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-168">description</span><span class="sxs-lookup"><span data-stu-id="b8974-168">description</span></span>|<span data-ttu-id="b8974-169">String</span><span class="sxs-lookup"><span data-stu-id="b8974-169">String</span></span>|<span data-ttu-id="b8974-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b8974-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8974-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b8974-172">displayName</span></span>|<span data-ttu-id="b8974-173">String</span><span class="sxs-lookup"><span data-stu-id="b8974-173">String</span></span>|<span data-ttu-id="b8974-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b8974-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8974-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8974-176">version</span><span class="sxs-lookup"><span data-stu-id="b8974-176">version</span></span>|<span data-ttu-id="b8974-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b8974-177">Int32</span></span>|<span data-ttu-id="b8974-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b8974-178">Version of the device configuration.</span></span> <span data-ttu-id="b8974-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8974-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b8974-180">响应</span><span class="sxs-lookup"><span data-stu-id="b8974-180">Response</span></span>
<span data-ttu-id="b8974-181">如果成功，此方法在响应`201 Created`正文中返回响应代码和[iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8974-181">If successful, this method returns a `201 Created` response code and a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8974-182">示例</span><span class="sxs-lookup"><span data-stu-id="b8974-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8974-183">请求</span><span class="sxs-lookup"><span data-stu-id="b8974-183">Request</span></span>
<span data-ttu-id="b8974-184">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8974-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1034

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
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
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="b8974-185">响应</span><span class="sxs-lookup"><span data-stu-id="b8974-185">Response</span></span>
<span data-ttu-id="b8974-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8974-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1206

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
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
  "version": 7
}
```



