---
title: 创建 androidWorkProfileVpnConfiguration
description: 创建新的 androidWorkProfileVpnConfiguration 对象。
ms.openlocfilehash: c362b3fd3ff08f8c8ad8a78073439c077daa2de0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045987"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="1c584-103">创建 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c584-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="1c584-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c584-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c584-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c584-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c584-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1c584-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c584-107">创建新的[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c584-107">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c584-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1c584-108">Prerequisites</span></span>
<span data-ttu-id="1c584-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1c584-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c584-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c584-111">Permission type</span></span>|<span data-ttu-id="1c584-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1c584-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c584-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c584-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1c584-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c584-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c584-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c584-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c584-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c584-116">Not supported.</span></span>|
|<span data-ttu-id="1c584-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c584-117">Application</span></span>|<span data-ttu-id="1c584-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c584-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c584-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c584-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c584-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c584-120">Request headers</span></span>
|<span data-ttu-id="1c584-121">标头</span><span class="sxs-lookup"><span data-stu-id="1c584-121">Header</span></span>|<span data-ttu-id="1c584-122">值</span><span class="sxs-lookup"><span data-stu-id="1c584-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c584-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c584-123">Authorization</span></span>|<span data-ttu-id="1c584-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1c584-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c584-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1c584-125">Accept</span></span>|<span data-ttu-id="1c584-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1c584-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c584-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c584-127">Request body</span></span>
<span data-ttu-id="1c584-128">在请求正文中，提供 androidWorkProfileVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c584-128">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="1c584-129">下表显示时创建 androidWorkProfileVpnConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1c584-129">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="1c584-130">属性</span><span class="sxs-lookup"><span data-stu-id="1c584-130">Property</span></span>|<span data-ttu-id="1c584-131">类型</span><span class="sxs-lookup"><span data-stu-id="1c584-131">Type</span></span>|<span data-ttu-id="1c584-132">说明</span><span class="sxs-lookup"><span data-stu-id="1c584-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c584-133">id</span><span class="sxs-lookup"><span data-stu-id="1c584-133">id</span></span>|<span data-ttu-id="1c584-134">String</span><span class="sxs-lookup"><span data-stu-id="1c584-134">String</span></span>|<span data-ttu-id="1c584-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1c584-135">Key of the entity.</span></span> <span data-ttu-id="1c584-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c584-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c584-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c584-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1c584-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c584-138">DateTimeOffset</span></span>|<span data-ttu-id="1c584-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1c584-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1c584-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c584-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c584-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c584-141">roleScopeTagIds</span></span>|<span data-ttu-id="1c584-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1c584-142">String collection</span></span>|<span data-ttu-id="1c584-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="1c584-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c584-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c584-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c584-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1c584-145">supportsScopeTags</span></span>|<span data-ttu-id="1c584-146">布尔</span><span class="sxs-lookup"><span data-stu-id="1c584-146">Boolean</span></span>|<span data-ttu-id="1c584-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="1c584-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1c584-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="1c584-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1c584-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="1c584-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1c584-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1c584-150">This property is read-only.</span></span> <span data-ttu-id="1c584-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c584-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c584-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c584-152">createdDateTime</span></span>|<span data-ttu-id="1c584-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c584-153">DateTimeOffset</span></span>|<span data-ttu-id="1c584-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1c584-154">DateTime the object was created.</span></span> <span data-ttu-id="1c584-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c584-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c584-156">description</span><span class="sxs-lookup"><span data-stu-id="1c584-156">description</span></span>|<span data-ttu-id="1c584-157">String</span><span class="sxs-lookup"><span data-stu-id="1c584-157">String</span></span>|<span data-ttu-id="1c584-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1c584-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c584-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c584-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c584-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1c584-160">displayName</span></span>|<span data-ttu-id="1c584-161">String</span><span class="sxs-lookup"><span data-stu-id="1c584-161">String</span></span>|<span data-ttu-id="1c584-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1c584-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c584-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c584-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c584-164">version</span><span class="sxs-lookup"><span data-stu-id="1c584-164">version</span></span>|<span data-ttu-id="1c584-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1c584-165">Int32</span></span>|<span data-ttu-id="1c584-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1c584-166">Version of the device configuration.</span></span> <span data-ttu-id="1c584-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c584-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c584-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="1c584-168">connectionName</span></span>|<span data-ttu-id="1c584-169">字符串</span><span class="sxs-lookup"><span data-stu-id="1c584-169">String</span></span>|<span data-ttu-id="1c584-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="1c584-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="1c584-171">连接</span><span class="sxs-lookup"><span data-stu-id="1c584-171">connectionType</span></span>|[<span data-ttu-id="1c584-172">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="1c584-172">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="1c584-173">连接类型。</span><span class="sxs-lookup"><span data-stu-id="1c584-173">Connection type.</span></span> <span data-ttu-id="1c584-174">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="1c584-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="1c584-175">role</span><span class="sxs-lookup"><span data-stu-id="1c584-175">role</span></span>|<span data-ttu-id="1c584-176">字符串</span><span class="sxs-lookup"><span data-stu-id="1c584-176">String</span></span>|<span data-ttu-id="1c584-177">当连接类型设置为脉冲安全角色。</span><span class="sxs-lookup"><span data-stu-id="1c584-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="1c584-178">领域</span><span class="sxs-lookup"><span data-stu-id="1c584-178">realm</span></span>|<span data-ttu-id="1c584-179">字符串</span><span class="sxs-lookup"><span data-stu-id="1c584-179">String</span></span>|<span data-ttu-id="1c584-180">当连接类型设置为脉冲安全领域。</span><span class="sxs-lookup"><span data-stu-id="1c584-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="1c584-181">服务器</span><span class="sxs-lookup"><span data-stu-id="1c584-181">servers</span></span>|<span data-ttu-id="1c584-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c584-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1c584-183">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="1c584-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="1c584-184">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="1c584-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1c584-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="1c584-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1c584-186">指纹</span><span class="sxs-lookup"><span data-stu-id="1c584-186">fingerprint</span></span>|<span data-ttu-id="1c584-187">字符串</span><span class="sxs-lookup"><span data-stu-id="1c584-187">String</span></span>|<span data-ttu-id="1c584-188">指纹是一个字符串，用于验证 VPN 服务器可以被信任，检查点胶囊 VPN 连接类型时，这是仅适用。</span><span class="sxs-lookup"><span data-stu-id="1c584-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="1c584-189">customData</span><span class="sxs-lookup"><span data-stu-id="1c584-189">customData</span></span>|<span data-ttu-id="1c584-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c584-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="1c584-191">自定义数据连接类型设置为 Citrix 时。</span><span class="sxs-lookup"><span data-stu-id="1c584-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="1c584-192">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="1c584-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="1c584-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="1c584-193">customKeyValueData</span></span>|<span data-ttu-id="1c584-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1c584-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1c584-195">自定义数据连接类型设置为 Citrix 时。</span><span class="sxs-lookup"><span data-stu-id="1c584-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="1c584-196">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="1c584-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="1c584-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1c584-197">authenticationMethod</span></span>|[<span data-ttu-id="1c584-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1c584-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="1c584-199">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="1c584-199">Authentication method.</span></span> <span data-ttu-id="1c584-200">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="1c584-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="1c584-201">响应</span><span class="sxs-lookup"><span data-stu-id="1c584-201">Response</span></span>
<span data-ttu-id="1c584-202">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c584-202">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c584-203">示例</span><span class="sxs-lookup"><span data-stu-id="1c584-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c584-204">请求</span><span class="sxs-lookup"><span data-stu-id="1c584-204">Request</span></span>
<span data-ttu-id="1c584-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c584-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1053

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="1c584-206">响应</span><span class="sxs-lookup"><span data-stu-id="1c584-206">Response</span></span>
<span data-ttu-id="1c584-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c584-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1161

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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





