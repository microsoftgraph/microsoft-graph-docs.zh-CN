---
title: 更新 windows10SecureAssessmentConfiguration
description: 更新 windows10SecureAssessmentConfiguration 对象的属性。
ms.openlocfilehash: 884b19833ffa63c65adfd9eba991e5577f0aca04
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049354"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="6f1e2-103">更新 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f1e2-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="6f1e2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f1e2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f1e2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f1e2-107">更新 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f1e2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f1e2-108">Prerequisites</span></span>
<span data-ttu-id="6f1e2-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6f1e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f1e2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f1e2-111">Permission type</span></span>|<span data-ttu-id="6f1e2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f1e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f1e2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f1e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f1e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f1e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f1e2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f1e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f1e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-116">Not supported.</span></span>|
|<span data-ttu-id="6f1e2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f1e2-117">Application</span></span>|<span data-ttu-id="6f1e2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f1e2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f1e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6f1e2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f1e2-120">Request headers</span></span>
|<span data-ttu-id="6f1e2-121">标头</span><span class="sxs-lookup"><span data-stu-id="6f1e2-121">Header</span></span>|<span data-ttu-id="6f1e2-122">值</span><span class="sxs-lookup"><span data-stu-id="6f1e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f1e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f1e2-123">Authorization</span></span>|<span data-ttu-id="6f1e2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f1e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f1e2-125">Accept</span></span>|<span data-ttu-id="6f1e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f1e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f1e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f1e2-127">Request body</span></span>
<span data-ttu-id="6f1e2-128">在请求正文中，提供 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="6f1e2-129">下表显示创建 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="6f1e2-130">属性</span><span class="sxs-lookup"><span data-stu-id="6f1e2-130">Property</span></span>|<span data-ttu-id="6f1e2-131">类型</span><span class="sxs-lookup"><span data-stu-id="6f1e2-131">Type</span></span>|<span data-ttu-id="6f1e2-132">说明</span><span class="sxs-lookup"><span data-stu-id="6f1e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f1e2-133">id</span><span class="sxs-lookup"><span data-stu-id="6f1e2-133">id</span></span>|<span data-ttu-id="6f1e2-134">String</span><span class="sxs-lookup"><span data-stu-id="6f1e2-134">String</span></span>|<span data-ttu-id="6f1e2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-135">Key of the entity.</span></span> <span data-ttu-id="6f1e2-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f1e2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f1e2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f1e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f1e2-138">DateTimeOffset</span></span>|<span data-ttu-id="6f1e2-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6f1e2-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f1e2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f1e2-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f1e2-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="6f1e2-142">String collection</span></span>|<span data-ttu-id="6f1e2-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f1e2-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f1e2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6f1e2-145">supportsScopeTags</span></span>|<span data-ttu-id="6f1e2-146">布尔</span><span class="sxs-lookup"><span data-stu-id="6f1e2-146">Boolean</span></span>|<span data-ttu-id="6f1e2-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f1e2-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f1e2-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f1e2-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-150">This property is read-only.</span></span> <span data-ttu-id="6f1e2-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f1e2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f1e2-152">createdDateTime</span></span>|<span data-ttu-id="6f1e2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f1e2-153">DateTimeOffset</span></span>|<span data-ttu-id="6f1e2-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-154">DateTime the object was created.</span></span> <span data-ttu-id="6f1e2-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f1e2-156">description</span><span class="sxs-lookup"><span data-stu-id="6f1e2-156">description</span></span>|<span data-ttu-id="6f1e2-157">String</span><span class="sxs-lookup"><span data-stu-id="6f1e2-157">String</span></span>|<span data-ttu-id="6f1e2-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f1e2-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f1e2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="6f1e2-160">displayName</span></span>|<span data-ttu-id="6f1e2-161">String</span><span class="sxs-lookup"><span data-stu-id="6f1e2-161">String</span></span>|<span data-ttu-id="6f1e2-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f1e2-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f1e2-164">version</span><span class="sxs-lookup"><span data-stu-id="6f1e2-164">version</span></span>|<span data-ttu-id="6f1e2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="6f1e2-165">Int32</span></span>|<span data-ttu-id="6f1e2-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-166">Version of the device configuration.</span></span> <span data-ttu-id="6f1e2-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f1e2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f1e2-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="6f1e2-168">launchUri</span></span>|<span data-ttu-id="6f1e2-169">String</span><span class="sxs-lookup"><span data-stu-id="6f1e2-169">String</span></span>|<span data-ttu-id="6f1e2-170">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="6f1e2-171">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="6f1e2-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="6f1e2-172">configurationAccount</span></span>|<span data-ttu-id="6f1e2-173">String</span><span class="sxs-lookup"><span data-stu-id="6f1e2-173">String</span></span>|<span data-ttu-id="6f1e2-174">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="6f1e2-175">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="6f1e2-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="6f1e2-176">configurationAccountType</span></span>|[<span data-ttu-id="6f1e2-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="6f1e2-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="6f1e2-178">使用 ConfigurationAccount 帐户类型。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="6f1e2-179">可取值为：`azureADAccount`、`domainAccount`、`localAccount`。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="6f1e2-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="6f1e2-180">allowPrinting</span></span>|<span data-ttu-id="6f1e2-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1e2-181">Boolean</span></span>|<span data-ttu-id="6f1e2-182">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="6f1e2-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="6f1e2-183">allowScreenCapture</span></span>|<span data-ttu-id="6f1e2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1e2-184">Boolean</span></span>|<span data-ttu-id="6f1e2-185">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="6f1e2-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="6f1e2-186">allowTextSuggestion</span></span>|<span data-ttu-id="6f1e2-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f1e2-187">Boolean</span></span>|<span data-ttu-id="6f1e2-188">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="6f1e2-189">响应</span><span class="sxs-lookup"><span data-stu-id="6f1e2-189">Response</span></span>
<span data-ttu-id="6f1e2-190">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-190">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f1e2-191">示例</span><span class="sxs-lookup"><span data-stu-id="6f1e2-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f1e2-192">请求</span><span class="sxs-lookup"><span data-stu-id="6f1e2-192">Request</span></span>
<span data-ttu-id="6f1e2-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 486

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="6f1e2-194">响应</span><span class="sxs-lookup"><span data-stu-id="6f1e2-194">Response</span></span>
<span data-ttu-id="6f1e2-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f1e2-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 671

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





