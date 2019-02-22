---
title: 创建 androidWorkProfileVpnConfiguration
description: 创建新的 androidWorkProfileVpnConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aabfed08848f0c3e68fadb557051afa48596e80f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140766"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="06676-103">创建 androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="06676-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="06676-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06676-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06676-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06676-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06676-106">创建新的[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="06676-106">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06676-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="06676-107">Prerequisites</span></span>
<span data-ttu-id="06676-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="06676-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="06676-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="06676-110">Permission type</span></span>|<span data-ttu-id="06676-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06676-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06676-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06676-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06676-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06676-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06676-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06676-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06676-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="06676-115">Not supported.</span></span>|
|<span data-ttu-id="06676-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="06676-116">Application</span></span>|<span data-ttu-id="06676-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="06676-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06676-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06676-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="06676-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="06676-119">Request headers</span></span>
|<span data-ttu-id="06676-120">标头</span><span class="sxs-lookup"><span data-stu-id="06676-120">Header</span></span>|<span data-ttu-id="06676-121">值</span><span class="sxs-lookup"><span data-stu-id="06676-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06676-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06676-122">Authorization</span></span>|<span data-ttu-id="06676-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06676-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06676-124">Accept</span><span class="sxs-lookup"><span data-stu-id="06676-124">Accept</span></span>|<span data-ttu-id="06676-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06676-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06676-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="06676-126">Request body</span></span>
<span data-ttu-id="06676-127">在请求正文中, 提供 androidWorkProfileVpnConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06676-127">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="06676-128">下表显示创建 androidWorkProfileVpnConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06676-128">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="06676-129">属性</span><span class="sxs-lookup"><span data-stu-id="06676-129">Property</span></span>|<span data-ttu-id="06676-130">类型</span><span class="sxs-lookup"><span data-stu-id="06676-130">Type</span></span>|<span data-ttu-id="06676-131">说明</span><span class="sxs-lookup"><span data-stu-id="06676-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06676-132">id</span><span class="sxs-lookup"><span data-stu-id="06676-132">id</span></span>|<span data-ttu-id="06676-133">String</span><span class="sxs-lookup"><span data-stu-id="06676-133">String</span></span>|<span data-ttu-id="06676-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06676-134">Key of the entity.</span></span> <span data-ttu-id="06676-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06676-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06676-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06676-136">lastModifiedDateTime</span></span>|<span data-ttu-id="06676-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06676-137">DateTimeOffset</span></span>|<span data-ttu-id="06676-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06676-138">DateTime the object was last modified.</span></span> <span data-ttu-id="06676-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06676-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06676-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06676-140">roleScopeTagIds</span></span>|<span data-ttu-id="06676-141">String collection</span><span class="sxs-lookup"><span data-stu-id="06676-141">String collection</span></span>|<span data-ttu-id="06676-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="06676-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06676-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06676-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06676-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="06676-144">supportsScopeTags</span></span>|<span data-ttu-id="06676-145">布尔</span><span class="sxs-lookup"><span data-stu-id="06676-145">Boolean</span></span>|<span data-ttu-id="06676-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="06676-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06676-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="06676-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06676-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="06676-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06676-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="06676-149">This property is read-only.</span></span> <span data-ttu-id="06676-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06676-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06676-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06676-151">createdDateTime</span></span>|<span data-ttu-id="06676-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06676-152">DateTimeOffset</span></span>|<span data-ttu-id="06676-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="06676-153">DateTime the object was created.</span></span> <span data-ttu-id="06676-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06676-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06676-155">description</span><span class="sxs-lookup"><span data-stu-id="06676-155">description</span></span>|<span data-ttu-id="06676-156">String</span><span class="sxs-lookup"><span data-stu-id="06676-156">String</span></span>|<span data-ttu-id="06676-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="06676-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06676-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06676-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06676-159">displayName</span><span class="sxs-lookup"><span data-stu-id="06676-159">displayName</span></span>|<span data-ttu-id="06676-160">String</span><span class="sxs-lookup"><span data-stu-id="06676-160">String</span></span>|<span data-ttu-id="06676-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="06676-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06676-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06676-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06676-163">version</span><span class="sxs-lookup"><span data-stu-id="06676-163">version</span></span>|<span data-ttu-id="06676-164">Int32</span><span class="sxs-lookup"><span data-stu-id="06676-164">Int32</span></span>|<span data-ttu-id="06676-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="06676-165">Version of the device configuration.</span></span> <span data-ttu-id="06676-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06676-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06676-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="06676-167">connectionName</span></span>|<span data-ttu-id="06676-168">字符串</span><span class="sxs-lookup"><span data-stu-id="06676-168">String</span></span>|<span data-ttu-id="06676-169">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="06676-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="06676-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="06676-170">connectionType</span></span>|[<span data-ttu-id="06676-171">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="06676-171">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="06676-172">连接类型。</span><span class="sxs-lookup"><span data-stu-id="06676-172">Connection type.</span></span> <span data-ttu-id="06676-173">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`、`paloAltoGlobalProtect`。</span><span class="sxs-lookup"><span data-stu-id="06676-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="06676-174">role</span><span class="sxs-lookup"><span data-stu-id="06676-174">role</span></span>|<span data-ttu-id="06676-175">字符串</span><span class="sxs-lookup"><span data-stu-id="06676-175">String</span></span>|<span data-ttu-id="06676-176">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="06676-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="06676-177">领域</span><span class="sxs-lookup"><span data-stu-id="06676-177">realm</span></span>|<span data-ttu-id="06676-178">字符串</span><span class="sxs-lookup"><span data-stu-id="06676-178">String</span></span>|<span data-ttu-id="06676-179">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="06676-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="06676-180">服务器</span><span class="sxs-lookup"><span data-stu-id="06676-180">servers</span></span>|<span data-ttu-id="06676-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="06676-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="06676-182">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="06676-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="06676-183">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="06676-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="06676-184">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="06676-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="06676-185">其次</span><span class="sxs-lookup"><span data-stu-id="06676-185">fingerprint</span></span>|<span data-ttu-id="06676-186">字符串</span><span class="sxs-lookup"><span data-stu-id="06676-186">String</span></span>|<span data-ttu-id="06676-187">指纹是一个字符串, 用于验证 VPN 服务器是否可以信任, 这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="06676-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="06676-188">customData</span><span class="sxs-lookup"><span data-stu-id="06676-188">customData</span></span>|<span data-ttu-id="06676-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06676-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="06676-190">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="06676-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="06676-191">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="06676-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="06676-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="06676-192">customKeyValueData</span></span>|<span data-ttu-id="06676-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06676-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="06676-194">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="06676-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="06676-195">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="06676-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="06676-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="06676-196">authenticationMethod</span></span>|[<span data-ttu-id="06676-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="06676-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="06676-198">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="06676-198">Authentication method.</span></span> <span data-ttu-id="06676-199">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="06676-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="06676-200">响应</span><span class="sxs-lookup"><span data-stu-id="06676-200">Response</span></span>
<span data-ttu-id="06676-201">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="06676-201">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06676-202">示例</span><span class="sxs-lookup"><span data-stu-id="06676-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="06676-203">请求</span><span class="sxs-lookup"><span data-stu-id="06676-203">Request</span></span>
<span data-ttu-id="06676-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06676-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06676-205">响应</span><span class="sxs-lookup"><span data-stu-id="06676-205">Response</span></span>
<span data-ttu-id="06676-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06676-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




