---
title: 更新 windowsDomainJoinConfiguration
description: 更新 windowsDomainJoinConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5e6a1430cf53326bb1d3c603f1ac30e1d0160b6a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933664"
---
# <a name="update-windowsdomainjoinconfiguration"></a><span data-ttu-id="567fb-103">更新 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="567fb-103">Update windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="567fb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="567fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="567fb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="567fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="567fb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="567fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="567fb-107">更新[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="567fb-107">Update the properties of a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="567fb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="567fb-108">Prerequisites</span></span>
<span data-ttu-id="567fb-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="567fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="567fb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="567fb-111">Permission type</span></span>|<span data-ttu-id="567fb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="567fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="567fb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="567fb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="567fb-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="567fb-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="567fb-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="567fb-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="567fb-116">&nbsp; &nbsp; **注册**</span><span class="sxs-lookup"><span data-stu-id="567fb-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="567fb-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="567fb-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="567fb-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="567fb-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="567fb-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="567fb-119">Not supported.</span></span>|
|<span data-ttu-id="567fb-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="567fb-120">Application</span></span>|<span data-ttu-id="567fb-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="567fb-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="567fb-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="567fb-122">HTTP Request</span></span>

<span data-ttu-id="567fb-123">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="567fb-123">**Device configuration**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="567fb-124">**注册**</span><span class="sxs-lookup"><span data-stu-id="567fb-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="567fb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="567fb-125">Request headers</span></span>
|<span data-ttu-id="567fb-126">标头</span><span class="sxs-lookup"><span data-stu-id="567fb-126">Header</span></span>|<span data-ttu-id="567fb-127">值</span><span class="sxs-lookup"><span data-stu-id="567fb-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="567fb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="567fb-128">Authorization</span></span>|<span data-ttu-id="567fb-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="567fb-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="567fb-130">Accept</span><span class="sxs-lookup"><span data-stu-id="567fb-130">Accept</span></span>|<span data-ttu-id="567fb-131">application/json</span><span class="sxs-lookup"><span data-stu-id="567fb-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="567fb-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="567fb-132">Request body</span></span>
<span data-ttu-id="567fb-133">在请求正文中，提供[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="567fb-133">In the request body, supply a JSON representation for the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

<span data-ttu-id="567fb-134">下表显示时创建[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="567fb-134">The following table shows the properties that are required when you create the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>

|<span data-ttu-id="567fb-135">属性</span><span class="sxs-lookup"><span data-stu-id="567fb-135">Property</span></span>|<span data-ttu-id="567fb-136">类型</span><span class="sxs-lookup"><span data-stu-id="567fb-136">Type</span></span>|<span data-ttu-id="567fb-137">说明</span><span class="sxs-lookup"><span data-stu-id="567fb-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="567fb-138">id</span><span class="sxs-lookup"><span data-stu-id="567fb-138">id</span></span>|<span data-ttu-id="567fb-139">String</span><span class="sxs-lookup"><span data-stu-id="567fb-139">String</span></span>|<span data-ttu-id="567fb-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="567fb-140">Key of the entity.</span></span> <span data-ttu-id="567fb-141">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567fb-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567fb-142">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="567fb-142">**Device configuration**</span></span>|
|<span data-ttu-id="567fb-143">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="567fb-143">activeDirectoryDomainName</span></span>|<span data-ttu-id="567fb-144">字符串</span><span class="sxs-lookup"><span data-stu-id="567fb-144">String</span></span>|<span data-ttu-id="567fb-145">Active Directory 域名加入。</span><span class="sxs-lookup"><span data-stu-id="567fb-145">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="567fb-146">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="567fb-146">computerNameStaticPrefix</span></span>|<span data-ttu-id="567fb-147">字符串</span><span class="sxs-lookup"><span data-stu-id="567fb-147">String</span></span>|<span data-ttu-id="567fb-148">固定的前缀用于计算机名称。</span><span class="sxs-lookup"><span data-stu-id="567fb-148">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="567fb-149">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="567fb-149">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="567fb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="567fb-150">Int32</span></span>|<span data-ttu-id="567fb-151">动态生成的计算机名称用作后缀的字符。</span><span class="sxs-lookup"><span data-stu-id="567fb-151">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="567fb-152">有效值 3 到 14</span><span class="sxs-lookup"><span data-stu-id="567fb-152">Valid values 3 to 14</span></span>|
|<span data-ttu-id="567fb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="567fb-153">createdDateTime</span></span>|<span data-ttu-id="567fb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="567fb-154">DateTimeOffset</span></span>|<span data-ttu-id="567fb-155">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="567fb-155">DateTime the object was created.</span></span> <span data-ttu-id="567fb-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567fb-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567fb-157">description</span><span class="sxs-lookup"><span data-stu-id="567fb-157">description</span></span>|<span data-ttu-id="567fb-158">String</span><span class="sxs-lookup"><span data-stu-id="567fb-158">String</span></span>|<span data-ttu-id="567fb-159">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="567fb-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="567fb-160">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567fb-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567fb-161">displayName</span><span class="sxs-lookup"><span data-stu-id="567fb-161">displayName</span></span>|<span data-ttu-id="567fb-162">String</span><span class="sxs-lookup"><span data-stu-id="567fb-162">String</span></span>|<span data-ttu-id="567fb-163">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="567fb-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="567fb-164">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567fb-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567fb-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="567fb-165">lastModifiedDateTime</span></span>|<span data-ttu-id="567fb-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="567fb-166">DateTimeOffset</span></span>|<span data-ttu-id="567fb-167">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="567fb-167">DateTime the object was last modified.</span></span> <span data-ttu-id="567fb-168">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567fb-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567fb-169">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="567fb-169">organizationalUnit</span></span>|<span data-ttu-id="567fb-170">字符串</span><span class="sxs-lookup"><span data-stu-id="567fb-170">String</span></span>|<span data-ttu-id="567fb-171">将在其中创建计算机帐户组织单位 (OU)。</span><span class="sxs-lookup"><span data-stu-id="567fb-171">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="567fb-172">如果此参数为 NULL，则将发布域中使用已知的计算机对象容器。</span><span class="sxs-lookup"><span data-stu-id="567fb-172">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="567fb-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="567fb-173">roleScopeTagIds</span></span>|<span data-ttu-id="567fb-174">String 集合</span><span class="sxs-lookup"><span data-stu-id="567fb-174">String collection</span></span>|<span data-ttu-id="567fb-175">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="567fb-175">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="567fb-176">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567fb-176">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567fb-177">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="567fb-177">supportsScopeTags</span></span>|<span data-ttu-id="567fb-178">布尔</span><span class="sxs-lookup"><span data-stu-id="567fb-178">Boolean</span></span>|<span data-ttu-id="567fb-179">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="567fb-179">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="567fb-180">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="567fb-180">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="567fb-181">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="567fb-181">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="567fb-182">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="567fb-182">This property is read-only.</span></span> <span data-ttu-id="567fb-183">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567fb-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567fb-184">version</span><span class="sxs-lookup"><span data-stu-id="567fb-184">version</span></span>|<span data-ttu-id="567fb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="567fb-185">Int32</span></span>|<span data-ttu-id="567fb-186">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="567fb-186">Version of the device configuration.</span></span> <span data-ttu-id="567fb-187">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567fb-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



<span data-ttu-id="567fb-188">注意： 请求正文中属性支持取决于呼叫上下文。</span><span class="sxs-lookup"><span data-stu-id="567fb-188">Note: Request body properties support depends on the context of the call.</span></span>  <span data-ttu-id="567fb-189">并非所有属性都都适用于所有工作流。</span><span class="sxs-lookup"><span data-stu-id="567fb-189">Not all properties are appropriate for all workflows.</span></span>

## <a name="response"></a><span data-ttu-id="567fb-190">响应</span><span class="sxs-lookup"><span data-stu-id="567fb-190">Response</span></span>
<span data-ttu-id="567fb-191">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="567fb-191">If successful, this method returns a `200 OK` response code and an updated [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="567fb-192">示例</span><span class="sxs-lookup"><span data-stu-id="567fb-192">Example</span></span>
### <a name="request"></a><span data-ttu-id="567fb-193">请求</span><span class="sxs-lookup"><span data-stu-id="567fb-193">Request</span></span>
<span data-ttu-id="567fb-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="567fb-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="567fb-195">响应</span><span class="sxs-lookup"><span data-stu-id="567fb-195">Response</span></span>
<span data-ttu-id="567fb-196">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="567fb-196">Here is an example of the response.</span></span> <span data-ttu-id="567fb-197">注意：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="567fb-197">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="567fb-198">根据上下文而有所不同实际的调用返回的属性。</span><span class="sxs-lookup"><span data-stu-id="567fb-198">Properties returned by actual calls vary according to the context.</span></span>
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



