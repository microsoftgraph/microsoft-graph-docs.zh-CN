---
title: 创建 windowsDomainJoinConfiguration
description: 创建新的 windowsDomainJoinConfiguration 对象。
ms.openlocfilehash: 8069dfac727ee24d96f72875a4cec19fa42b8baa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048793"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="877da-103">创建 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="877da-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="877da-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="877da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="877da-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="877da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="877da-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="877da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="877da-107">创建新的[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="877da-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="877da-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="877da-108">Prerequisites</span></span>
<span data-ttu-id="877da-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="877da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="877da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="877da-111">Permission type</span></span>|<span data-ttu-id="877da-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="877da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="877da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="877da-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="877da-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="877da-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="877da-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="877da-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="877da-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="877da-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="877da-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="877da-117">Not supported.</span></span>|
|<span data-ttu-id="877da-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="877da-118">Application</span></span>|<span data-ttu-id="877da-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="877da-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="877da-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="877da-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="877da-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="877da-121">Request headers</span></span>

|<span data-ttu-id="877da-122">标头</span><span class="sxs-lookup"><span data-stu-id="877da-122">Header</span></span>|<span data-ttu-id="877da-123">值</span><span class="sxs-lookup"><span data-stu-id="877da-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="877da-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="877da-124">Authorization</span></span>|<span data-ttu-id="877da-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="877da-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="877da-126">Accept</span><span class="sxs-lookup"><span data-stu-id="877da-126">Accept</span></span>|<span data-ttu-id="877da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="877da-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="877da-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="877da-128">Request body</span></span>

<span data-ttu-id="877da-129">在请求正文中，提供 windowsDomainJoinConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="877da-129">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="877da-130">下表显示时创建 windowsDomainJoinConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="877da-130">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="877da-131">属性</span><span class="sxs-lookup"><span data-stu-id="877da-131">Property</span></span>|<span data-ttu-id="877da-132">类型</span><span class="sxs-lookup"><span data-stu-id="877da-132">Type</span></span>|<span data-ttu-id="877da-133">说明</span><span class="sxs-lookup"><span data-stu-id="877da-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="877da-134">id</span><span class="sxs-lookup"><span data-stu-id="877da-134">id</span></span>|<span data-ttu-id="877da-135">String</span><span class="sxs-lookup"><span data-stu-id="877da-135">String</span></span>|<span data-ttu-id="877da-136">实体的键。</span><span class="sxs-lookup"><span data-stu-id="877da-136">Key of the entity.</span></span> <span data-ttu-id="877da-137">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="877da-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="877da-138">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="877da-138">**Device configuration**</span></span>|
|<span data-ttu-id="877da-139">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="877da-139">activeDirectoryDomainName</span></span>|<span data-ttu-id="877da-140">字符串</span><span class="sxs-lookup"><span data-stu-id="877da-140">String</span></span>|<span data-ttu-id="877da-141">Active Directory 域名加入。</span><span class="sxs-lookup"><span data-stu-id="877da-141">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="877da-142">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="877da-142">computerNameStaticPrefix</span></span>|<span data-ttu-id="877da-143">字符串</span><span class="sxs-lookup"><span data-stu-id="877da-143">String</span></span>|<span data-ttu-id="877da-144">固定的前缀用于计算机名称。</span><span class="sxs-lookup"><span data-stu-id="877da-144">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="877da-145">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="877da-145">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="877da-146">Int32</span><span class="sxs-lookup"><span data-stu-id="877da-146">Int32</span></span>|<span data-ttu-id="877da-147">动态生成的计算机名称用作后缀的字符。</span><span class="sxs-lookup"><span data-stu-id="877da-147">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="877da-148">有效值 3 到 14</span><span class="sxs-lookup"><span data-stu-id="877da-148">Valid values 3 to 14</span></span>|
|<span data-ttu-id="877da-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="877da-149">createdDateTime</span></span>|<span data-ttu-id="877da-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="877da-150">DateTimeOffset</span></span>|<span data-ttu-id="877da-151">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="877da-151">DateTime the object was created.</span></span> <span data-ttu-id="877da-152">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="877da-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="877da-153">description</span><span class="sxs-lookup"><span data-stu-id="877da-153">description</span></span>|<span data-ttu-id="877da-154">String</span><span class="sxs-lookup"><span data-stu-id="877da-154">String</span></span>|<span data-ttu-id="877da-155">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="877da-155">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="877da-156">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="877da-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="877da-157">displayName</span><span class="sxs-lookup"><span data-stu-id="877da-157">displayName</span></span>|<span data-ttu-id="877da-158">String</span><span class="sxs-lookup"><span data-stu-id="877da-158">String</span></span>|<span data-ttu-id="877da-159">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="877da-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="877da-160">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="877da-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="877da-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="877da-161">lastModifiedDateTime</span></span>|<span data-ttu-id="877da-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="877da-162">DateTimeOffset</span></span>|<span data-ttu-id="877da-163">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="877da-163">DateTime the object was last modified.</span></span> <span data-ttu-id="877da-164">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="877da-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="877da-165">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="877da-165">organizationalUnit</span></span>|<span data-ttu-id="877da-166">字符串</span><span class="sxs-lookup"><span data-stu-id="877da-166">String</span></span>|<span data-ttu-id="877da-167">将在其中创建计算机帐户组织单位 (OU)。</span><span class="sxs-lookup"><span data-stu-id="877da-167">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="877da-168">如果此参数为 NULL，则将发布域中使用已知的计算机对象容器。</span><span class="sxs-lookup"><span data-stu-id="877da-168">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="877da-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="877da-169">roleScopeTagIds</span></span>|<span data-ttu-id="877da-170">String 集合</span><span class="sxs-lookup"><span data-stu-id="877da-170">String collection</span></span>|<span data-ttu-id="877da-171">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="877da-171">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="877da-172">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="877da-172">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="877da-173">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="877da-173">supportsScopeTags</span></span>|<span data-ttu-id="877da-174">布尔</span><span class="sxs-lookup"><span data-stu-id="877da-174">Boolean</span></span>|<span data-ttu-id="877da-175">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="877da-175">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="877da-176">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="877da-176">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="877da-177">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="877da-177">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="877da-178">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="877da-178">This property is read-only.</span></span> <span data-ttu-id="877da-179">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="877da-179">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="877da-180">version</span><span class="sxs-lookup"><span data-stu-id="877da-180">version</span></span>|<span data-ttu-id="877da-181">Int32</span><span class="sxs-lookup"><span data-stu-id="877da-181">Int32</span></span>|<span data-ttu-id="877da-182">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="877da-182">Version of the device configuration.</span></span> <span data-ttu-id="877da-183">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="877da-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="877da-184">响应</span><span class="sxs-lookup"><span data-stu-id="877da-184">Response</span></span>

<span data-ttu-id="877da-185">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="877da-185">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="877da-186">示例</span><span class="sxs-lookup"><span data-stu-id="877da-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="877da-187">请求</span><span class="sxs-lookup"><span data-stu-id="877da-187">Request</span></span>

<span data-ttu-id="877da-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="877da-188">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 559

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```

### <a name="response"></a><span data-ttu-id="877da-189">响应</span><span class="sxs-lookup"><span data-stu-id="877da-189">Response</span></span>

<span data-ttu-id="877da-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="877da-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
  "id": "40118d08-8d08-4011-088d-1140088d1140",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "computerNameStaticPrefix": "Computer Name Static Prefix value",
  "computerNameSuffixRandomCharCount": 1,
  "activeDirectoryDomainName": "Active Directory Domain Name value",
  "organizationalUnit": "Organizational Unit value"
}
```



