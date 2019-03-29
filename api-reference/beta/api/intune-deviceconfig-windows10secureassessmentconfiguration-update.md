---
title: 更新 windows10SecureAssessmentConfiguration
description: 更新 windows10SecureAssessmentConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ebff2b3c12e605727fd0eeff5f953713d5303b8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984462"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="cd557-103">更新 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd557-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="cd557-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd557-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd557-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd557-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd557-106">更新 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cd557-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd557-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd557-107">Prerequisites</span></span>
<span data-ttu-id="cd557-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd557-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd557-110">Permission type</span></span>|<span data-ttu-id="cd557-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd557-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd557-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd557-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd557-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd557-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd557-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd557-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd557-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd557-115">Not supported.</span></span>|
|<span data-ttu-id="cd557-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd557-116">Application</span></span>|<span data-ttu-id="cd557-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd557-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd557-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd557-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cd557-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd557-119">Request headers</span></span>
|<span data-ttu-id="cd557-120">标头</span><span class="sxs-lookup"><span data-stu-id="cd557-120">Header</span></span>|<span data-ttu-id="cd557-121">值</span><span class="sxs-lookup"><span data-stu-id="cd557-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd557-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd557-122">Authorization</span></span>|<span data-ttu-id="cd557-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd557-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd557-124">接受</span><span class="sxs-lookup"><span data-stu-id="cd557-124">Accept</span></span>|<span data-ttu-id="cd557-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd557-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd557-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd557-126">Request body</span></span>
<span data-ttu-id="cd557-127">在请求正文中，提供 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd557-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="cd557-128">下表显示创建 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cd557-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="cd557-129">属性</span><span class="sxs-lookup"><span data-stu-id="cd557-129">Property</span></span>|<span data-ttu-id="cd557-130">类型</span><span class="sxs-lookup"><span data-stu-id="cd557-130">Type</span></span>|<span data-ttu-id="cd557-131">说明</span><span class="sxs-lookup"><span data-stu-id="cd557-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd557-132">id</span><span class="sxs-lookup"><span data-stu-id="cd557-132">id</span></span>|<span data-ttu-id="cd557-133">String</span><span class="sxs-lookup"><span data-stu-id="cd557-133">String</span></span>|<span data-ttu-id="cd557-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cd557-134">Key of the entity.</span></span> <span data-ttu-id="cd557-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd557-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd557-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd557-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cd557-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd557-137">DateTimeOffset</span></span>|<span data-ttu-id="cd557-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cd557-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cd557-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd557-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd557-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cd557-140">roleScopeTagIds</span></span>|<span data-ttu-id="cd557-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="cd557-141">String collection</span></span>|<span data-ttu-id="cd557-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="cd557-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cd557-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd557-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd557-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cd557-144">supportsScopeTags</span></span>|<span data-ttu-id="cd557-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd557-145">Boolean</span></span>|<span data-ttu-id="cd557-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="cd557-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cd557-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="cd557-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cd557-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="cd557-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cd557-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="cd557-149">This property is read-only.</span></span> <span data-ttu-id="cd557-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd557-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd557-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd557-151">createdDateTime</span></span>|<span data-ttu-id="cd557-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd557-152">DateTimeOffset</span></span>|<span data-ttu-id="cd557-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cd557-153">DateTime the object was created.</span></span> <span data-ttu-id="cd557-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd557-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd557-155">description</span><span class="sxs-lookup"><span data-stu-id="cd557-155">description</span></span>|<span data-ttu-id="cd557-156">String</span><span class="sxs-lookup"><span data-stu-id="cd557-156">String</span></span>|<span data-ttu-id="cd557-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cd557-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cd557-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd557-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd557-159">displayName</span><span class="sxs-lookup"><span data-stu-id="cd557-159">displayName</span></span>|<span data-ttu-id="cd557-160">String</span><span class="sxs-lookup"><span data-stu-id="cd557-160">String</span></span>|<span data-ttu-id="cd557-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cd557-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cd557-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd557-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd557-163">version</span><span class="sxs-lookup"><span data-stu-id="cd557-163">version</span></span>|<span data-ttu-id="cd557-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cd557-164">Int32</span></span>|<span data-ttu-id="cd557-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cd557-165">Version of the device configuration.</span></span> <span data-ttu-id="cd557-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd557-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cd557-167">launchUri</span><span class="sxs-lookup"><span data-stu-id="cd557-167">launchUri</span></span>|<span data-ttu-id="cd557-168">String</span><span class="sxs-lookup"><span data-stu-id="cd557-168">String</span></span>|<span data-ttu-id="cd557-169">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="cd557-169">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="cd557-170">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="cd557-170">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="cd557-171">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="cd557-171">configurationAccount</span></span>|<span data-ttu-id="cd557-172">String</span><span class="sxs-lookup"><span data-stu-id="cd557-172">String</span></span>|<span data-ttu-id="cd557-173">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="cd557-173">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="cd557-174">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="cd557-174">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="cd557-175">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="cd557-175">configurationAccountType</span></span>|[<span data-ttu-id="cd557-176">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="cd557-176">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="cd557-177">由 ConfigurationAccount 使用的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="cd557-177">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="cd557-178">可取值为：`azureADAccount`、`domainAccount`、`localAccount`。</span><span class="sxs-lookup"><span data-stu-id="cd557-178">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`.</span></span>|
|<span data-ttu-id="cd557-179">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="cd557-179">allowPrinting</span></span>|<span data-ttu-id="cd557-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd557-180">Boolean</span></span>|<span data-ttu-id="cd557-181">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="cd557-181">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="cd557-182">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="cd557-182">allowScreenCapture</span></span>|<span data-ttu-id="cd557-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd557-183">Boolean</span></span>|<span data-ttu-id="cd557-184">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="cd557-184">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="cd557-185">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="cd557-185">allowTextSuggestion</span></span>|<span data-ttu-id="cd557-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd557-186">Boolean</span></span>|<span data-ttu-id="cd557-187">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="cd557-187">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="cd557-188">响应</span><span class="sxs-lookup"><span data-stu-id="cd557-188">Response</span></span>
<span data-ttu-id="cd557-189">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd557-189">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd557-190">示例</span><span class="sxs-lookup"><span data-stu-id="cd557-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd557-191">请求</span><span class="sxs-lookup"><span data-stu-id="cd557-191">Request</span></span>
<span data-ttu-id="cd557-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd557-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cd557-193">响应</span><span class="sxs-lookup"><span data-stu-id="cd557-193">Response</span></span>
<span data-ttu-id="cd557-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd557-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




