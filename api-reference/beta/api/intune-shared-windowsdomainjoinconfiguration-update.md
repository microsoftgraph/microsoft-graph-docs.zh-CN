---
title: 更新 windowsDomainJoinConfiguration
description: 更新 windowsDomainJoinConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 28e3d372db91180be70822f34721748aae8ee9b0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447287"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="49ca3-103">更新 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="49ca3-103">Update windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="49ca3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49ca3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49ca3-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49ca3-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49ca3-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49ca3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49ca3-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49ca3-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49ca3-108">更新[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="49ca3-108">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49ca3-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="49ca3-109">Prerequisites</span></span>
<span data-ttu-id="49ca3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49ca3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49ca3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="49ca3-112">Permission type</span></span>|<span data-ttu-id="49ca3-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="49ca3-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49ca3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49ca3-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="49ca3-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="49ca3-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="49ca3-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ca3-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="49ca3-117">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="49ca3-117">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="49ca3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ca3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="49ca3-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49ca3-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49ca3-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="49ca3-120">Not supported.</span></span>|
|<span data-ttu-id="49ca3-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="49ca3-121">Application</span></span>||
| <span data-ttu-id="49ca3-122">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="49ca3-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="49ca3-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ca3-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="49ca3-124">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="49ca3-124">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="49ca3-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49ca3-125">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49ca3-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49ca3-126">HTTP Request</span></span>

<span data-ttu-id="49ca3-127">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="49ca3-127">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="49ca3-128">**开户**</span><span class="sxs-lookup"><span data-stu-id="49ca3-128">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="49ca3-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="49ca3-129">Request headers</span></span>
|<span data-ttu-id="49ca3-130">标头</span><span class="sxs-lookup"><span data-stu-id="49ca3-130">Header</span></span>|<span data-ttu-id="49ca3-131">值</span><span class="sxs-lookup"><span data-stu-id="49ca3-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49ca3-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="49ca3-132">Authorization</span></span>|<span data-ttu-id="49ca3-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="49ca3-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49ca3-134">接受</span><span class="sxs-lookup"><span data-stu-id="49ca3-134">Accept</span></span>|<span data-ttu-id="49ca3-135">application/json</span><span class="sxs-lookup"><span data-stu-id="49ca3-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49ca3-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="49ca3-136">Request body</span></span>
<span data-ttu-id="49ca3-137">在请求正文中，提供[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49ca3-137">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="49ca3-138">下表显示创建[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="49ca3-138">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="49ca3-139">属性</span><span class="sxs-lookup"><span data-stu-id="49ca3-139">Property</span></span>|<span data-ttu-id="49ca3-140">类型</span><span class="sxs-lookup"><span data-stu-id="49ca3-140">Type</span></span>|<span data-ttu-id="49ca3-141">说明</span><span class="sxs-lookup"><span data-stu-id="49ca3-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49ca3-142">id</span><span class="sxs-lookup"><span data-stu-id="49ca3-142">id</span></span>|<span data-ttu-id="49ca3-143">字符串</span><span class="sxs-lookup"><span data-stu-id="49ca3-143">String</span></span>|<span data-ttu-id="49ca3-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="49ca3-144">Key of the entity.</span></span> <span data-ttu-id="49ca3-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ca3-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49ca3-146">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="49ca3-146">**Device configuration**</span></span>|
|<span data-ttu-id="49ca3-147">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="49ca3-147">activeDirectoryDomainName</span></span>|<span data-ttu-id="49ca3-148">String</span><span class="sxs-lookup"><span data-stu-id="49ca3-148">String</span></span>|<span data-ttu-id="49ca3-149">要加入的 Active Directory 域名称。</span><span class="sxs-lookup"><span data-stu-id="49ca3-149">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="49ca3-150">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="49ca3-150">computerNameStaticPrefix</span></span>|<span data-ttu-id="49ca3-151">String</span><span class="sxs-lookup"><span data-stu-id="49ca3-151">String</span></span>|<span data-ttu-id="49ca3-152">要用于计算机名称的固定前缀。</span><span class="sxs-lookup"><span data-stu-id="49ca3-152">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="49ca3-153">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="49ca3-153">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="49ca3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="49ca3-154">Int32</span></span>|<span data-ttu-id="49ca3-155">作为计算机名称的后缀使用的动态生成字符。</span><span class="sxs-lookup"><span data-stu-id="49ca3-155">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="49ca3-156">有效的值3至14</span><span class="sxs-lookup"><span data-stu-id="49ca3-156">Valid values 3 to 14</span></span>|
|<span data-ttu-id="49ca3-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49ca3-157">createdDateTime</span></span>|<span data-ttu-id="49ca3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49ca3-158">DateTimeOffset</span></span>|<span data-ttu-id="49ca3-159">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="49ca3-159">DateTime the object was created.</span></span> <span data-ttu-id="49ca3-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ca3-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49ca3-161">description</span><span class="sxs-lookup"><span data-stu-id="49ca3-161">description</span></span>|<span data-ttu-id="49ca3-162">String</span><span class="sxs-lookup"><span data-stu-id="49ca3-162">String</span></span>|<span data-ttu-id="49ca3-163">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="49ca3-163">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="49ca3-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ca3-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49ca3-165">displayName</span><span class="sxs-lookup"><span data-stu-id="49ca3-165">displayName</span></span>|<span data-ttu-id="49ca3-166">String</span><span class="sxs-lookup"><span data-stu-id="49ca3-166">String</span></span>|<span data-ttu-id="49ca3-167">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="49ca3-167">Admin provided name of the device configuration.</span></span> <span data-ttu-id="49ca3-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ca3-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49ca3-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49ca3-169">lastModifiedDateTime</span></span>|<span data-ttu-id="49ca3-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49ca3-170">DateTimeOffset</span></span>|<span data-ttu-id="49ca3-171">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="49ca3-171">DateTime the object was last modified.</span></span> <span data-ttu-id="49ca3-172">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ca3-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49ca3-173">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="49ca3-173">organizationalUnit</span></span>|<span data-ttu-id="49ca3-174">String</span><span class="sxs-lookup"><span data-stu-id="49ca3-174">String</span></span>|<span data-ttu-id="49ca3-175">将在其中创建计算机帐户的组织单位（OU）。</span><span class="sxs-lookup"><span data-stu-id="49ca3-175">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="49ca3-176">如果此参数为 NULL，则已知的计算机对象容器将被用作域中的已发布。</span><span class="sxs-lookup"><span data-stu-id="49ca3-176">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="49ca3-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49ca3-177">roleScopeTagIds</span></span>|<span data-ttu-id="49ca3-178">String 集合</span><span class="sxs-lookup"><span data-stu-id="49ca3-178">String collection</span></span>|<span data-ttu-id="49ca3-179">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="49ca3-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="49ca3-180">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ca3-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49ca3-181">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="49ca3-181">supportsScopeTags</span></span>|<span data-ttu-id="49ca3-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="49ca3-182">Boolean</span></span>|<span data-ttu-id="49ca3-183">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="49ca3-183">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="49ca3-184">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="49ca3-184">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="49ca3-185">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="49ca3-185">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="49ca3-186">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="49ca3-186">This property is read-only.</span></span> <span data-ttu-id="49ca3-187">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ca3-187">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="49ca3-188">version</span><span class="sxs-lookup"><span data-stu-id="49ca3-188">version</span></span>|<span data-ttu-id="49ca3-189">Int32</span><span class="sxs-lookup"><span data-stu-id="49ca3-189">Int32</span></span>|<span data-ttu-id="49ca3-190">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="49ca3-190">Version of the device configuration.</span></span> <span data-ttu-id="49ca3-191">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="49ca3-191">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="49ca3-192">注意：请求正文属性支持取决于调用的上下文。</span><span class="sxs-lookup"><span data-stu-id="49ca3-192">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="49ca3-193">并非所有属性都适用于所有工作流。</span><span class="sxs-lookup"><span data-stu-id="49ca3-193">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="49ca3-194">响应</span><span class="sxs-lookup"><span data-stu-id="49ca3-194">Response</span></span>
<span data-ttu-id="49ca3-195">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49ca3-195">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49ca3-196">示例</span><span class="sxs-lookup"><span data-stu-id="49ca3-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="49ca3-197">请求</span><span class="sxs-lookup"><span data-stu-id="49ca3-197">Request</span></span>
<span data-ttu-id="49ca3-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49ca3-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 344

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="49ca3-199">响应</span><span class="sxs-lookup"><span data-stu-id="49ca3-199">Response</span></span>
<span data-ttu-id="49ca3-200">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="49ca3-200">Here is an example of the response.</span></span> <span data-ttu-id="49ca3-201">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="49ca3-201">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="49ca3-202">实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="49ca3-202">Properties returned by actual calls vary according to the context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 521

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value"
}
```









