---
title: 更新 windowsDomainJoinConfiguration
description: 更新 windowsDomainJoinConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac8732ff9e9b6ee32a36205af919331372154236
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864758"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="1f831-103">更新 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f831-103">Update windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="1f831-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f831-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f831-105">**重要提示：** Microsoft Graph 中的 /beta 版本下的 API 可能会更改。</span><span class="sxs-lookup"><span data-stu-id="1f831-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1f831-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1f831-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f831-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f831-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f831-108">更新 [windowsDomainJoinConfiguration 对象](../resources/intune-shared-windowsdomainjoinconfiguration.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1f831-108">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f831-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f831-109">Prerequisites</span></span>
<span data-ttu-id="1f831-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f831-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f831-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f831-112">Permission type</span></span>|<span data-ttu-id="1f831-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f831-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f831-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f831-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1f831-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="1f831-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1f831-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f831-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="1f831-117">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="1f831-117">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="1f831-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f831-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1f831-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f831-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f831-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f831-120">Not supported.</span></span>|
|<span data-ttu-id="1f831-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f831-121">Application</span></span>||
| <span data-ttu-id="1f831-122">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="1f831-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="1f831-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f831-123">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="1f831-124">&nbsp;&nbsp;**注册**</span><span class="sxs-lookup"><span data-stu-id="1f831-124">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="1f831-125">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f831-125">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f831-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f831-126">HTTP Request</span></span>

<span data-ttu-id="1f831-127">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="1f831-127">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="1f831-128">**注册**</span><span class="sxs-lookup"><span data-stu-id="1f831-128">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="1f831-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f831-129">Request headers</span></span>
|<span data-ttu-id="1f831-130">标头</span><span class="sxs-lookup"><span data-stu-id="1f831-130">Header</span></span>|<span data-ttu-id="1f831-131">值</span><span class="sxs-lookup"><span data-stu-id="1f831-131">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f831-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f831-132">Authorization</span></span>|<span data-ttu-id="1f831-133">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f831-133">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f831-134">接受</span><span class="sxs-lookup"><span data-stu-id="1f831-134">Accept</span></span>|<span data-ttu-id="1f831-135">application/json</span><span class="sxs-lookup"><span data-stu-id="1f831-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f831-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f831-136">Request body</span></span>
<span data-ttu-id="1f831-137">在请求正文中，提供 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f831-137">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="1f831-138">下表显示创建 [windowsDomainJoinConfiguration 时所需的属性](../resources/intune-shared-windowsdomainjoinconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="1f831-138">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="1f831-139">属性</span><span class="sxs-lookup"><span data-stu-id="1f831-139">Property</span></span>|<span data-ttu-id="1f831-140">类型</span><span class="sxs-lookup"><span data-stu-id="1f831-140">Type</span></span>|<span data-ttu-id="1f831-141">说明</span><span class="sxs-lookup"><span data-stu-id="1f831-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f831-142">id</span><span class="sxs-lookup"><span data-stu-id="1f831-142">id</span></span>|<span data-ttu-id="1f831-143">String</span><span class="sxs-lookup"><span data-stu-id="1f831-143">String</span></span>|<span data-ttu-id="1f831-144">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1f831-144">Key of the entity.</span></span> <span data-ttu-id="1f831-145">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f831-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f831-146">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="1f831-146">**Device configuration**</span></span>|
|<span data-ttu-id="1f831-147">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="1f831-147">activeDirectoryDomainName</span></span>|<span data-ttu-id="1f831-148">String</span><span class="sxs-lookup"><span data-stu-id="1f831-148">String</span></span>|<span data-ttu-id="1f831-149">要加入的 Active Directory 域名。</span><span class="sxs-lookup"><span data-stu-id="1f831-149">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="1f831-150">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="1f831-150">computerNameStaticPrefix</span></span>|<span data-ttu-id="1f831-151">String</span><span class="sxs-lookup"><span data-stu-id="1f831-151">String</span></span>|<span data-ttu-id="1f831-152">用于计算机名称的固定前缀。</span><span class="sxs-lookup"><span data-stu-id="1f831-152">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="1f831-153">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="1f831-153">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="1f831-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1f831-154">Int32</span></span>|<span data-ttu-id="1f831-155">动态生成的字符，用作计算机名称的后缀。</span><span class="sxs-lookup"><span data-stu-id="1f831-155">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="1f831-156">有效值为 3 至 14</span><span class="sxs-lookup"><span data-stu-id="1f831-156">Valid values 3 to 14</span></span>|
|<span data-ttu-id="1f831-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f831-157">createdDateTime</span></span>|<span data-ttu-id="1f831-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f831-158">DateTimeOffset</span></span>|<span data-ttu-id="1f831-159">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1f831-159">DateTime the object was created.</span></span> <span data-ttu-id="1f831-160">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f831-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f831-161">说明</span><span class="sxs-lookup"><span data-stu-id="1f831-161">description</span></span>|<span data-ttu-id="1f831-162">String</span><span class="sxs-lookup"><span data-stu-id="1f831-162">String</span></span>|<span data-ttu-id="1f831-163">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1f831-163">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f831-164">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f831-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f831-165">displayName</span><span class="sxs-lookup"><span data-stu-id="1f831-165">displayName</span></span>|<span data-ttu-id="1f831-166">String</span><span class="sxs-lookup"><span data-stu-id="1f831-166">String</span></span>|<span data-ttu-id="1f831-167">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1f831-167">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f831-168">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f831-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f831-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f831-169">lastModifiedDateTime</span></span>|<span data-ttu-id="1f831-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f831-170">DateTimeOffset</span></span>|<span data-ttu-id="1f831-171">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1f831-171">DateTime the object was last modified.</span></span> <span data-ttu-id="1f831-172">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f831-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f831-173">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="1f831-173">organizationalUnit</span></span>|<span data-ttu-id="1f831-174">String</span><span class="sxs-lookup"><span data-stu-id="1f831-174">String</span></span>|<span data-ttu-id="1f831-175">组织 (OU) 将在其中创建计算机帐户的组织单位。</span><span class="sxs-lookup"><span data-stu-id="1f831-175">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="1f831-176">如果此参数为 NULL，则已知的计算机对象容器将用作域中发布的容器。</span><span class="sxs-lookup"><span data-stu-id="1f831-176">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="1f831-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1f831-177">roleScopeTagIds</span></span>|<span data-ttu-id="1f831-178">String 集合</span><span class="sxs-lookup"><span data-stu-id="1f831-178">String collection</span></span>|<span data-ttu-id="1f831-179">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1f831-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1f831-180">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f831-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f831-181">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1f831-181">supportsScopeTags</span></span>|<span data-ttu-id="1f831-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f831-182">Boolean</span></span>|<span data-ttu-id="1f831-183">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="1f831-183">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1f831-184">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="1f831-184">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1f831-185">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="1f831-185">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1f831-186">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1f831-186">This property is read-only.</span></span> <span data-ttu-id="1f831-187">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f831-187">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f831-188">version</span><span class="sxs-lookup"><span data-stu-id="1f831-188">version</span></span>|<span data-ttu-id="1f831-189">Int32</span><span class="sxs-lookup"><span data-stu-id="1f831-189">Int32</span></span>|<span data-ttu-id="1f831-190">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1f831-190">Version of the device configuration.</span></span> <span data-ttu-id="1f831-191">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f831-191">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



<span data-ttu-id="1f831-192">注意：请求正文属性支持取决于调用的上下文。</span><span class="sxs-lookup"><span data-stu-id="1f831-192">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="1f831-193">并非所有属性都适合所有工作流。</span><span class="sxs-lookup"><span data-stu-id="1f831-193">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="1f831-194">响应</span><span class="sxs-lookup"><span data-stu-id="1f831-194">Response</span></span>
<span data-ttu-id="1f831-195">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f831-195">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f831-196">示例</span><span class="sxs-lookup"><span data-stu-id="1f831-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f831-197">请求</span><span class="sxs-lookup"><span data-stu-id="1f831-197">Request</span></span>
<span data-ttu-id="1f831-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f831-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f831-199">响应</span><span class="sxs-lookup"><span data-stu-id="1f831-199">Response</span></span>
<span data-ttu-id="1f831-200">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1f831-200">Here is an example of the response.</span></span> <span data-ttu-id="1f831-201">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1f831-201">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1f831-202">实际调用返回的属性因上下文而异。</span><span class="sxs-lookup"><span data-stu-id="1f831-202">Properties returned by actual calls vary according to the context.</span></span>
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










