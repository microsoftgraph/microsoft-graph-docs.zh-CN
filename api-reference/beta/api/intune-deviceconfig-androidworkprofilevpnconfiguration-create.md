---
title: 创建 androidWorkProfileVpnConfiguration
description: 创建新的 androidWorkProfileVpnConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6cdac06f045af7b5fc60f2debc0b17c7baf6bd2d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399176"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="ce61e-103">创建 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce61e-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="ce61e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ce61e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce61e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ce61e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce61e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce61e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce61e-107">创建新的[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ce61e-107">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce61e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce61e-108">Prerequisites</span></span>
<span data-ttu-id="ce61e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ce61e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ce61e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce61e-111">Permission type</span></span>|<span data-ttu-id="ce61e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ce61e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce61e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce61e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce61e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce61e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce61e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce61e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce61e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce61e-116">Not supported.</span></span>|
|<span data-ttu-id="ce61e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce61e-117">Application</span></span>|<span data-ttu-id="ce61e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce61e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce61e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce61e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ce61e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce61e-120">Request headers</span></span>
|<span data-ttu-id="ce61e-121">标头</span><span class="sxs-lookup"><span data-stu-id="ce61e-121">Header</span></span>|<span data-ttu-id="ce61e-122">值</span><span class="sxs-lookup"><span data-stu-id="ce61e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce61e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce61e-123">Authorization</span></span>|<span data-ttu-id="ce61e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce61e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce61e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce61e-125">Accept</span></span>|<span data-ttu-id="ce61e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce61e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce61e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce61e-127">Request body</span></span>
<span data-ttu-id="ce61e-128">在请求正文中，提供 androidWorkProfileVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce61e-128">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="ce61e-129">下表显示时创建 androidWorkProfileVpnConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ce61e-129">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="ce61e-130">属性</span><span class="sxs-lookup"><span data-stu-id="ce61e-130">Property</span></span>|<span data-ttu-id="ce61e-131">类型</span><span class="sxs-lookup"><span data-stu-id="ce61e-131">Type</span></span>|<span data-ttu-id="ce61e-132">说明</span><span class="sxs-lookup"><span data-stu-id="ce61e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce61e-133">id</span><span class="sxs-lookup"><span data-stu-id="ce61e-133">id</span></span>|<span data-ttu-id="ce61e-134">String</span><span class="sxs-lookup"><span data-stu-id="ce61e-134">String</span></span>|<span data-ttu-id="ce61e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ce61e-135">Key of the entity.</span></span> <span data-ttu-id="ce61e-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce61e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce61e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce61e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ce61e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce61e-138">DateTimeOffset</span></span>|<span data-ttu-id="ce61e-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ce61e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ce61e-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce61e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce61e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce61e-141">roleScopeTagIds</span></span>|<span data-ttu-id="ce61e-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="ce61e-142">String collection</span></span>|<span data-ttu-id="ce61e-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="ce61e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ce61e-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce61e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce61e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ce61e-145">supportsScopeTags</span></span>|<span data-ttu-id="ce61e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce61e-146">Boolean</span></span>|<span data-ttu-id="ce61e-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="ce61e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ce61e-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="ce61e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ce61e-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="ce61e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ce61e-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ce61e-150">This property is read-only.</span></span> <span data-ttu-id="ce61e-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce61e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce61e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce61e-152">createdDateTime</span></span>|<span data-ttu-id="ce61e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce61e-153">DateTimeOffset</span></span>|<span data-ttu-id="ce61e-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ce61e-154">DateTime the object was created.</span></span> <span data-ttu-id="ce61e-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce61e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce61e-156">description</span><span class="sxs-lookup"><span data-stu-id="ce61e-156">description</span></span>|<span data-ttu-id="ce61e-157">String</span><span class="sxs-lookup"><span data-stu-id="ce61e-157">String</span></span>|<span data-ttu-id="ce61e-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ce61e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ce61e-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce61e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce61e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ce61e-160">displayName</span></span>|<span data-ttu-id="ce61e-161">String</span><span class="sxs-lookup"><span data-stu-id="ce61e-161">String</span></span>|<span data-ttu-id="ce61e-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ce61e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ce61e-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce61e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce61e-164">version</span><span class="sxs-lookup"><span data-stu-id="ce61e-164">version</span></span>|<span data-ttu-id="ce61e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ce61e-165">Int32</span></span>|<span data-ttu-id="ce61e-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ce61e-166">Version of the device configuration.</span></span> <span data-ttu-id="ce61e-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ce61e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ce61e-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="ce61e-168">connectionName</span></span>|<span data-ttu-id="ce61e-169">String</span><span class="sxs-lookup"><span data-stu-id="ce61e-169">String</span></span>|<span data-ttu-id="ce61e-170">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="ce61e-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="ce61e-171">连接</span><span class="sxs-lookup"><span data-stu-id="ce61e-171">connectionType</span></span>|[<span data-ttu-id="ce61e-172">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ce61e-172">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="ce61e-173">连接类型。</span><span class="sxs-lookup"><span data-stu-id="ce61e-173">Connection type.</span></span> <span data-ttu-id="ce61e-174">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="ce61e-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="ce61e-175">role</span><span class="sxs-lookup"><span data-stu-id="ce61e-175">role</span></span>|<span data-ttu-id="ce61e-176">String</span><span class="sxs-lookup"><span data-stu-id="ce61e-176">String</span></span>|<span data-ttu-id="ce61e-177">当连接类型设置为脉冲安全角色。</span><span class="sxs-lookup"><span data-stu-id="ce61e-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ce61e-178">领域</span><span class="sxs-lookup"><span data-stu-id="ce61e-178">realm</span></span>|<span data-ttu-id="ce61e-179">String</span><span class="sxs-lookup"><span data-stu-id="ce61e-179">String</span></span>|<span data-ttu-id="ce61e-180">当连接类型设置为脉冲安全领域。</span><span class="sxs-lookup"><span data-stu-id="ce61e-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ce61e-181">服务器</span><span class="sxs-lookup"><span data-stu-id="ce61e-181">servers</span></span>|<span data-ttu-id="ce61e-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="ce61e-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ce61e-183">VPN 服务器的网络上的列表。</span><span class="sxs-lookup"><span data-stu-id="ce61e-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="ce61e-184">确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="ce61e-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ce61e-185">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="ce61e-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ce61e-186">指纹</span><span class="sxs-lookup"><span data-stu-id="ce61e-186">fingerprint</span></span>|<span data-ttu-id="ce61e-187">String</span><span class="sxs-lookup"><span data-stu-id="ce61e-187">String</span></span>|<span data-ttu-id="ce61e-188">指纹是一个字符串，用于验证 VPN 服务器可以被信任，检查点胶囊 VPN 连接类型时，这是仅适用。</span><span class="sxs-lookup"><span data-stu-id="ce61e-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ce61e-189">customData</span><span class="sxs-lookup"><span data-stu-id="ce61e-189">customData</span></span>|<span data-ttu-id="ce61e-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="ce61e-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ce61e-191">自定义数据连接类型设置为 Citrix 时。</span><span class="sxs-lookup"><span data-stu-id="ce61e-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ce61e-192">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="ce61e-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ce61e-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ce61e-193">customKeyValueData</span></span>|<span data-ttu-id="ce61e-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ce61e-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ce61e-195">自定义数据连接类型设置为 Citrix 时。</span><span class="sxs-lookup"><span data-stu-id="ce61e-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ce61e-196">此集合可以包含最多 25 元素。</span><span class="sxs-lookup"><span data-stu-id="ce61e-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ce61e-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ce61e-197">authenticationMethod</span></span>|[<span data-ttu-id="ce61e-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ce61e-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ce61e-199">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ce61e-199">Authentication method.</span></span> <span data-ttu-id="ce61e-200">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="ce61e-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="ce61e-201">响应</span><span class="sxs-lookup"><span data-stu-id="ce61e-201">Response</span></span>
<span data-ttu-id="ce61e-202">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ce61e-202">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce61e-203">示例</span><span class="sxs-lookup"><span data-stu-id="ce61e-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce61e-204">请求</span><span class="sxs-lookup"><span data-stu-id="ce61e-204">Request</span></span>
<span data-ttu-id="ce61e-205">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce61e-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 989

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="ce61e-206">响应</span><span class="sxs-lookup"><span data-stu-id="ce61e-206">Response</span></span>
<span data-ttu-id="ce61e-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce61e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




