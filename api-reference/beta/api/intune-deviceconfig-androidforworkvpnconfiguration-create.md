---
title: 创建 androidForWorkVpnConfiguration
description: 创建新的 androidForWorkVpnConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 307585ae70d79de01e1b9c34584e91121e6763ae
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33932808"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="759d4-103">创建 androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="759d4-103">Create androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="759d4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="759d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="759d4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="759d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="759d4-106">创建新的[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="759d4-106">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="759d4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="759d4-107">Prerequisites</span></span>
<span data-ttu-id="759d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="759d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="759d4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="759d4-110">Permission type</span></span>|<span data-ttu-id="759d4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="759d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="759d4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="759d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="759d4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="759d4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="759d4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="759d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="759d4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="759d4-115">Not supported.</span></span>|
|<span data-ttu-id="759d4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="759d4-116">Application</span></span>|<span data-ttu-id="759d4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="759d4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="759d4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="759d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="759d4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="759d4-119">Request headers</span></span>
|<span data-ttu-id="759d4-120">标头</span><span class="sxs-lookup"><span data-stu-id="759d4-120">Header</span></span>|<span data-ttu-id="759d4-121">值</span><span class="sxs-lookup"><span data-stu-id="759d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="759d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="759d4-122">Authorization</span></span>|<span data-ttu-id="759d4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="759d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="759d4-124">接受</span><span class="sxs-lookup"><span data-stu-id="759d4-124">Accept</span></span>|<span data-ttu-id="759d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="759d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="759d4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="759d4-126">Request body</span></span>
<span data-ttu-id="759d4-127">在请求正文中, 提供 androidForWorkVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="759d4-127">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="759d4-128">下表显示创建 androidForWorkVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="759d4-128">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="759d4-129">属性</span><span class="sxs-lookup"><span data-stu-id="759d4-129">Property</span></span>|<span data-ttu-id="759d4-130">类型</span><span class="sxs-lookup"><span data-stu-id="759d4-130">Type</span></span>|<span data-ttu-id="759d4-131">说明</span><span class="sxs-lookup"><span data-stu-id="759d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="759d4-132">id</span><span class="sxs-lookup"><span data-stu-id="759d4-132">id</span></span>|<span data-ttu-id="759d4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="759d4-133">String</span></span>|<span data-ttu-id="759d4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="759d4-134">Key of the entity.</span></span> <span data-ttu-id="759d4-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="759d4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="759d4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="759d4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="759d4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="759d4-137">DateTimeOffset</span></span>|<span data-ttu-id="759d4-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="759d4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="759d4-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="759d4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="759d4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="759d4-140">roleScopeTagIds</span></span>|<span data-ttu-id="759d4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="759d4-141">String collection</span></span>|<span data-ttu-id="759d4-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="759d4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="759d4-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="759d4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="759d4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="759d4-144">supportsScopeTags</span></span>|<span data-ttu-id="759d4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="759d4-145">Boolean</span></span>|<span data-ttu-id="759d4-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="759d4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="759d4-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="759d4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="759d4-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="759d4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="759d4-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="759d4-149">This property is read-only.</span></span> <span data-ttu-id="759d4-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="759d4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="759d4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="759d4-151">createdDateTime</span></span>|<span data-ttu-id="759d4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="759d4-152">DateTimeOffset</span></span>|<span data-ttu-id="759d4-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="759d4-153">DateTime the object was created.</span></span> <span data-ttu-id="759d4-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="759d4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="759d4-155">说明</span><span class="sxs-lookup"><span data-stu-id="759d4-155">description</span></span>|<span data-ttu-id="759d4-156">String</span><span class="sxs-lookup"><span data-stu-id="759d4-156">String</span></span>|<span data-ttu-id="759d4-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="759d4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="759d4-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="759d4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="759d4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="759d4-159">displayName</span></span>|<span data-ttu-id="759d4-160">String</span><span class="sxs-lookup"><span data-stu-id="759d4-160">String</span></span>|<span data-ttu-id="759d4-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="759d4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="759d4-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="759d4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="759d4-163">version</span><span class="sxs-lookup"><span data-stu-id="759d4-163">version</span></span>|<span data-ttu-id="759d4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="759d4-164">Int32</span></span>|<span data-ttu-id="759d4-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="759d4-165">Version of the device configuration.</span></span> <span data-ttu-id="759d4-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="759d4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="759d4-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="759d4-167">connectionName</span></span>|<span data-ttu-id="759d4-168">String</span><span class="sxs-lookup"><span data-stu-id="759d4-168">String</span></span>|<span data-ttu-id="759d4-169">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="759d4-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="759d4-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="759d4-170">connectionType</span></span>|[<span data-ttu-id="759d4-171">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="759d4-171">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="759d4-172">连接类型。</span><span class="sxs-lookup"><span data-stu-id="759d4-172">Connection type.</span></span> <span data-ttu-id="759d4-173">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="759d4-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="759d4-174">role</span><span class="sxs-lookup"><span data-stu-id="759d4-174">role</span></span>|<span data-ttu-id="759d4-175">String</span><span class="sxs-lookup"><span data-stu-id="759d4-175">String</span></span>|<span data-ttu-id="759d4-176">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="759d4-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="759d4-177">型</span><span class="sxs-lookup"><span data-stu-id="759d4-177">realm</span></span>|<span data-ttu-id="759d4-178">String</span><span class="sxs-lookup"><span data-stu-id="759d4-178">String</span></span>|<span data-ttu-id="759d4-179">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="759d4-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="759d4-180">台</span><span class="sxs-lookup"><span data-stu-id="759d4-180">servers</span></span>|<span data-ttu-id="759d4-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="759d4-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="759d4-182">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="759d4-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="759d4-183">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="759d4-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="759d4-184">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="759d4-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="759d4-185">其次</span><span class="sxs-lookup"><span data-stu-id="759d4-185">fingerprint</span></span>|<span data-ttu-id="759d4-186">String</span><span class="sxs-lookup"><span data-stu-id="759d4-186">String</span></span>|<span data-ttu-id="759d4-187">指纹是一个字符串, 用于验证 VPN 服务器是否可以信任, 这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="759d4-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="759d4-188">customData</span><span class="sxs-lookup"><span data-stu-id="759d4-188">customData</span></span>|<span data-ttu-id="759d4-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="759d4-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="759d4-190">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="759d4-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="759d4-191">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="759d4-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="759d4-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="759d4-192">customKeyValueData</span></span>|<span data-ttu-id="759d4-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="759d4-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="759d4-194">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="759d4-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="759d4-195">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="759d4-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="759d4-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="759d4-196">authenticationMethod</span></span>|[<span data-ttu-id="759d4-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="759d4-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="759d4-198">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="759d4-198">Authentication method.</span></span> <span data-ttu-id="759d4-199">可取值为：`certificate`、`usernameAndPassword`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="759d4-199">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="759d4-200">响应</span><span class="sxs-lookup"><span data-stu-id="759d4-200">Response</span></span>
<span data-ttu-id="759d4-201">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="759d4-201">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="759d4-202">示例</span><span class="sxs-lookup"><span data-stu-id="759d4-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="759d4-203">请求</span><span class="sxs-lookup"><span data-stu-id="759d4-203">Request</span></span>
<span data-ttu-id="759d4-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="759d4-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 985

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="759d4-205">响应</span><span class="sxs-lookup"><span data-stu-id="759d4-205">Response</span></span>
<span data-ttu-id="759d4-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="759d4-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1157

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```




