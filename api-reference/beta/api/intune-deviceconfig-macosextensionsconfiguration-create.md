---
title: 创建 macOSExtensionsConfiguration
description: 创建新的 macOSExtensionsConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9002c6c72809c96ef15ab17dbf855b6c81ea2d4e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948315"
---
# <a name="create-macosextensionsconfiguration"></a><span data-ttu-id="1f2dc-103">创建 macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f2dc-103">Create macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="1f2dc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f2dc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f2dc-106">创建新的[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-106">Create a new [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f2dc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f2dc-107">Prerequisites</span></span>
<span data-ttu-id="1f2dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f2dc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f2dc-110">Permission type</span></span>|<span data-ttu-id="1f2dc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f2dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f2dc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f2dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f2dc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2dc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f2dc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f2dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f2dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-115">Not supported.</span></span>|
|<span data-ttu-id="1f2dc-116">Application</span><span class="sxs-lookup"><span data-stu-id="1f2dc-116">Application</span></span>|<span data-ttu-id="1f2dc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2dc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f2dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f2dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1f2dc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f2dc-119">Request headers</span></span>
|<span data-ttu-id="1f2dc-120">标头</span><span class="sxs-lookup"><span data-stu-id="1f2dc-120">Header</span></span>|<span data-ttu-id="1f2dc-121">值</span><span class="sxs-lookup"><span data-stu-id="1f2dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f2dc-122">授权</span><span class="sxs-lookup"><span data-stu-id="1f2dc-122">Authorization</span></span>|<span data-ttu-id="1f2dc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f2dc-124">接受</span><span class="sxs-lookup"><span data-stu-id="1f2dc-124">Accept</span></span>|<span data-ttu-id="1f2dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f2dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f2dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f2dc-126">Request body</span></span>
<span data-ttu-id="1f2dc-127">在请求正文中，提供 macOSExtensionsConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-127">In the request body, supply a JSON representation for the macOSExtensionsConfiguration object.</span></span>

<span data-ttu-id="1f2dc-128">下表显示创建 macOSExtensionsConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-128">The following table shows the properties that are required when you create the macOSExtensionsConfiguration.</span></span>

|<span data-ttu-id="1f2dc-129">属性</span><span class="sxs-lookup"><span data-stu-id="1f2dc-129">Property</span></span>|<span data-ttu-id="1f2dc-130">类型</span><span class="sxs-lookup"><span data-stu-id="1f2dc-130">Type</span></span>|<span data-ttu-id="1f2dc-131">说明</span><span class="sxs-lookup"><span data-stu-id="1f2dc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f2dc-132">id</span><span class="sxs-lookup"><span data-stu-id="1f2dc-132">id</span></span>|<span data-ttu-id="1f2dc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="1f2dc-133">String</span></span>|<span data-ttu-id="1f2dc-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-134">Key of the entity.</span></span> <span data-ttu-id="1f2dc-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f2dc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1f2dc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f2dc-137">DateTimeOffset</span></span>|<span data-ttu-id="1f2dc-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1f2dc-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1f2dc-140">roleScopeTagIds</span></span>|<span data-ttu-id="1f2dc-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1f2dc-141">String collection</span></span>|<span data-ttu-id="1f2dc-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1f2dc-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1f2dc-144">supportsScopeTags</span></span>|<span data-ttu-id="1f2dc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f2dc-145">Boolean</span></span>|<span data-ttu-id="1f2dc-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1f2dc-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1f2dc-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1f2dc-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-149">This property is read-only.</span></span> <span data-ttu-id="1f2dc-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1f2dc-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1f2dc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1f2dc-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1f2dc-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1f2dc-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1f2dc-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1f2dc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1f2dc-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1f2dc-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1f2dc-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1f2dc-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1f2dc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1f2dc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1f2dc-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1f2dc-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f2dc-163">createdDateTime</span></span>|<span data-ttu-id="1f2dc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f2dc-164">DateTimeOffset</span></span>|<span data-ttu-id="1f2dc-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-165">DateTime the object was created.</span></span> <span data-ttu-id="1f2dc-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-167">说明</span><span class="sxs-lookup"><span data-stu-id="1f2dc-167">description</span></span>|<span data-ttu-id="1f2dc-168">String</span><span class="sxs-lookup"><span data-stu-id="1f2dc-168">String</span></span>|<span data-ttu-id="1f2dc-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f2dc-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1f2dc-171">displayName</span></span>|<span data-ttu-id="1f2dc-172">String</span><span class="sxs-lookup"><span data-stu-id="1f2dc-172">String</span></span>|<span data-ttu-id="1f2dc-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f2dc-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-175">version</span><span class="sxs-lookup"><span data-stu-id="1f2dc-175">version</span></span>|<span data-ttu-id="1f2dc-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1f2dc-176">Int32</span></span>|<span data-ttu-id="1f2dc-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-177">Version of the device configuration.</span></span> <span data-ttu-id="1f2dc-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f2dc-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f2dc-179">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="1f2dc-179">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="1f2dc-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f2dc-180">Boolean</span></span>|<span data-ttu-id="1f2dc-181">如果设置为 true，则用户可以批准配置文件配置文件未明确允许的其他内核扩展。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-181">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="1f2dc-182">kernelExtensionAllowedTeamIdentifiers</span><span class="sxs-lookup"><span data-stu-id="1f2dc-182">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="1f2dc-183">String collection</span><span class="sxs-lookup"><span data-stu-id="1f2dc-183">String collection</span></span>|<span data-ttu-id="1f2dc-184">将允许加载此列表中由团队标识符有效签名的所有内核扩展。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-184">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="1f2dc-185">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="1f2dc-185">kernelExtensionsAllowed</span></span>|<span data-ttu-id="1f2dc-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)集合</span><span class="sxs-lookup"><span data-stu-id="1f2dc-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="1f2dc-187">将允许加载的内核扩展的列表。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-187">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="1f2dc-188">.</span><span class="sxs-lookup"><span data-stu-id="1f2dc-188"></span></span> <span data-ttu-id="1f2dc-189">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-189">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1f2dc-190">响应</span><span class="sxs-lookup"><span data-stu-id="1f2dc-190">Response</span></span>
<span data-ttu-id="1f2dc-191">如果成功，此方法在响应`201 Created`正文中返回响应代码和[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-191">If successful, this method returns a `201 Created` response code and a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f2dc-192">示例</span><span class="sxs-lookup"><span data-stu-id="1f2dc-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f2dc-193">请求</span><span class="sxs-lookup"><span data-stu-id="1f2dc-193">Request</span></span>
<span data-ttu-id="1f2dc-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1383

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
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
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1f2dc-195">响应</span><span class="sxs-lookup"><span data-stu-id="1f2dc-195">Response</span></span>
<span data-ttu-id="1f2dc-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f2dc-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1555

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
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
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```





