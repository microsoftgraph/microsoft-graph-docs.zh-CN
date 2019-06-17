---
title: 创建 windows10SecureAssessmentConfiguration
description: 创建新的 windows10SecureAssessmentConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b94b94941b0b4f2f5b90a750100e4ad5798988bf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962412"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="9d412-103">创建 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="9d412-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="9d412-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9d412-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d412-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d412-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d412-106">创建新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d412-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d412-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9d412-107">Prerequisites</span></span>
<span data-ttu-id="9d412-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d412-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d412-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d412-110">Permission type</span></span>|<span data-ttu-id="9d412-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9d412-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d412-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d412-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d412-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d412-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d412-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d412-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d412-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d412-115">Not supported.</span></span>|
|<span data-ttu-id="9d412-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d412-116">Application</span></span>|<span data-ttu-id="9d412-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d412-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d412-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d412-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9d412-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d412-119">Request headers</span></span>
|<span data-ttu-id="9d412-120">标头</span><span class="sxs-lookup"><span data-stu-id="9d412-120">Header</span></span>|<span data-ttu-id="9d412-121">值</span><span class="sxs-lookup"><span data-stu-id="9d412-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d412-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d412-122">Authorization</span></span>|<span data-ttu-id="9d412-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9d412-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d412-124">接受</span><span class="sxs-lookup"><span data-stu-id="9d412-124">Accept</span></span>|<span data-ttu-id="9d412-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d412-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d412-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d412-126">Request body</span></span>
<span data-ttu-id="9d412-127">在请求正文中，提供 windows10SecureAssessmentConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d412-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="9d412-128">下表显示创建 windows10SecureAssessmentConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9d412-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="9d412-129">属性</span><span class="sxs-lookup"><span data-stu-id="9d412-129">Property</span></span>|<span data-ttu-id="9d412-130">类型</span><span class="sxs-lookup"><span data-stu-id="9d412-130">Type</span></span>|<span data-ttu-id="9d412-131">说明</span><span class="sxs-lookup"><span data-stu-id="9d412-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d412-132">id</span><span class="sxs-lookup"><span data-stu-id="9d412-132">id</span></span>|<span data-ttu-id="9d412-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9d412-133">String</span></span>|<span data-ttu-id="9d412-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9d412-134">Key of the entity.</span></span> <span data-ttu-id="9d412-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d412-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9d412-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d412-137">DateTimeOffset</span></span>|<span data-ttu-id="9d412-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9d412-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9d412-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9d412-140">roleScopeTagIds</span></span>|<span data-ttu-id="9d412-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9d412-141">String collection</span></span>|<span data-ttu-id="9d412-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9d412-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9d412-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9d412-144">supportsScopeTags</span></span>|<span data-ttu-id="9d412-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d412-145">Boolean</span></span>|<span data-ttu-id="9d412-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9d412-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9d412-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9d412-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9d412-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9d412-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9d412-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9d412-149">This property is read-only.</span></span> <span data-ttu-id="9d412-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9d412-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9d412-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9d412-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9d412-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="9d412-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9d412-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9d412-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9d412-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9d412-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9d412-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9d412-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9d412-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9d412-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9d412-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9d412-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9d412-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="9d412-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9d412-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d412-163">createdDateTime</span></span>|<span data-ttu-id="9d412-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d412-164">DateTimeOffset</span></span>|<span data-ttu-id="9d412-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9d412-165">DateTime the object was created.</span></span> <span data-ttu-id="9d412-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-167">说明</span><span class="sxs-lookup"><span data-stu-id="9d412-167">description</span></span>|<span data-ttu-id="9d412-168">String</span><span class="sxs-lookup"><span data-stu-id="9d412-168">String</span></span>|<span data-ttu-id="9d412-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9d412-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9d412-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9d412-171">displayName</span></span>|<span data-ttu-id="9d412-172">字符串</span><span class="sxs-lookup"><span data-stu-id="9d412-172">String</span></span>|<span data-ttu-id="9d412-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9d412-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9d412-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-175">version</span><span class="sxs-lookup"><span data-stu-id="9d412-175">version</span></span>|<span data-ttu-id="9d412-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9d412-176">Int32</span></span>|<span data-ttu-id="9d412-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9d412-177">Version of the device configuration.</span></span> <span data-ttu-id="9d412-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9d412-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d412-179">launchUri</span><span class="sxs-lookup"><span data-stu-id="9d412-179">launchUri</span></span>|<span data-ttu-id="9d412-180">String</span><span class="sxs-lookup"><span data-stu-id="9d412-180">String</span></span>|<span data-ttu-id="9d412-181">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="9d412-181">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="9d412-182">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="9d412-182">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="9d412-183">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="9d412-183">configurationAccount</span></span>|<span data-ttu-id="9d412-184">String</span><span class="sxs-lookup"><span data-stu-id="9d412-184">String</span></span>|<span data-ttu-id="9d412-185">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="9d412-185">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="9d412-186">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="9d412-186">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="9d412-187">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="9d412-187">configurationAccountType</span></span>|[<span data-ttu-id="9d412-188">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="9d412-188">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="9d412-189">由 ConfigurationAccount 使用的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="9d412-189">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="9d412-190">可取值为：`azureADAccount`、`domainAccount`、`localAccount`。</span><span class="sxs-lookup"><span data-stu-id="9d412-190">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="9d412-191">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="9d412-191">allowPrinting</span></span>|<span data-ttu-id="9d412-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d412-192">Boolean</span></span>|<span data-ttu-id="9d412-193">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="9d412-193">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="9d412-194">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="9d412-194">allowScreenCapture</span></span>|<span data-ttu-id="9d412-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d412-195">Boolean</span></span>|<span data-ttu-id="9d412-196">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="9d412-196">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="9d412-197">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="9d412-197">allowTextSuggestion</span></span>|<span data-ttu-id="9d412-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d412-198">Boolean</span></span>|<span data-ttu-id="9d412-199">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="9d412-199">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="9d412-200">响应</span><span class="sxs-lookup"><span data-stu-id="9d412-200">Response</span></span>
<span data-ttu-id="9d412-201">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9d412-201">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d412-202">示例</span><span class="sxs-lookup"><span data-stu-id="9d412-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d412-203">请求</span><span class="sxs-lookup"><span data-stu-id="9d412-203">Request</span></span>
<span data-ttu-id="9d412-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d412-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1272

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
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
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="9d412-205">响应</span><span class="sxs-lookup"><span data-stu-id="9d412-205">Response</span></span>
<span data-ttu-id="9d412-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9d412-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1444

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
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
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```





