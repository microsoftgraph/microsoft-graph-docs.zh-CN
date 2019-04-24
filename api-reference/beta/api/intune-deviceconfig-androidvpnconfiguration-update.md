---
title: 更新 androidVpnConfiguration
description: 更新 androidVpnConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97c229584352b190bc7095bd8368bc6ed4a68688
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32475345"
---
# <a name="update-androidvpnconfiguration"></a><span data-ttu-id="77134-103">更新 androidVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="77134-103">Update androidVpnConfiguration</span></span>

> <span data-ttu-id="77134-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77134-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77134-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77134-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77134-106">更新[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77134-106">Update the properties of a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77134-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="77134-107">Prerequisites</span></span>
<span data-ttu-id="77134-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77134-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77134-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="77134-110">Permission type</span></span>|<span data-ttu-id="77134-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77134-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77134-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77134-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77134-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77134-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77134-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77134-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77134-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77134-115">Not supported.</span></span>|
|<span data-ttu-id="77134-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="77134-116">Application</span></span>|<span data-ttu-id="77134-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="77134-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77134-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77134-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="77134-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="77134-119">Request headers</span></span>
|<span data-ttu-id="77134-120">标头</span><span class="sxs-lookup"><span data-stu-id="77134-120">Header</span></span>|<span data-ttu-id="77134-121">值</span><span class="sxs-lookup"><span data-stu-id="77134-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77134-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77134-122">Authorization</span></span>|<span data-ttu-id="77134-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77134-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77134-124">接受</span><span class="sxs-lookup"><span data-stu-id="77134-124">Accept</span></span>|<span data-ttu-id="77134-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77134-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77134-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="77134-126">Request body</span></span>
<span data-ttu-id="77134-127">在请求正文中, 提供[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77134-127">In the request body, supply a JSON representation for the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

<span data-ttu-id="77134-128">下表显示创建[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="77134-128">The following table shows the properties that are required when you create the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span></span>

|<span data-ttu-id="77134-129">属性</span><span class="sxs-lookup"><span data-stu-id="77134-129">Property</span></span>|<span data-ttu-id="77134-130">类型</span><span class="sxs-lookup"><span data-stu-id="77134-130">Type</span></span>|<span data-ttu-id="77134-131">说明</span><span class="sxs-lookup"><span data-stu-id="77134-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77134-132">id</span><span class="sxs-lookup"><span data-stu-id="77134-132">id</span></span>|<span data-ttu-id="77134-133">String</span><span class="sxs-lookup"><span data-stu-id="77134-133">String</span></span>|<span data-ttu-id="77134-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="77134-134">Key of the entity.</span></span> <span data-ttu-id="77134-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77134-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77134-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77134-136">lastModifiedDateTime</span></span>|<span data-ttu-id="77134-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77134-137">DateTimeOffset</span></span>|<span data-ttu-id="77134-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="77134-138">DateTime the object was last modified.</span></span> <span data-ttu-id="77134-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77134-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77134-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77134-140">roleScopeTagIds</span></span>|<span data-ttu-id="77134-141">String collection</span><span class="sxs-lookup"><span data-stu-id="77134-141">String collection</span></span>|<span data-ttu-id="77134-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="77134-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="77134-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77134-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77134-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="77134-144">supportsScopeTags</span></span>|<span data-ttu-id="77134-145">布尔</span><span class="sxs-lookup"><span data-stu-id="77134-145">Boolean</span></span>|<span data-ttu-id="77134-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="77134-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="77134-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="77134-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="77134-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="77134-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="77134-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="77134-149">This property is read-only.</span></span> <span data-ttu-id="77134-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77134-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77134-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77134-151">createdDateTime</span></span>|<span data-ttu-id="77134-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77134-152">DateTimeOffset</span></span>|<span data-ttu-id="77134-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="77134-153">DateTime the object was created.</span></span> <span data-ttu-id="77134-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77134-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77134-155">description</span><span class="sxs-lookup"><span data-stu-id="77134-155">description</span></span>|<span data-ttu-id="77134-156">字符串</span><span class="sxs-lookup"><span data-stu-id="77134-156">String</span></span>|<span data-ttu-id="77134-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="77134-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="77134-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77134-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77134-159">displayName</span><span class="sxs-lookup"><span data-stu-id="77134-159">displayName</span></span>|<span data-ttu-id="77134-160">String</span><span class="sxs-lookup"><span data-stu-id="77134-160">String</span></span>|<span data-ttu-id="77134-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="77134-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="77134-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77134-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77134-163">version</span><span class="sxs-lookup"><span data-stu-id="77134-163">version</span></span>|<span data-ttu-id="77134-164">Int32</span><span class="sxs-lookup"><span data-stu-id="77134-164">Int32</span></span>|<span data-ttu-id="77134-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="77134-165">Version of the device configuration.</span></span> <span data-ttu-id="77134-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="77134-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="77134-167">connectionName</span><span class="sxs-lookup"><span data-stu-id="77134-167">connectionName</span></span>|<span data-ttu-id="77134-168">字符串</span><span class="sxs-lookup"><span data-stu-id="77134-168">String</span></span>|<span data-ttu-id="77134-169">向用户显示的连接名称。</span><span class="sxs-lookup"><span data-stu-id="77134-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="77134-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="77134-170">connectionType</span></span>|[<span data-ttu-id="77134-171">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="77134-171">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="77134-172">连接类型。</span><span class="sxs-lookup"><span data-stu-id="77134-172">Connection type.</span></span> <span data-ttu-id="77134-173">可取值为：`ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix`。</span><span class="sxs-lookup"><span data-stu-id="77134-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="77134-174">role</span><span class="sxs-lookup"><span data-stu-id="77134-174">role</span></span>|<span data-ttu-id="77134-175">字符串</span><span class="sxs-lookup"><span data-stu-id="77134-175">String</span></span>|<span data-ttu-id="77134-176">将 "连接类型" 设置为 "脉冲安全" 时的角色。</span><span class="sxs-lookup"><span data-stu-id="77134-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="77134-177">型</span><span class="sxs-lookup"><span data-stu-id="77134-177">realm</span></span>|<span data-ttu-id="77134-178">字符串</span><span class="sxs-lookup"><span data-stu-id="77134-178">String</span></span>|<span data-ttu-id="77134-179">连接类型设置为脉冲安全时的领域。</span><span class="sxs-lookup"><span data-stu-id="77134-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="77134-180">台</span><span class="sxs-lookup"><span data-stu-id="77134-180">servers</span></span>|<span data-ttu-id="77134-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md)集合</span><span class="sxs-lookup"><span data-stu-id="77134-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="77134-182">网络上的 VPN 服务器的列表。</span><span class="sxs-lookup"><span data-stu-id="77134-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="77134-183">请确保最终用户可以访问这些网络位置。</span><span class="sxs-lookup"><span data-stu-id="77134-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="77134-184">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="77134-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="77134-185">其次</span><span class="sxs-lookup"><span data-stu-id="77134-185">fingerprint</span></span>|<span data-ttu-id="77134-186">字符串</span><span class="sxs-lookup"><span data-stu-id="77134-186">String</span></span>|<span data-ttu-id="77134-187">指纹是一个字符串, 用于验证 VPN 服务器是否可以信任, 这仅在连接类型为 "检查点胶囊" VPN 时适用。</span><span class="sxs-lookup"><span data-stu-id="77134-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="77134-188">customData</span><span class="sxs-lookup"><span data-stu-id="77134-188">customData</span></span>|<span data-ttu-id="77134-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77134-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="77134-190">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="77134-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="77134-191">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="77134-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="77134-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="77134-192">customKeyValueData</span></span>|<span data-ttu-id="77134-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77134-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="77134-194">将连接类型设置为 Citrix 时的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="77134-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="77134-195">此集合最多可包含25个元素。</span><span class="sxs-lookup"><span data-stu-id="77134-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="77134-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77134-196">authenticationMethod</span></span>|[<span data-ttu-id="77134-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="77134-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="77134-198">身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="77134-198">Authentication method.</span></span> <span data-ttu-id="77134-199">可取值为：`certificate`、`usernameAndPassword`。</span><span class="sxs-lookup"><span data-stu-id="77134-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="77134-200">响应</span><span class="sxs-lookup"><span data-stu-id="77134-200">Response</span></span>
<span data-ttu-id="77134-201">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="77134-201">If successful, this method returns a `200 OK` response code and an updated [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77134-202">示例</span><span class="sxs-lookup"><span data-stu-id="77134-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="77134-203">请求</span><span class="sxs-lookup"><span data-stu-id="77134-203">Request</span></span>
<span data-ttu-id="77134-204">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77134-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 978

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="77134-205">响应</span><span class="sxs-lookup"><span data-stu-id="77134-205">Response</span></span>
<span data-ttu-id="77134-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77134-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
  "id": "d4c48852-8852-d4c4-5288-c4d45288c4d4",
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





