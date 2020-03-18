---
title: 创建 windowsDomainJoinConfiguration
description: 创建新的 windowsDomainJoinConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a083f270d43cf5863fb97345af830865434ad0c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800478"
---
# <a name="create-windowsdomainjoinconfiguration"></a><span data-ttu-id="f7e16-103">创建 windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7e16-103">Create windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="f7e16-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f7e16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f7e16-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f7e16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7e16-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7e16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7e16-107">创建新的[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7e16-107">Create a new [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7e16-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7e16-108">Prerequisites</span></span>
<span data-ttu-id="f7e16-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7e16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e16-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7e16-111">Permission type</span></span>|<span data-ttu-id="f7e16-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7e16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7e16-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e16-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f7e16-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="f7e16-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f7e16-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e16-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="f7e16-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e16-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7e16-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7e16-117">Not supported.</span></span>|
|<span data-ttu-id="f7e16-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7e16-118">Application</span></span>||
| <span data-ttu-id="f7e16-119">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="f7e16-119">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="f7e16-120">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e16-120">DeviceManagementConfiguration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7e16-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7e16-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f7e16-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7e16-122">Request headers</span></span>

|<span data-ttu-id="f7e16-123">标头</span><span class="sxs-lookup"><span data-stu-id="f7e16-123">Header</span></span>|<span data-ttu-id="f7e16-124">值</span><span class="sxs-lookup"><span data-stu-id="f7e16-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7e16-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7e16-125">Authorization</span></span>|<span data-ttu-id="f7e16-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7e16-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7e16-127">接受</span><span class="sxs-lookup"><span data-stu-id="f7e16-127">Accept</span></span>|<span data-ttu-id="f7e16-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f7e16-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7e16-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7e16-129">Request body</span></span>

<span data-ttu-id="f7e16-130">在请求正文中，提供 windowsDomainJoinConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7e16-130">In the request body, supply a JSON representation for the windowsDomainJoinConfiguration object.</span></span>

<span data-ttu-id="f7e16-131">下表显示创建 windowsDomainJoinConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f7e16-131">The following table shows the properties that are required when you create the windowsDomainJoinConfiguration.</span></span>

|<span data-ttu-id="f7e16-132">属性</span><span class="sxs-lookup"><span data-stu-id="f7e16-132">Property</span></span>|<span data-ttu-id="f7e16-133">类型</span><span class="sxs-lookup"><span data-stu-id="f7e16-133">Type</span></span>|<span data-ttu-id="f7e16-134">说明</span><span class="sxs-lookup"><span data-stu-id="f7e16-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7e16-135">id</span><span class="sxs-lookup"><span data-stu-id="f7e16-135">id</span></span>|<span data-ttu-id="f7e16-136">字符串</span><span class="sxs-lookup"><span data-stu-id="f7e16-136">String</span></span>|<span data-ttu-id="f7e16-137">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f7e16-137">Key of the entity.</span></span> <span data-ttu-id="f7e16-138">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7e16-138">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7e16-139">**设备配置**</span><span class="sxs-lookup"><span data-stu-id="f7e16-139">**Device configuration**</span></span>|
|<span data-ttu-id="f7e16-140">activeDirectoryDomainName</span><span class="sxs-lookup"><span data-stu-id="f7e16-140">activeDirectoryDomainName</span></span>|<span data-ttu-id="f7e16-141">String</span><span class="sxs-lookup"><span data-stu-id="f7e16-141">String</span></span>|<span data-ttu-id="f7e16-142">要加入的 Active Directory 域名称。</span><span class="sxs-lookup"><span data-stu-id="f7e16-142">Active Directory domain name to join.</span></span>|
|<span data-ttu-id="f7e16-143">computerNameStaticPrefix</span><span class="sxs-lookup"><span data-stu-id="f7e16-143">computerNameStaticPrefix</span></span>|<span data-ttu-id="f7e16-144">String</span><span class="sxs-lookup"><span data-stu-id="f7e16-144">String</span></span>|<span data-ttu-id="f7e16-145">要用于计算机名称的固定前缀。</span><span class="sxs-lookup"><span data-stu-id="f7e16-145">Fixed prefix to be used for computer name.</span></span>|
|<span data-ttu-id="f7e16-146">computerNameSuffixRandomCharCount</span><span class="sxs-lookup"><span data-stu-id="f7e16-146">computerNameSuffixRandomCharCount</span></span>|<span data-ttu-id="f7e16-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f7e16-147">Int32</span></span>|<span data-ttu-id="f7e16-148">作为计算机名称的后缀使用的动态生成字符。</span><span class="sxs-lookup"><span data-stu-id="f7e16-148">Dynamically generated characters used as suffix for computer name.</span></span> <span data-ttu-id="f7e16-149">有效的值3至14</span><span class="sxs-lookup"><span data-stu-id="f7e16-149">Valid values 3 to 14</span></span>|
|<span data-ttu-id="f7e16-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7e16-150">createdDateTime</span></span>|<span data-ttu-id="f7e16-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7e16-151">DateTimeOffset</span></span>|<span data-ttu-id="f7e16-152">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f7e16-152">DateTime the object was created.</span></span> <span data-ttu-id="f7e16-153">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7e16-153">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7e16-154">说明</span><span class="sxs-lookup"><span data-stu-id="f7e16-154">description</span></span>|<span data-ttu-id="f7e16-155">String</span><span class="sxs-lookup"><span data-stu-id="f7e16-155">String</span></span>|<span data-ttu-id="f7e16-156">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f7e16-156">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f7e16-157">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7e16-157">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7e16-158">displayName</span><span class="sxs-lookup"><span data-stu-id="f7e16-158">displayName</span></span>|<span data-ttu-id="f7e16-159">String</span><span class="sxs-lookup"><span data-stu-id="f7e16-159">String</span></span>|<span data-ttu-id="f7e16-160">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f7e16-160">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f7e16-161">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7e16-161">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7e16-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7e16-162">lastModifiedDateTime</span></span>|<span data-ttu-id="f7e16-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7e16-163">DateTimeOffset</span></span>|<span data-ttu-id="f7e16-164">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f7e16-164">DateTime the object was last modified.</span></span> <span data-ttu-id="f7e16-165">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7e16-165">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7e16-166">organizationalUnit</span><span class="sxs-lookup"><span data-stu-id="f7e16-166">organizationalUnit</span></span>|<span data-ttu-id="f7e16-167">String</span><span class="sxs-lookup"><span data-stu-id="f7e16-167">String</span></span>|<span data-ttu-id="f7e16-168">将在其中创建计算机帐户的组织单位（OU）。</span><span class="sxs-lookup"><span data-stu-id="f7e16-168">Organizational unit (OU) where the computer account will be created.</span></span> <span data-ttu-id="f7e16-169">如果此参数为 NULL，则已知的计算机对象容器将被用作域中的已发布。</span><span class="sxs-lookup"><span data-stu-id="f7e16-169">If this parameter is NULL, the well known computer object container will be used as published in the domain.</span></span>|
|<span data-ttu-id="f7e16-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f7e16-170">roleScopeTagIds</span></span>|<span data-ttu-id="f7e16-171">String collection</span><span class="sxs-lookup"><span data-stu-id="f7e16-171">String collection</span></span>|<span data-ttu-id="f7e16-172">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f7e16-172">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f7e16-173">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7e16-173">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7e16-174">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f7e16-174">supportsScopeTags</span></span>|<span data-ttu-id="f7e16-175">布尔值</span><span class="sxs-lookup"><span data-stu-id="f7e16-175">Boolean</span></span>|<span data-ttu-id="f7e16-176">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f7e16-176">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f7e16-177">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f7e16-177">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f7e16-178">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f7e16-178">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f7e16-179">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f7e16-179">This property is read-only.</span></span> <span data-ttu-id="f7e16-180">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7e16-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7e16-181">version</span><span class="sxs-lookup"><span data-stu-id="f7e16-181">version</span></span>|<span data-ttu-id="f7e16-182">Int32</span><span class="sxs-lookup"><span data-stu-id="f7e16-182">Int32</span></span>|<span data-ttu-id="f7e16-183">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f7e16-183">Version of the device configuration.</span></span> <span data-ttu-id="f7e16-184">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7e16-184">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f7e16-185">响应</span><span class="sxs-lookup"><span data-stu-id="f7e16-185">Response</span></span>

<span data-ttu-id="f7e16-186">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7e16-186">If successful, this method returns a `201 Created` response code and a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e16-187">示例</span><span class="sxs-lookup"><span data-stu-id="f7e16-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7e16-188">请求</span><span class="sxs-lookup"><span data-stu-id="f7e16-188">Request</span></span>

<span data-ttu-id="f7e16-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7e16-189">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="f7e16-190">响应</span><span class="sxs-lookup"><span data-stu-id="f7e16-190">Response</span></span>

<span data-ttu-id="f7e16-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7e16-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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










