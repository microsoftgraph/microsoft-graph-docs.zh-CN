---
title: 创建 androidForWorkVpnConfiguration
description: 创建新的 androidForWorkVpnConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0e1e6b8bc7374ae6218434dc7b00d7bcd8b8d5c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812710"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="298d1-103">创建 androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="298d1-103">Create androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="298d1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="298d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="298d1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="298d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="298d1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="298d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="298d1-107">创建新的[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="298d1-107">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="298d1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="298d1-108">Prerequisites</span></span>
<span data-ttu-id="298d1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="298d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="298d1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="298d1-111">Permission type</span></span>|<span data-ttu-id="298d1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="298d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="298d1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="298d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="298d1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="298d1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="298d1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="298d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="298d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="298d1-116">Not supported.</span></span>|
|<span data-ttu-id="298d1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="298d1-117">Application</span></span>|<span data-ttu-id="298d1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="298d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="298d1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="298d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="298d1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="298d1-120">Request headers</span></span>
|<span data-ttu-id="298d1-121">标头</span><span class="sxs-lookup"><span data-stu-id="298d1-121">Header</span></span>|<span data-ttu-id="298d1-122">值</span><span class="sxs-lookup"><span data-stu-id="298d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="298d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="298d1-123">Authorization</span></span>|<span data-ttu-id="298d1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="298d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="298d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="298d1-125">Accept</span></span>|<span data-ttu-id="298d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="298d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="298d1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="298d1-127">Request body</span></span>
<span data-ttu-id="298d1-128">在请求正文中，提供 androidForWorkVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="298d1-128">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="298d1-129">下表显示时创建 androidForWorkVpnConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="298d1-129">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="298d1-130">属性</span><span class="sxs-lookup"><span data-stu-id="298d1-130">Property</span></span>|<span data-ttu-id="298d1-131">类型</span><span class="sxs-lookup"><span data-stu-id="298d1-131">Type</span></span>|<span data-ttu-id="298d1-132">说明</span><span class="sxs-lookup"><span data-stu-id="298d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="298d1-133">id</span><span class="sxs-lookup"><span data-stu-id="298d1-133">id</span></span>|<span data-ttu-id="298d1-134">String</span><span class="sxs-lookup"><span data-stu-id="298d1-134">String</span></span>|<span data-ttu-id="298d1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="298d1-135">Key of the entity.</span></span> <span data-ttu-id="298d1-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="298d1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="298d1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="298d1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="298d1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="298d1-138">DateTimeOffset</span></span>|<span data-ttu-id="298d1-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="298d1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="298d1-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="298d1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="298d1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="298d1-141">roleScopeTagIds</span></span>|<span data-ttu-id="298d1-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="298d1-142">String collection</span></span>|<span data-ttu-id="298d1-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="298d1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="298d1-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="298d1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="298d1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="298d1-145">supportsScopeTags</span></span>|<span data-ttu-id="298d1-146">布尔</span><span class="sxs-lookup"><span data-stu-id="298d1-146">Boolean</span></span>|<span data-ttu-id="298d1-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="298d1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="298d1-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="298d1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="298d1-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="298d1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="298d1-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="298d1-150">This property is read-only.</span></span> <span data-ttu-id="298d1-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="298d1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="298d1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="298d1-152">createdDateTime</span></span>|<span data-ttu-id="298d1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="298d1-153">DateTimeOffset</span></span>|<span data-ttu-id="298d1-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="298d1-154">DateTime the object was created.</span></span> <span data-ttu-id="298d1-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="298d1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="298d1-156">description</span><span class="sxs-lookup"><span data-stu-id="298d1-156">description</span></span>|<span data-ttu-id="298d1-157">String</span><span class="sxs-lookup"><span data-stu-id="298d1-157">String</span></span>|<span data-ttu-id="298d1-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="298d1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="298d1-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="298d1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="298d1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="298d1-160">displayName</span></span>|<span data-ttu-id="298d1-161">String</span><span class="sxs-lookup"><span data-stu-id="298d1-161">String</span></span>|<span data-ttu-id="298d1-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="298d1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="298d1-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="298d1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="298d1-164">version</span><span class="sxs-lookup"><span data-stu-id="298d1-164">version</span></span>|<span data-ttu-id="298d1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="298d1-165">Int32</span></span>|<span data-ttu-id="298d1-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="298d1-166">Version of the device configuration.</span></span> <span data-ttu-id="298d1-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="298d1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="298d1-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="298d1-168">connectionName</span></span>|<span data-ttu-id="298d1-169">字符串</span><span class="sxs-lookup"><span data-stu-id="298d1-169">String</span></span>|<span data-ttu-id="298d1-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="298d1-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="298d1-171">连接</span><span class="sxs-lookup"><span data-stu-id="298d1-171">connectionType</span></span>|[<span data-ttu-id="298d1-172">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="298d1-172">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="298d1-173">连接类型。</span><span class="sxs-lookup"><span data-stu-id="298d1-173">Connection type.</span></span> <span data-ttu-id="298d1-174">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="298d1-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="298d1-175">role</span><span class="sxs-lookup"><span data-stu-id="298d1-175">role</span></span>|<span data-ttu-id="298d1-176">字符串</span><span class="sxs-lookup"><span data-stu-id="298d1-176">String</span></span>|<span data-ttu-id="298d1-177">当连接类型设置为脉冲安全角色。</span><span class="sxs-lookup"><span data-stu-id="298d1-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="298d1-178">领域</span><span class="sxs-lookup"><span data-stu-id="298d1-178">realm</span></span>|<span data-ttu-id="298d1-179">字符串</span><span class="sxs-lookup"><span data-stu-id="298d1-179">String</span></span>|<span data-ttu-id="298d1-180">当连接类型设置为脉冲安全领域。</span><span class="sxs-lookup"><span data-stu-id="298d1-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="298d1-181">服务器</span><span class="sxs-lookup"><span data-stu-id="298d1-181">servers</span></span>|<span data-ttu-id="298d1-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="298d1-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="298d1-183">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="298d1-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="298d1-184">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="298d1-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="298d1-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="298d1-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="298d1-186">指纹</span><span class="sxs-lookup"><span data-stu-id="298d1-186">fingerprint</span></span>|<span data-ttu-id="298d1-187">字符串</span><span class="sxs-lookup"><span data-stu-id="298d1-187">String</span></span>|<span data-ttu-id="298d1-188">指纹是一个字符串，用于验证 VPN 服务器可以被信任，检查点胶囊 VPN 连接类型时，这是仅适用。</span><span class="sxs-lookup"><span data-stu-id="298d1-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="298d1-189">customData</span><span class="sxs-lookup"><span data-stu-id="298d1-189">customData</span></span>|<span data-ttu-id="298d1-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="298d1-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="298d1-191">自定义数据连接类型设置为 Citrix 时。</span><span class="sxs-lookup"><span data-stu-id="298d1-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="298d1-192">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="298d1-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="298d1-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="298d1-193">customKeyValueData</span></span>|<span data-ttu-id="298d1-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="298d1-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="298d1-195">自定义数据连接类型设置为 Citrix 时。</span><span class="sxs-lookup"><span data-stu-id="298d1-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="298d1-196">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="298d1-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="298d1-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="298d1-197">authenticationMethod</span></span>|[<span data-ttu-id="298d1-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="298d1-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="298d1-199">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="298d1-199">Authentication method.</span></span> <span data-ttu-id="298d1-200">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="298d1-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="298d1-201">响应</span><span class="sxs-lookup"><span data-stu-id="298d1-201">Response</span></span>
<span data-ttu-id="298d1-202">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="298d1-202">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="298d1-203">示例</span><span class="sxs-lookup"><span data-stu-id="298d1-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="298d1-204">请求</span><span class="sxs-lookup"><span data-stu-id="298d1-204">Request</span></span>
<span data-ttu-id="298d1-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="298d1-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1049

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="298d1-206">响应</span><span class="sxs-lookup"><span data-stu-id="298d1-206">Response</span></span>
<span data-ttu-id="298d1-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="298d1-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





