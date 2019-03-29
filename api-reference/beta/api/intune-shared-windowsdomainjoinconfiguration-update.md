---
title: 更新 windowsDomainJoinConfiguration
description: 更新 windowsDomainJoinConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 66314179f65748abca432dcf4f41bab3c16ebd32
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969636"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="63e4e-103">更新 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="63e4e-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="63e4e-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="63e4e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63e4e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63e4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63e4e-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63e4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63e4e-107">更新[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="63e4e-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63e4e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="63e4e-108">Prerequisites</span></span>
<span data-ttu-id="63e4e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63e4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63e4e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63e4e-111">Permission type</span></span>|<span data-ttu-id="63e4e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63e4e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63e4e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63e4e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="63e4e-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="63e4e-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="63e4e-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63e4e-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="63e4e-116">&nbsp;&nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="63e4e-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="63e4e-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63e4e-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63e4e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63e4e-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63e4e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="63e4e-119">Not supported.</span></span>|
|<span data-ttu-id="63e4e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="63e4e-120">Application</span></span>|<span data-ttu-id="63e4e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="63e4e-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63e4e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63e4e-122">HTTP Request</span></span>

<span data-ttu-id="63e4e-123">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="63e4e-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="63e4e-124">**开户**</span><span class="sxs-lookup"><span data-stu-id="63e4e-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="63e4e-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="63e4e-125">Request headers</span></span>
|<span data-ttu-id="63e4e-126">标头</span><span class="sxs-lookup"><span data-stu-id="63e4e-126">Header</span></span>|<span data-ttu-id="63e4e-127">值</span><span class="sxs-lookup"><span data-stu-id="63e4e-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63e4e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="63e4e-128">Authorization</span></span>|<span data-ttu-id="63e4e-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63e4e-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63e4e-130">接受</span><span class="sxs-lookup"><span data-stu-id="63e4e-130">Accept</span></span>|<span data-ttu-id="63e4e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="63e4e-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63e4e-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="63e4e-132">Request body</span></span>
<span data-ttu-id="63e4e-133">在请求正文中, 提供[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63e4e-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="63e4e-134">下表显示创建[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="63e4e-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="63e4e-135">属性</span><span class="sxs-lookup"><span data-stu-id="63e4e-135">Property</span></span>|<span data-ttu-id="63e4e-136">类型</span><span class="sxs-lookup"><span data-stu-id="63e4e-136">Type</span></span>|<span data-ttu-id="63e4e-137">说明</span><span class="sxs-lookup"><span data-stu-id="63e4e-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63e4e-138">id</span><span class="sxs-lookup"><span data-stu-id="63e4e-138">id</span></span>|<span data-ttu-id="63e4e-139">String</span><span class="sxs-lookup"><span data-stu-id="63e4e-139">String</span></span>|<span data-ttu-id="63e4e-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="63e4e-140">Key of the entity.</span></span> <span data-ttu-id="63e4e-141">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63e4e-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63e4e-142">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="63e4e-142">**Device configuration**</span></span>|
|<span data-ttu-id="63e4e-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="63e4e-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="63e4e-144">String</span><span class="sxs-lookup"><span data-stu-id="63e4e-144">String</span></span>|<span data-ttu-id="63e4e-145">要加入的 Active Directory 域名称。</span><span class="sxs-lookup"><span data-stu-id="63e4e-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="63e4e-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="63e4e-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="63e4e-147">String</span><span class="sxs-lookup"><span data-stu-id="63e4e-147">String</span></span>|<span data-ttu-id="63e4e-148">要用于计算机名称的固定前缀。</span><span class="sxs-lookup"><span data-stu-id="63e4e-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="63e4e-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="63e4e-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="63e4e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="63e4e-150">Int32</span></span>|<span data-ttu-id="63e4e-151">作为计算机名称的后缀使用的动态生成字符。</span><span class="sxs-lookup"><span data-stu-id="63e4e-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="63e4e-152">有效的值3至14</span><span class="sxs-lookup"><span data-stu-id="63e4e-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="63e4e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63e4e-153">createdDateTime</span></span>|<span data-ttu-id="63e4e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63e4e-154">DateTimeOffset</span></span>|<span data-ttu-id="63e4e-155">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="63e4e-155">DateTime the object was created.</span></span> <span data-ttu-id="63e4e-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63e4e-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63e4e-157">description</span><span class="sxs-lookup"><span data-stu-id="63e4e-157">description</span></span>|<span data-ttu-id="63e4e-158">String</span><span class="sxs-lookup"><span data-stu-id="63e4e-158">String</span></span>|<span data-ttu-id="63e4e-159">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="63e4e-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63e4e-160">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63e4e-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63e4e-161">displayName</span><span class="sxs-lookup"><span data-stu-id="63e4e-161">displayName</span></span>|<span data-ttu-id="63e4e-162">String</span><span class="sxs-lookup"><span data-stu-id="63e4e-162">String</span></span>|<span data-ttu-id="63e4e-163">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="63e4e-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63e4e-164">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63e4e-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63e4e-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63e4e-165">lastModifiedDateTime</span></span>|<span data-ttu-id="63e4e-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63e4e-166">DateTimeOffset</span></span>|<span data-ttu-id="63e4e-167">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="63e4e-167">DateTime the object was last modified.</span></span> <span data-ttu-id="63e4e-168">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63e4e-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63e4e-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="63e4e-169">organizationalUnit</span></span>|<span data-ttu-id="63e4e-170">String</span><span class="sxs-lookup"><span data-stu-id="63e4e-170">String</span></span>|<span data-ttu-id="63e4e-171">将在其中创建计算机帐户的组织单位 (OU)。</span><span class="sxs-lookup"><span data-stu-id="63e4e-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="63e4e-172">如果此参数为 NULL, 则已知的计算机对象容器将被用作域中的已发布。</span><span class="sxs-lookup"><span data-stu-id="63e4e-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="63e4e-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="63e4e-173">roleScopeTagIds</span></span>|<span data-ttu-id="63e4e-174">String 集合</span><span class="sxs-lookup"><span data-stu-id="63e4e-174">String collection</span></span>|<span data-ttu-id="63e4e-175">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="63e4e-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="63e4e-176">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63e4e-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63e4e-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="63e4e-177">supportsScopeTags</span></span>|<span data-ttu-id="63e4e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="63e4e-178">Boolean</span></span>|<span data-ttu-id="63e4e-179">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="63e4e-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="63e4e-180">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="63e4e-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="63e4e-181">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="63e4e-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="63e4e-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="63e4e-182">This property is read-only.</span></span> <span data-ttu-id="63e4e-183">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63e4e-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63e4e-184">version</span><span class="sxs-lookup"><span data-stu-id="63e4e-184">version</span></span>|<span data-ttu-id="63e4e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="63e4e-185">Int32</span></span>|<span data-ttu-id="63e4e-186">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="63e4e-186">Version of the device configuration.</span></span> <span data-ttu-id="63e4e-187">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63e4e-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="63e4e-188">注意: 请求正文属性支持取决于调用的上下文。</span><span class="sxs-lookup"><span data-stu-id="63e4e-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="63e4e-189">并非所有属性都适用于所有工作流。</span><span class="sxs-lookup"><span data-stu-id="63e4e-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="63e4e-190">响应</span><span class="sxs-lookup"><span data-stu-id="63e4e-190">Response</span></span>
<span data-ttu-id="63e4e-191">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63e4e-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63e4e-192">示例</span><span class="sxs-lookup"><span data-stu-id="63e4e-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="63e4e-193">请求</span><span class="sxs-lookup"><span data-stu-id="63e4e-193">Request</span></span>
<span data-ttu-id="63e4e-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63e4e-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="63e4e-195">响应</span><span class="sxs-lookup"><span data-stu-id="63e4e-195">Response</span></span>
<span data-ttu-id="63e4e-196">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="63e4e-196">Here is an example of the response.</span></span> <span data-ttu-id="63e4e-197">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63e4e-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="63e4e-198">实际调用返回的属性根据上下文的不同而不同。</span><span class="sxs-lookup"><span data-stu-id="63e4e-198">Properties returned by actual calls vary according to the context.</span></span>
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



