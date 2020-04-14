---
title: 创建 windowsDomainJoinConfiguration
description: 创建新的 windowsDomainJoinConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 97d760b9e5dd34038a70cea14294fa4a27e55a3b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447355"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="d5d36-103">创建 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5d36-103">Create windowsDomainJoinConfiguration</span></span>

<span data-ttu-id="d5d36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5d36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5d36-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d5d36-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5d36-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d5d36-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5d36-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5d36-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5d36-108">创建新的[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5d36-108">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5d36-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5d36-109">Prerequisites</span></span>
<span data-ttu-id="d5d36-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5d36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5d36-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5d36-112">Permission type</span></span>|<span data-ttu-id="d5d36-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5d36-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5d36-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5d36-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d5d36-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="d5d36-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d5d36-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d36-116">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="d5d36-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5d36-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5d36-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5d36-118">Not supported.</span></span>|
|<span data-ttu-id="d5d36-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5d36-119">Application</span></span>||
| <span data-ttu-id="d5d36-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="d5d36-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="d5d36-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5d36-121">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5d36-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5d36-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d5d36-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5d36-123">Request headers</span></span>

|<span data-ttu-id="d5d36-124">标头</span><span class="sxs-lookup"><span data-stu-id="d5d36-124">Header</span></span>|<span data-ttu-id="d5d36-125">值</span><span class="sxs-lookup"><span data-stu-id="d5d36-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5d36-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5d36-126">Authorization</span></span>|<span data-ttu-id="d5d36-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5d36-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5d36-128">接受</span><span class="sxs-lookup"><span data-stu-id="d5d36-128">Accept</span></span>|<span data-ttu-id="d5d36-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d5d36-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5d36-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5d36-130">Request body</span></span>

<span data-ttu-id="d5d36-131">在请求正文中，提供 windowsDomainJoinConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5d36-131">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="d5d36-132">下表显示创建 windowsDomainJoinConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d5d36-132">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="d5d36-133">属性</span><span class="sxs-lookup"><span data-stu-id="d5d36-133">Property</span></span>|<span data-ttu-id="d5d36-134">类型</span><span class="sxs-lookup"><span data-stu-id="d5d36-134">Type</span></span>|<span data-ttu-id="d5d36-135">说明</span><span class="sxs-lookup"><span data-stu-id="d5d36-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5d36-136">id</span><span class="sxs-lookup"><span data-stu-id="d5d36-136">id</span></span>|<span data-ttu-id="d5d36-137">字符串</span><span class="sxs-lookup"><span data-stu-id="d5d36-137">String</span></span>|<span data-ttu-id="d5d36-138">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d5d36-138">Key of the entity.</span></span> <span data-ttu-id="d5d36-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5d36-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d36-140">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="d5d36-140">**Device configuration**</span></span>|
|<span data-ttu-id="d5d36-141">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="d5d36-141">activeDirectoryDomainName</span></span>|<span data-ttu-id="d5d36-142">String</span><span class="sxs-lookup"><span data-stu-id="d5d36-142">String</span></span>|<span data-ttu-id="d5d36-143">要加入的 Active Directory 域名称。</span><span class="sxs-lookup"><span data-stu-id="d5d36-143">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="d5d36-144">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="d5d36-144">computerNameStaticPrefix</span></span>|<span data-ttu-id="d5d36-145">String</span><span class="sxs-lookup"><span data-stu-id="d5d36-145">String</span></span>|<span data-ttu-id="d5d36-146">要用于计算机名称的固定前缀。</span><span class="sxs-lookup"><span data-stu-id="d5d36-146">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="d5d36-147">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="d5d36-147">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="d5d36-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d5d36-148">Int32</span></span>|<span data-ttu-id="d5d36-149">作为计算机名称的后缀使用的动态生成字符。</span><span class="sxs-lookup"><span data-stu-id="d5d36-149">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="d5d36-150">有效的值3至14</span><span class="sxs-lookup"><span data-stu-id="d5d36-150">Valid values 3 to 14</span></span>|
|<span data-ttu-id="d5d36-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5d36-151">createdDateTime</span></span>|<span data-ttu-id="d5d36-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5d36-152">DateTimeOffset</span></span>|<span data-ttu-id="d5d36-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d5d36-153">DateTime the object was created.</span></span> <span data-ttu-id="d5d36-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5d36-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d36-155">description</span><span class="sxs-lookup"><span data-stu-id="d5d36-155">description</span></span>|<span data-ttu-id="d5d36-156">String</span><span class="sxs-lookup"><span data-stu-id="d5d36-156">String</span></span>|<span data-ttu-id="d5d36-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d5d36-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5d36-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5d36-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d36-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d5d36-159">displayName</span></span>|<span data-ttu-id="d5d36-160">String</span><span class="sxs-lookup"><span data-stu-id="d5d36-160">String</span></span>|<span data-ttu-id="d5d36-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d5d36-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5d36-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5d36-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d36-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5d36-163">lastModifiedDateTime</span></span>|<span data-ttu-id="d5d36-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5d36-164">DateTimeOffset</span></span>|<span data-ttu-id="d5d36-165">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d5d36-165">DateTime the object was last modified.</span></span> <span data-ttu-id="d5d36-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5d36-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d36-167">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="d5d36-167">organizationalUnit</span></span>|<span data-ttu-id="d5d36-168">String</span><span class="sxs-lookup"><span data-stu-id="d5d36-168">String</span></span>|<span data-ttu-id="d5d36-169">将在其中创建计算机帐户的组织单位（OU）。</span><span class="sxs-lookup"><span data-stu-id="d5d36-169">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="d5d36-170">如果此参数为 NULL，则已知的计算机对象容器将被用作域中的已发布。</span><span class="sxs-lookup"><span data-stu-id="d5d36-170">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="d5d36-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5d36-171">roleScopeTagIds</span></span>|<span data-ttu-id="d5d36-172">String 集合</span><span class="sxs-lookup"><span data-stu-id="d5d36-172">String collection</span></span>|<span data-ttu-id="d5d36-173">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d5d36-173">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d5d36-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5d36-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d36-175">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d5d36-175">supportsScopeTags</span></span>|<span data-ttu-id="d5d36-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5d36-176">Boolean</span></span>|<span data-ttu-id="d5d36-177">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d5d36-177">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d5d36-178">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d5d36-178">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d5d36-179">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d5d36-179">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d5d36-180">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d5d36-180">This property is read-only.</span></span> <span data-ttu-id="d5d36-181">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5d36-181">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5d36-182">version</span><span class="sxs-lookup"><span data-stu-id="d5d36-182">version</span></span>|<span data-ttu-id="d5d36-183">Int32</span><span class="sxs-lookup"><span data-stu-id="d5d36-183">Int32</span></span>|<span data-ttu-id="d5d36-184">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d5d36-184">Version of the device configuration.</span></span> <span data-ttu-id="d5d36-185">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5d36-185">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d5d36-186">响应</span><span class="sxs-lookup"><span data-stu-id="d5d36-186">Response</span></span>

<span data-ttu-id="d5d36-187">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d5d36-187">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5d36-188">示例</span><span class="sxs-lookup"><span data-stu-id="d5d36-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5d36-189">请求</span><span class="sxs-lookup"><span data-stu-id="d5d36-189">Request</span></span>

<span data-ttu-id="d5d36-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5d36-190">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="d5d36-191">响应</span><span class="sxs-lookup"><span data-stu-id="d5d36-191">Response</span></span>

<span data-ttu-id="d5d36-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5d36-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









