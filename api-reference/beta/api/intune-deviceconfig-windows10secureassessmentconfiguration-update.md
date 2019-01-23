---
title: 更新 windows10SecureAssessmentConfiguration
description: 更新 windows10SecureAssessmentConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4503276def73977eb623eb472b7dd9fcf1446e6f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421408"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="f0bdc-103">更新 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0bdc-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="f0bdc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f0bdc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0bdc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0bdc-107">更新 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0bdc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0bdc-108">Prerequisites</span></span>
<span data-ttu-id="f0bdc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f0bdc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0bdc-111">Permission type</span></span>|<span data-ttu-id="f0bdc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0bdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0bdc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0bdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0bdc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0bdc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0bdc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0bdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0bdc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-116">Not supported.</span></span>|
|<span data-ttu-id="f0bdc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0bdc-117">Application</span></span>|<span data-ttu-id="f0bdc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0bdc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0bdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f0bdc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0bdc-120">Request headers</span></span>
|<span data-ttu-id="f0bdc-121">标头</span><span class="sxs-lookup"><span data-stu-id="f0bdc-121">Header</span></span>|<span data-ttu-id="f0bdc-122">值</span><span class="sxs-lookup"><span data-stu-id="f0bdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0bdc-123">授权</span><span class="sxs-lookup"><span data-stu-id="f0bdc-123">Authorization</span></span>|<span data-ttu-id="f0bdc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0bdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0bdc-125">Accept</span></span>|<span data-ttu-id="f0bdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0bdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0bdc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0bdc-127">Request body</span></span>
<span data-ttu-id="f0bdc-128">在请求正文中，提供 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="f0bdc-129">下表显示创建 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="f0bdc-130">属性</span><span class="sxs-lookup"><span data-stu-id="f0bdc-130">Property</span></span>|<span data-ttu-id="f0bdc-131">类型</span><span class="sxs-lookup"><span data-stu-id="f0bdc-131">Type</span></span>|<span data-ttu-id="f0bdc-132">说明</span><span class="sxs-lookup"><span data-stu-id="f0bdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0bdc-133">id</span><span class="sxs-lookup"><span data-stu-id="f0bdc-133">id</span></span>|<span data-ttu-id="f0bdc-134">String</span><span class="sxs-lookup"><span data-stu-id="f0bdc-134">String</span></span>|<span data-ttu-id="f0bdc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-135">Key of the entity.</span></span> <span data-ttu-id="f0bdc-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0bdc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0bdc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0bdc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f0bdc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0bdc-138">DateTimeOffset</span></span>|<span data-ttu-id="f0bdc-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f0bdc-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0bdc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0bdc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0bdc-141">roleScopeTagIds</span></span>|<span data-ttu-id="f0bdc-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="f0bdc-142">String collection</span></span>|<span data-ttu-id="f0bdc-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f0bdc-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0bdc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0bdc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f0bdc-145">supportsScopeTags</span></span>|<span data-ttu-id="f0bdc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0bdc-146">Boolean</span></span>|<span data-ttu-id="f0bdc-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f0bdc-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f0bdc-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f0bdc-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-150">This property is read-only.</span></span> <span data-ttu-id="f0bdc-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0bdc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0bdc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0bdc-152">createdDateTime</span></span>|<span data-ttu-id="f0bdc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0bdc-153">DateTimeOffset</span></span>|<span data-ttu-id="f0bdc-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-154">DateTime the object was created.</span></span> <span data-ttu-id="f0bdc-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0bdc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0bdc-156">description</span><span class="sxs-lookup"><span data-stu-id="f0bdc-156">description</span></span>|<span data-ttu-id="f0bdc-157">String</span><span class="sxs-lookup"><span data-stu-id="f0bdc-157">String</span></span>|<span data-ttu-id="f0bdc-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0bdc-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0bdc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0bdc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f0bdc-160">displayName</span></span>|<span data-ttu-id="f0bdc-161">String</span><span class="sxs-lookup"><span data-stu-id="f0bdc-161">String</span></span>|<span data-ttu-id="f0bdc-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0bdc-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0bdc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0bdc-164">version</span><span class="sxs-lookup"><span data-stu-id="f0bdc-164">version</span></span>|<span data-ttu-id="f0bdc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f0bdc-165">Int32</span></span>|<span data-ttu-id="f0bdc-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-166">Version of the device configuration.</span></span> <span data-ttu-id="f0bdc-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0bdc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0bdc-168">launchUri</span><span class="sxs-lookup"><span data-stu-id="f0bdc-168">launchUri</span></span>|<span data-ttu-id="f0bdc-169">String</span><span class="sxs-lookup"><span data-stu-id="f0bdc-169">String</span></span>|<span data-ttu-id="f0bdc-170">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-170">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="f0bdc-171">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-171">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="f0bdc-172">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="f0bdc-172">configurationAccount</span></span>|<span data-ttu-id="f0bdc-173">String</span><span class="sxs-lookup"><span data-stu-id="f0bdc-173">String</span></span>|<span data-ttu-id="f0bdc-174">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-174">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="f0bdc-175">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-175">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="f0bdc-176">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="f0bdc-176">configurationAccountType</span></span>|[<span data-ttu-id="f0bdc-177">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="f0bdc-177">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="f0bdc-178">使用 ConfigurationAccount 帐户类型。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-178">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="f0bdc-179">可取值为：`azureADAccount`、`domainAccount`、`localAccount`。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-179">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="f0bdc-180">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="f0bdc-180">allowPrinting</span></span>|<span data-ttu-id="f0bdc-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0bdc-181">Boolean</span></span>|<span data-ttu-id="f0bdc-182">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-182">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="f0bdc-183">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="f0bdc-183">allowScreenCapture</span></span>|<span data-ttu-id="f0bdc-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0bdc-184">Boolean</span></span>|<span data-ttu-id="f0bdc-185">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-185">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="f0bdc-186">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="f0bdc-186">allowTextSuggestion</span></span>|<span data-ttu-id="f0bdc-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0bdc-187">Boolean</span></span>|<span data-ttu-id="f0bdc-188">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-188">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="f0bdc-189">响应</span><span class="sxs-lookup"><span data-stu-id="f0bdc-189">Response</span></span>
<span data-ttu-id="f0bdc-190">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-190">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0bdc-191">示例</span><span class="sxs-lookup"><span data-stu-id="f0bdc-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0bdc-192">请求</span><span class="sxs-lookup"><span data-stu-id="f0bdc-192">Request</span></span>
<span data-ttu-id="f0bdc-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 499

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
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

### <a name="response"></a><span data-ttu-id="f0bdc-194">响应</span><span class="sxs-lookup"><span data-stu-id="f0bdc-194">Response</span></span>
<span data-ttu-id="f0bdc-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0bdc-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




